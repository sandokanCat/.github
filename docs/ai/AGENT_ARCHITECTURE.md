# AI coding-agent instruction architecture

This document records the implementation choices for sharing one project instruction source across coding agents. Vendor products and configuration schemas evolve; verify official documentation before changing adapters.

## Decision

- Canonical project-wide instructions live in the repository-root `AGENTS.md`.
- Tool-specific files exist only where an agent requires a native discovery mechanism. They must be minimal adapters, not independent policy documents.
- Do not assume every agent interprets Markdown links, `@file` syntax, or arbitrary settings identically. A reference is not equivalent to automatic inclusion unless documented.
- Path-scoped rules are exceptions for genuinely file-specific constraints, not a second home for general policy. This repository currently has no active path-specific AI rules.
- Load detailed documentation from `docs/` on demand. Do not put the entire documentation tree in every prompt.

## Current adapters

| Tool | Native discovery mechanism | Implementation |
|---|---|---|
| OpenAI Codex and compatible AGENTS.md agents | Root `AGENTS.md`, with nested files for scoped rules | Read root `AGENTS.md` directly; no duplicate adapter is needed. |
| VS Code Local agent harness | Root `AGENTS.md` via `chat.useAgentsMdFile` | Enable the setting; this setting applies to the Local harness, not all Copilot sessions. |
| GitHub Copilot | `.github/copilot-instructions.md`; AGENTS.md support varies by feature/surface | Keep a short adapter directing the agent to root `AGENTS.md`. Copilot surfaces do not all support the same instruction formats. |
| Claude Code | Root `CLAUDE.md`; supports importing Markdown files with `@path` | Root `CLAUDE.md` contains only `@AGENTS.md`. |
| Gemini CLI | Context files default to `GEMINI.md`; `context.fileName` can select another filename | Configure `.gemini/settings.json` with `context.fileName: "AGENTS.md"`; no duplicate GEMINI.md policy. |
| OpenCode | Root `AGENTS.md` is discovered automatically; `instructions` can add other files | Use the root file. Do not place a project adapter under `.config/opencode/`, which is configuration storage rather than the project-root instruction location. OpenCode does not automatically interpret arbitrary `@file` references in AGENTS.md. |
| Aider | `.aider.conf.yml` supports a `read` list of read-only context files | Configure `read: [AGENTS.md]`. |
| Cursor | Project rules under `.cursor/rules`; AGENTS.md support depends on current product/version | Prefer native AGENTS.md discovery where supported; add a minimal adapter only if the target version requires it. |
| Windsurf | `.windsurfrules` historically; newer versions support scoped rule files | Verify installed version before adding an adapter. Do not add duplicate rules speculatively. |
| Cline / Roo Code | Project instructions and custom rule files, with support varying by product/version | Verify current settings and discovery behavior before adding a compatibility file. |
| Continue and other IDE/CLI agents | Product-specific rules/configuration and varying AGENTS.md support | Prefer native AGENTS.md support; otherwise use a thin adapter and verify actual loading. |

## Historical patterns and migration guidance

Instruction mechanisms evolved from prompt text repeated manually, to project convention files loaded with commands, to root-level agent files, and then to scoped rules, skills, hooks, and tool-specific configuration. Examples include Aider's `--read`/configuration `read` option, Claude Code's `CLAUDE.md` and imports, Gemini CLI's `GEMINI.md` context hierarchy, Copilot's repository-wide and path-specific instruction files, and OpenCode's automatic `AGENTS.md` discovery.

The modern shared-file strategy is not to force one filename on every client regardless of support. Keep one canonical policy file and use the smallest documented compatibility bridge for clients that need another entry point. Add native path-specific instructions only when requirements genuinely depend on file paths, and link them back to the canonical policy rather than copying general rules.

## Validation checklist

1. Check current official documentation for each affected tool and relevant product/version.
2. Verify exact filename, schema, path resolution, and import/reference semantics.
3. Check whether the client automatically loads the canonical file or merely displays a pointer.
4. Validate JSON/YAML syntax and remove redundant adapters only when no supported client depends on them.
5. Inspect all changed paths and the final diff; keep non-AI project files untouched.
6. Record implementation changes and any unverified client-specific behavior in `CHANGELOG.md`.

## Official references

- VS Code custom instructions and AGENTS.md: https://code.visualstudio.com/docs/agent-customization/custom-instructions
- VS Code AI settings: https://code.visualstudio.com/docs/agents/reference/ai-settings
- GitHub Copilot custom instructions: https://docs.github.com/en/copilot/concepts/prompting-and-context/custom-instructions
- GitHub Copilot format support by surface: https://docs.github.com/en/copilot/reference/custom-instructions-support
- Gemini CLI context files: https://geminicli.com/docs/cli/gemini-md/
- Gemini CLI settings: https://geminicli.com/docs/reference/configuration/
- OpenCode rules and instruction loading: https://docs.opencode.ai/docs/rules/
- Aider configuration: https://aider.chat/docs/config/aider_conf.html
- Aider conventions/read-only context: https://aider.chat/docs/usage/conventions.html
- Claude Code memory and project instructions: https://docs.anthropic.com/en/docs/claude-code/memory

## Scope and limitations

This is a practical compatibility survey, not a claim to enumerate every AI model, coding assistant, fork, or version in existence. Model providers and coding-agent clients are different layers: instructions are generally interpreted by the client/harness, not inherently by the model. Validate the actual client and version rather than assuming all models share a common instruction-file protocol.
