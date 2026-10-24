# AI coding-agent instruction architecture

This document records how coding agents discover shared project instructions. Vendor schemas and capabilities evolve; verify official documentation before changing adapters.

## Decision

- Canonical project-wide instructions live in root `AGENTS.md`.
- Add tool-specific files only when a client needs a native discovery mechanism. Keep them as minimal adapters, never duplicate policy.
- A Markdown link, an `@file` import, and a settings option are different mechanisms. A pointer is not automatic inclusion unless the client documents and supports it.
- Path-scoped rules are for genuinely file-specific constraints, not a second home for general policy.
- Load detailed `docs/` content on demand instead of injecting the whole documentation tree into every prompt.

## Discovery matrix

| Agent/client | Native discovery and implementation | Need an adapter here? |
|---|---|---|
| OpenAI Codex CLI | Root `AGENTS.md`; nested files can scope instructions | No |
| Amp | Root/parent/subtree `AGENTS.md`; `@file` references supported | No |
| Claude Code | Current versions support root `AGENTS.md`, but an applicable `CLAUDE.md` can take precedence. Direct AGENTS support requires v2.1.277+; older versions need a `CLAUDE.md` import | Yes: root `CLAUDE.md` imports `@AGENTS.md` for compatibility |
| Gemini CLI | Defaults to `GEMINI.md`; `.gemini/settings.json` can set `context.fileName` to `AGENTS.md` | Yes: existing settings file |
| GitHub Copilot | Support differs by surface. Repository instructions use `.github/copilot-instructions.md`; Copilot coding agent and CLI also support AGENTS.md in documented cases | Keep the minimal repository instructions bridge for broad surface compatibility |
| VS Code Local agent harness | Can load root `AGENTS.md` with `chat.useAgentsMdFile`; `chat.includeReferencedInstructions` follows Markdown-linked instruction files | Existing settings enable both; not a guarantee for every Copilot surface |
| OpenCode | Discovers root `AGENTS.md` automatically | No; do not put a redundant instruction file in `.config/opencode/` |
| Aider | Supports read-only context files through `read` in `.aider.conf.yml` | Yes: existing config |
| Cursor | Reads root and nested `AGENTS.md`; `.cursor/rules/*.mdc` is an alternative for scoped rules | No |
| Zed Agent | Searches known formats including `AGENTS.md`, `CLAUDE.md`, `.github/copilot-instructions.md` and legacy rule filenames | No |
| Cline | Supports root `AGENTS.md` alongside its native `.clinerules/` and `.cline/rules/` formats | No |
| Roo Code | Loads root `AGENTS.md` by default; `AGENT.md` is a fallback | No |
| JetBrains Junie CLI | Reads root `AGENTS.md`; also supports `.junie/AGENTS.md` and legacy guideline formats | No |
| Windsurf | Has native rules formats; exact AGENTS.md behavior depends on product/version and should be verified before relying on it | No adapter added without verified need |
| Continue | Supports configurable rules/context; discovery depends on product and configuration version | No adapter added without verified need |
| Amazon Q Developer / Kiro | Kiro uses `.kiro/steering/*.md`; this is a distinct steering system, not a universal AGENTS.md import mechanism | No adapter: a pointer alone would not guarantee instructions are loaded |
| Other ACP/editor agents | Behavior depends on the actual agent and harness; ACP itself does not imply a shared instruction protocol | Verify the concrete client before adding files |

## Implementation in this repository

- `AGENTS.md` is the canonical, stack-neutral policy.
- `CLAUDE.md` contains only `@AGENTS.md`.
- `.gemini/settings.json` configures Gemini CLI to use `AGENTS.md`.
- `.github/copilot-instructions.md` is a concise natural-language bridge for Copilot surfaces that consume repository instructions.
- `.aider.conf.yml` loads `AGENTS.md` as read-only context.
- `.vscode/settings.json` enables AGENTS.md support and referenced Markdown instructions.
- OpenCode, Cursor, Zed, Cline, Roo Code, Junie CLI, Amp, and Codex already support the canonical filename in documented configurations, so adding duplicate agent files would create unnecessary maintenance.
- Do not create `.cursor/rules`, `.junie/AGENTS.md`, `.clinerules/`, `.roo/rules`, `.windsurfrules`, or `.kiro/steering/` just to repeat a general policy. Use these native mechanisms only for actual scoped features or where verified client limitations require them.

## Why Copilot's file uses natural language

`.github/copilot-instructions.md` is itself a Markdown instruction document. Natural language is the expected format, not a fallback or inferior syntax. The file here intentionally stays short to avoid duplicating the canonical policy. Copilot support differs by surface, so check the official compatibility table before assuming that a particular GitHub or IDE feature reads a given file.

## Historical patterns

Instruction mechanisms evolved from prompt text repeated manually, to product-specific context files, to shared root-level `AGENTS.md`, then to scoped rules, skills, hooks, and client configuration. Examples include Aider's `--read`/configuration `read`, Claude Code's `CLAUDE.md` imports, Gemini CLI's `GEMINI.md` hierarchy, Copilot's repository and path-specific instructions, and OpenCode's automatic AGENTS.md discovery.

The robust strategy is not to force every client to use one filename irrespective of support. Keep one source of truth and the smallest documented compatibility bridge for clients that need another entry point. Models and clients are different layers: instruction discovery is generally a client/harness feature, not an inherent capability of the underlying model.

## Validation checklist

1. Verify official docs for the actual client and version.
2. Check filename, schema, path resolution, and whether imports are actually expanded.
3. Validate JSON/YAML syntax.
4. Confirm the adapter does not duplicate or conflict with `AGENTS.md`.
5. Review changed paths and final diff; keep unrelated files untouched.
6. Record changes and unresolved compatibility questions in `CHANGELOG.md`.

## Official references

- Claude Code memory and project instructions: https://docs.anthropic.com/en/docs/claude-code/memory
- Gemini CLI context files: https://geminicli.com/docs/cli/gemini-md/
- Gemini CLI settings: https://geminicli.com/docs/reference/configuration/
- GitHub Copilot custom instructions: https://docs.github.com/en/copilot/concepts/prompting-and-context/custom-instructions
- GitHub Copilot support by surface: https://docs.github.com/en/copilot/reference/custom-instructions-support
- VS Code custom instructions: https://code.visualstudio.com/docs/agent-customization/custom-instructions
- VS Code AI settings: https://code.visualstudio.com/docs/agents/reference/ai-settings
- OpenCode rules: https://docs.opencode.ai/docs/rules/
- Aider configuration: https://aider.chat/docs/config/aider_conf.html
- Cursor rules and AGENTS.md: https://cursor.com/docs/rules
- Zed instructions: https://zed.dev/docs/ai/instructions
- Cline rules: https://docs.cline.bot/customization/cline-rules
- Roo Code custom instructions: https://docs.roocode.com/features/custom-instructions
- JetBrains Junie guidelines: https://junie.jetbrains.com/docs/guidelines-and-memory.html
- Amp AGENTS.md: https://ampcode.com/docs/customize/agents-md
- AWS Agent Toolkit rules files: https://docs.aws.amazon.com/agent-toolkit/latest/userguide/rules-files.html

## Scope and limitations

This is a practical survey of widely used and emerging coding agents, not an exhaustive inventory of every model, IDE plugin, fork, and release. Product support can change quickly. Do not add compatibility files based only on a historical convention or a marketing claim; verify current discovery behavior for the target client.
