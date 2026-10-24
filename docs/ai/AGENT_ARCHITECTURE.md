# AI coding-agent instruction compatibility matrix

This repository is a reusable template, not a specific application. Its goal is to provide prepared entry points for mainstream and historically common coding-agent clients, IDE integrations, CLI tools, and hosted agents while keeping root `AGENTS.md` as the canonical policy.

Compatibility is version- and surface-dependent. No repository can guarantee that every arbitrary model, wrapper, fork, remote agent, or old release reads any file automatically. A client must implement discovery or be explicitly configured to read a file. A pointer in a file is not the same as a host-level include unless that client resolves it.

## Architecture and invariants

1. Root `AGENTS.md` is the canonical, complete project-wide instruction document.
2. Native entry-point files are compatibility shims. Prefer a documented include/import when supported; otherwise give a concise directive to read root `AGENTS.md`.
3. Legacy adapters are intentionally checked in even if modern versions can read `AGENTS.md` directly. This is a template repository and downstream projects may choose which adapters to copy.
4. Do not delete an adapter merely because a current version has native support. The target project may use an older version, another product surface, or a wrapper.
5. Do not assume a CLI, IDE extension, hosted coding agent, API model, and third-party harness share the same discovery rules.
6. Do not place secrets, machine-specific credentials, private notes, or personal preferences in repository instruction files.
7. Keep policy in `AGENTS.md`; use scoped rule files only to select/include the canonical policy or to add genuinely path-specific rules. Do not maintain conflicting copies of policy.
8. Validate actual loaded context in the client before relying on an adapter. Use the tool's context/memory/rules command or UI when available.

## Prepared entry points in this template

