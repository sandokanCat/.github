# Documentation index

This index is the primary entry point for repository documentation. The repository is a reusable GitHub community-health and configuration repository, not a single application. Many paths under docs/ are planned templates or placeholders; a filename alone does not make a document an active policy. Treat only populated, relevant documents as authoritative.

## Start here

- [Repository overview](../README.md) — purpose and scope of this shared repository.
- [Repository instructions](../AGENTS.md) — canonical project-wide instructions for coding agents.
- [AI instruction architecture](./ai/AGENT_ARCHITECTURE.md) — supported entry points, compatibility caveats, and the single-source-of-truth model.
- [Contribution guide](./CONTRIBUTING.md) — change scope, documentation conventions, validation, and review expectations.
- [Development summary](../SUMMARY.md) — date- and type-grouped work log with links to the original commits.
- [Changelog](../CHANGELOG.md) — notable changes organized by release, following [Keep a Changelog 2.0.0](https://keepachangelog.com/en/2.0.0/).
- [Version record](../VERSION.md) — status and scope of the current release or prerelease.
- [Decision register](./decisions/DECISIONS.md) — durable team decisions and their rationale.
- [Release process](./releases/RELEASE_PROCESS.md) — release preparation and publication workflow.
- [Tagging conventions](./releases/TAGGING.md) — version-tag naming and immutable release anchors.
- [Release checklist](./releases/RELEASE_CHECKLIST.md) — final checks before publication.

## Documentation areas

Use these directories as topic indexes when the relevant documents have been populated:

- ai/ — coding-agent instruction architecture and AI-related policy.
- architecture/ — system boundaries, architecture, components, and technical design.
- build/ and development/ — development workflow, toolchain, and build guidance.
- community/ — collaboration, maintainership, and community operations.
- decisions/, adr/, and rfcs/ — decisions, architecture decision records, and proposals.
- deployment/ and operations/ — deployment and operational procedures.
- installation/ — setup and installation guidance.
- releases/ — release lifecycle, versioning, compatibility, and release procedures.
- security/ and privacy/ — security controls, privacy, and data handling.
- testing/ — testing strategy and quality assurance.

## Change and release records

Each record has one responsibility:

| File | Purpose |
| --- | --- |
| [SUMMARY.md](../SUMMARY.md) | Complete, high-level work log; all commits grouped by UTC date and logical type, with each commit linked. |
| [CHANGELOG.md](../CHANGELOG.md) | Curated, user-facing notable changes by version; never a raw commit log. |
| [VERSION.md](../VERSION.md) | Expanded description and status of the current release or prerelease. |
| [docs/decisions/DECISIONS.md](./decisions/DECISIONS.md) | Durable decisions, rationale, consequences, and links to supporting documents. |
| [CONTRIBUTING.md](./CONTRIBUTING.md) | Rules for maintaining these records and contributing changes. |

Do not create parallel records for the same purpose. Legacy duplicates should point contributors to the canonical document and must not maintain a second copy of its content.
