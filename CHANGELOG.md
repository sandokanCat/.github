# Changelog

All notable changes to this repository are documented in this file.

This changelog follows the [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) format. Entries are grouped by commit date; no release versions are implied where no release has been published.

## [Unreleased]

### Added
- Expanded the AI instruction architecture survey to include Amp, Cursor, Zed, Cline, Roo Code, JetBrains Junie CLI, Kiro, and additional editor/CLI harnesses, with official documentation and guidance on when adapters are unnecessary.

### Changed
- Clarified that Claude Code v2.1.277+ supports native `AGENTS.md` discovery, but an applicable `CLAUDE.md` can take precedence; retained the tiny import bridge for backward compatibility.
- Documented that Gemini CLI can use `AGENTS.md` through `.gemini/settings.json` without maintaining `GEMINI.md`.
- Clarified that Copilot's `.github/copilot-instructions.md` is a native natural-language Markdown format, and that support for `AGENTS.md` differs by product surface.
- Confirmed that Cursor, Zed, Cline, Roo Code, Junie CLI, and Amp have documented `AGENTS.md` support; no redundant native adapter files were added for these clients.
- Documented why Kiro and other configurable rule systems do not automatically receive the canonical instructions merely because an adapter links to `AGENTS.md`.

### Previously documented
- Added a cross-agent instruction architecture reference at `docs/ai/AGENT_ARCHITECTURE.md`, including discovery mechanisms, migration history, official documentation, and validation guidance.
- Added canonical, stack-neutral coding-agent instructions to root `AGENTS.md`, including an on-demand index for relevant documentation under `docs/`.
- Recorded the AI instruction setup work from 2026-10-24 that was not previously represented here: [Gemini CLI settings](https://github.com/sandokanCat/.github/commit/ebac9c8d77af3999929ae328d94072b42cc4cb15), [Claude settings](https://github.com/sandokanCat/.github/commit/2f543bba0f7fe96ee130b46f7d58cef213cad712), [Claude import bridge](https://github.com/sandokanCat/.github/commit/f7ed3f6b3bb4464d348878d55d9beec9f7a0de0d), [Copilot adapter](https://github.com/sandokanCat/.github/commit/5e81cbf1ae6cccc2070ac8312bb772acc0070801), [OpenCode adapter](https://github.com/sandokanCat/.github/commit/72f375b05c255c49adca5e1a0a477ac4f0324dcd), and [VS Code settings](https://github.com/sandokanCat/.github/commit/d5708aaeee910d687bf81b5b085e5968dd5cfbdc).

## [2026-10-22]

### Added
- Added the initial `manifest.json` file.

## [2026-10-21]

### Added
- Added the initial VS Code task configuration and root-level license-exception file.

## [2026-10-20]

### Added
- Added repository-wide documentation placeholders and expanded `SUMMARY.md` into a categorized index of repository files.
- Added community-health and contribution resources, including issue and discussion templates, a pull request template, support guidance, a code of conduct, security guidance, governance documentation, and code ownership metadata.
- Added instructions for GitHub Copilot, Claude, Gemini, and compatible coding agents, together with a reusable skill definition.
- Added MkDocs and Docusaurus configuration files and documentation entry points.
- Added citation metadata, accessibility guidance, and an EditorConfig file.
- Added the repository's MIT license.
- Added root-level placeholders and site metadata mirrored from the CV repository, including sitemap-related files and search-engine verification placeholders.

### Changed
- Renamed the `skills/` directory to `badges/`.
- Updated funding configuration and sitemap-related files.

### Removed
- Removed the root-level `DESIGN.md` file after its initial addition.

## [2026-10-18]

### Added
- Moved reusable skill assets and VS Code configuration into this shared repository.
- Added auxiliary files from the RenderCV and GitHub Stats Extended repositories.
- Added a scheduled/manual upstream synchronization workflow.
- Added a README documenting archived workflows.

### Changed
- Updated the Patreon username in the funding configuration.
- Merged Dependabot updates for Axios and the Python dependency group used by RenderCV.

## [2026-10-11]

### Changed
- Updated the Patreon username to `sandokanLair`.

## [2026-10-05]

### Added
- Initialized the repository with default community-health information and funding configuration.

### Changed
- Moved `FUNDING.yml` into the `.github/` directory so GitHub can use the repository-level funding configuration.