| Client/tool family | Prepared path(s) | Mechanism and compatibility notes |
|---|---|---|
| OpenAI Codex CLI / IDE integrations | `AGENTS.md`, `AGENT.md`, optional `codex.md` fallback | Codex natively discovers `AGENTS.md`; `codex.md` is only relevant when explicitly configured as a fallback. |
| Claude Code | `CLAUDE.md`, `.claude/CLAUDE.md`, `.claude/settings.json` | `CLAUDE.md` imports `@AGENTS.md`. This covers the long-standing native filename; recent Claude Code versions can also discover AGENTS.md, subject to precedence. The existing plugin settings are preserved as a separate mechanism. |
| Gemini CLI | `GEMINI.md`, `.gemini/settings.json`, `.agents/rules/project.md` | `GEMINI.md` imports `@./AGENTS.md` for default/older behavior. Settings select `AGENTS.md` directly on versions supporting `context.fileName`. |
| GitHub Copilot (GitHub, IDE, CLI surfaces) | `.github/copilot-instructions.md`, `.github/instructions/project.instructions.md` | Repository-wide and path-scoped instruction formats. Support varies by surface; the short natural-language bridge remains for broad compatibility. |
| VS Code agent harness | `.vscode/settings.json`, root `AGENTS.md`, Copilot instruction files | Enables root/nested AGENTS.md, Claude Markdown instructions, and referenced instructions for the VS Code Local harness where supported. These settings do not force every external agent or hosted Copilot surface to use the same loader. |
| Cursor | `AGENTS.md`, `.cursorrules`, `.cursor/rules/project.mdc` | Native AGENTS.md support in current versions; legacy root rule and modern MDC rule formats prepared for older/different workflows. MDC `@AGENTS.md` inclusion depends on Cursor's rule include support. |
| Windsurf / Cascade / Devin Desktop transitions | `AGENTS.md`, `.windsurfrules`, `.windsurf/rules/project.md`, `.devin/rules/project.md` | Legacy and newer rule entry points are provided. Exact discovery depends on product generation and version; verify loaded rules. |
| Zed Agent | `AGENTS.md`, `.rules`, and other shared legacy filenames | Zed searches a list of common rule files, including AGENTS.md and legacy Cursor/Windsurf/Cline/Copilot/Claude/Gemini names. External agents and terminal threads have independent loaders. |
| OpenCode | `AGENTS.md` | Native discovery; the `.config/opencode/` directory is for OpenCode configuration, not a required project instruction shim. |
| Aider | `.aider.conf.yml`, `CONVENTIONS.md` | Explicit read-only context via `read:`; historical Aider convention workflows can use a conventions file. Verify config precedence for CLI/global/project usage. |
| Amp | `AGENTS.md`, optional `AGENT.md` | Native AGENTS.md discovery and historical fallback names documented by Amp. |
| Cline | `.clinerules`, `.cline/rules/project.md`, `AGENTS.md` | Legacy single-file and modern directory rule formats; AGENTS.md support is available in current versions. |
| Roo Code | `.roorules`, `.roo/rules/AGENTS.md`, `AGENTS.md` | Legacy and directory rule formats prepared; verify exact enabled rule mode/version. |
| Kilo Code | `AGENTS.md`, `AGENT.md` | Native discovery; Kilo documents `AGENT.md` as a fallback and supports legacy `.kilo/rules/` and `.kilocode/rules/` content. No duplicate Kilo rule is needed for general policy. |
| ZCode Agent | `AGENTS.md` | Native workspace instruction support; it does not expand imports or merge nested AGENTS.md files, so keep essential policy in the root file. |
| Google Jules | `AGENTS.md` | Repository instructions are supported natively; no separate adapter is needed. |
| Antigravity | `GEMINI.md`, `AGENTS.md` depending on surface | Keep `GEMINI.md` as the compatibility entry point; Antigravity rules are prepared under `.agents/rules/`; Antigravity and Gemini CLI are related products but not interchangeable loaders. |
| Factory Droid | `AGENTS.md` | Current harnesses support shared AGENTS.md instructions; verify the specific product/runtime before assuming identical behavior. |
| Kimi Code CLI | `AGENTS.md` | Reported as a native AGENTS.md client in current tooling; verify the actual version and runtime. |
| Qoder CLI | `AGENTS.md` | Reported as a native AGENTS.md client in current tooling; verify the actual version and runtime. |
| Grok CLI | `AGENTS.md` | Reported as a native AGENTS.md client in current tooling; verify the actual version and runtime. |
| Pi coding agent | `AGENTS.md` | Native/shared instruction discovery; external wrappers can alter behavior. |
| Hermes and Mastra Code | `AGENTS.md` | Emerging clients reported to use AGENTS.md; treat as provisional until confirmed against official release documentation. |
| JetBrains Junie | `.junie/AGENTS.md`, `AGENTS.md`, `.junie/guidelines.md` | Current AGENTS.md and legacy guidelines paths prepared. Junie CLI's documented discovery order gives `.junie/AGENTS.md` precedence over root AGENTS.md. |
| Qwen Code | `QWEN.md`, `.qwen/rules/project.md`, `AGENTS.md` | QWEN.md supports legacy/default context; modern rules live under `.qwen/rules/`. A directive to read AGENTS.md is a fallback instruction, not a host-level import guarantee. |
| Goose | `.goosehints`, `AGENTS.md` | Goose-specific hints file prepared for clients using the legacy native name; verify current project discovery behavior. |
| Augment Code | `.augment-guidelines`, `AGENTS.md` | Native guideline filename prepared for older/current integrations. |
| Amazon Q Developer | `.amazonq/rules/project.md`, `AGENTS.md` | Native rule path prepared; rule schema and inclusion behavior can differ by Q Developer surface/version. |
| Kiro | `.kiro/steering/00-project.md`, `AGENTS.md` | Native steering file uses `inclusion: always`; its content directs the agent to the canonical policy. A pointer only works if the agent can access the workspace file. |
| Continue | `.continue/rules/project.md`, `AGENTS.md` | Rule/context file prepared. Configure it as a rule source for versions that do not automatically discover AGENTS.md. |
| Trae | `.trae/rules/project.md`, `AGENTS.md` | Native rule directory entry point prepared; schema and loading depend on product/version. |
| OpenHands | `.openhands/microagents/repo.md`, `AGENTS.md` | Repository microagent compatibility path prepared. Confirm the deployed OpenHands version's microagent format. |
| Devin | `.devin/rules/project.md`, `AGENTS.md` | Workspace rule pointer prepared; hosted configuration and context access depend on the Devin environment. |
| Warp AI | `WARP.md`, `AGENTS.md` | Legacy/common project entry point prepared; verify current Warp Agent discovery. |
| Replit Agent | `replit.md`, `AGENTS.md` | Compatibility pointer prepared for workflows that read Replit project guidance; do not assume all Replit agent modes load it. |
| Generic/unknown agents | `AGENTS.md`, `AGENT.md`, `.rules`, `.github/copilot-instructions.md`, `CONVENTIONS.md`, `WARP.md`, `replit.md`, `codex.md`, `.agents/rules/project.md`, `.crush/CRUSH.md` | Common filenames improve the odds of discovery, but unknown clients must be explicitly pointed to root AGENTS.md. |

## Historical and alternate usage modes

