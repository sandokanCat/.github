# Changelog

All notable changes to this repository are documented in this file.

This changelog follows the [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) format. Entries are grouped by commit date; no release versions are implied where no release has been published.

## [Unreleased]

### Added
- Expanded the AI template with historical and current compatibility entry points for Gemini, Cursor, Windsurf, Zed, Cline, Roo Code, Qwen Code, Kiro, Junie, Goose, Augment, Amazon Q, Continue, Trae, OpenHands, Devin, Warp, Replit, and generic/legacy clients.
- Added `docs/ai/AGENT_ARCHITECTURE.md` as a detailed compatibility matrix covering CLI, IDE/local, hosted/external, API-harness, nested-directory, and historical-version scenarios.
- Added alternate common filenames (`AGENT.md`, `CONVENTIONS.md`, `WARP.md`, `replit.md`, `.rules`) for clients that use these conventions.

### Changed
- Kept root `AGENTS.md` as canonical policy while retaining vendor-specific entry points as thin compatibility shims for a reusable template.
- Added `GEMINI.md` with a native import of `AGENTS.md` for default/older Gemini CLI setups while retaining `.gemini/settings.json` for versions configured to load `AGENTS.md` directly.
- Added both legacy and modern rule locations for tools whose discovery conventions have changed over time.
- Documented that textual pointers cannot guarantee host-level context injection, and that every hosted/API/local/CLI surface must be validated independently.
- Preserved existing Claude plugin settings and Copilot/VS Code configuration while preparing additional native instruction locations.
- Updated the architecture and changelog to distinguish confirmed native support from version-dependent or unverified compatibility.

### Previously documented
- Canonical, stack-neutral coding-agent instructions in root `AGENTS.md`, with an on-demand index to relevant documentation under `docs/`.
- Minimal Claude, Copilot, Gemini, Aider, and VS Code setup and the earlier AI instruction commits; see the repository history for those changes.

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