- **CLI launched at repository root:** root AGENTS.md is usually easiest to discover. Check current working directory and ancestor-search rules.
- **CLI launched from a nested directory:** clients differ on ancestor traversal and nested instruction merging. Keep root AGENTS.md in place; add nested AGENTS.md only for genuinely scoped requirements.
- **IDE/local agent:** the extension or host may have its own instruction loader, settings toggle, trust mode, and context UI. Enable only documented settings and inspect the effective context.
- **Hosted/external agent:** repository-specific settings, permissions, or supported filenames may differ from the local CLI. A repository file cannot force an external service to load it.
- **API/model-only usage:** models do not autonomously search repository files unless the caller supplies tools/context. The integration must read AGENTS.md and pass its content in the request.
- **Older releases:** prefer their native historical filename or rule directory as a bridge. Imports such as `@AGENTS.md` only work in clients that implement that syntax.
- **Multiple instruction files:** some clients concatenate all matching files; others use the first match, nearest file, or precedence hierarchy. Avoid putting contradictory policy in multiple files.
- **Trusted-workspace modes:** some clients suppress project rules until the workspace is trusted or the user approves repository context.
- **Rules, skills, commands, hooks, MCP and agent definitions:** these are separate extension mechanisms. Do not treat them as substitutes for always-on project instructions. Add them only when the project actually needs the feature.
- **Global user instructions:** files under home directories (for example `~/.codex`, `~/.claude`, `~/.gemini`) are not appropriate for this repository template; they belong to individual machine/user setup.

## Maintaining this template

When adding an adapter:

1. Identify the exact product, surface (CLI, IDE, hosted, API harness), version range, and documented native filename.
2. Prefer the official documentation. Community matrices are useful for discovery, not final authority.
3. Add the native file only if it improves discovery for a real historical or current client.
4. Keep the adapter concise. Use a documented import where supported; otherwise say explicitly to read root `AGENTS.md`.
5. Do not claim a textual pointer guarantees context injection. Verify the client can read workspace files.
6. Update this matrix and `SUMMARY.md`. Add a `CHANGELOG.md` entry only when the change is notable for a planned or published release; record durable decisions in `docs/decisions/DECISIONS.md`.
7. Validate JSON/YAML/frontmatter syntax and review every changed path.

## Official references

- Claude Code project memory and imports: https://docs.anthropic.com/en/docs/claude-code/memory
- Gemini CLI context files and imports: https://geminicli.com/docs/cli/gemini-md/
- Gemini CLI settings: https://geminicli.com/docs/reference/configuration/
- GitHub Copilot custom instructions: https://docs.github.com/en/copilot/concepts/prompting-and-context/custom-instructions
- GitHub Copilot support by surface: https://docs.github.com/en/copilot/reference/custom-instructions-support
- VS Code custom instructions: https://code.visualstudio.com/docs/agent-customization/custom-instructions
- Cursor rules: https://cursor.com/docs/rules
- Zed instructions and supported filenames: https://zed.dev/docs/ai/instructions
- Kilo Code AGENTS.md: https://github.com/Kilo-Org/kilocode/blob/main/packages/kilo-docs/pages/customize/agents-md.md
- ZCode Agent instructions: https://zcode.z.ai/en/docs/agents
- Google Jules: https://jules.google/docs/
- OpenCode rules: https://docs.opencode.ai/docs/rules/
- Aider configuration: https://aider.chat/docs/config/aider_conf.html
- Amp AGENTS.md: https://ampcode.com/docs/customize/agents-md
- Qwen Code rules: https://qwenlm.github.io/qwen-code-docs/en/users/features/rules/
- JetBrains Junie guidelines and discovery order: https://junie.jetbrains.com/docs/guidelines-and-memory.html
- Cline rules: https://docs.cline.bot/customization/cline-rules
- Roo Code custom instructions: https://docs.roocode.com/features/custom-instructions
- Amazon Q Developer rules files: https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/context-project-rules.html
- Goose hints: https://block.github.io/goose/docs/guides/context-engineering/using-goosehints/
- OpenHands microagents: https://docs.all-hands.dev/usage/prompting/microagents-overview
- Windsurf rules: https://docs.windsurf.com/windsurf/cascade/memories
- Replit Agent: https://docs.replit.com/replitai/agent
- Warp Agent: https://docs.warp.dev/agents/rules

## Scope and limitations

This is a compatibility template, not a guarantee of universal discovery. Tool support changes quickly, and a model is not the same thing as its client. Where official documentation does not clearly guarantee a path, the matrix says so rather than inventing certainty. For a project, copy only the adapters needed by the target tools and versions, then test the effective instruction context.
