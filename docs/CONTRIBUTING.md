# Contributing

This repository provides reusable GitHub community-health files, shared repository configuration, and a compatibility template for coding-agent instructions. Keep changes scoped to the requested concern and preserve the canonical-source model described in [AGENTS.md](../AGENTS.md) and the [AI instruction architecture](./ai/AGENT_ARCHITECTURE.md).

## Before changing files

1. Read AGENTS.md, this guide, and the relevant populated documents linked from the [documentation index](./index.md).
2. Inspect the current tree, relevant file contents, and Git diff. Do not assume that a placeholder filename represents an active policy.
3. Prefer official primary documentation for external tool behavior. Clearly distinguish documented support from version-dependent, reported, or unverified behavior.
4. Keep the change minimal and avoid unrelated files. Do not duplicate policies that already have a canonical source.

## GitHub community health files

GitHub's default community health file (CHF) discovery rules are authoritative for filenames and locations. For files that support multiple locations, GitHub checks the `.github/` directory first, then the repository root, then `docs/`. Preserve these supported locations; do not move a CHF into a nested documentation directory merely for organizational consistency.

- Keep default contribution guidance in [`docs/CONTRIBUTING.md`](./CONTRIBUTING.md), a GitHub-supported location for a default community health file.
- Keep funding and vulnerability-report configuration under [`.github/`](../.github/), as required by GitHub's CHF rules.
- Keep operational issue and pull request templates in [`.github/ISSUE_TEMPLATE/`](../.github/ISSUE_TEMPLATE/) and [`.github/PULL_REQUEST_TEMPLATE.md`](../.github/PULL_REQUEST_TEMPLATE.md). A documentation page describing a template is not a substitute for the operational template.
- The canonical operational [`CODEOWNERS`](./CODEOWNERS) file is kept under `docs/`, the preferred location for this repository. It assigns `@sandokanCat` as the default owner and explicitly assigns ownership to the three supported CODEOWNERS paths: `/CODEOWNERS`, `/.github/CODEOWNERS`, and `/docs/CODEOWNERS`. GitHub uses only the highest-priority existing CODEOWNERS file (`.github/`, then root, then `docs/`), so these rules do **not** prevent a higher-priority file from shadowing this one. Keep one operational copy and do not add copies elsewhere.
- `CODEOWNERS` assigns ownership and can trigger review requests, but does not by itself block changes or prevent creation of a higher-priority CODEOWNERS file. To enforce review, configure branch protection or a ruleset requiring code-owner approval, and review bypass permissions separately.
- Avoid maintaining duplicate CHF copies. Where GitHub applies location precedence, a higher-priority file can shadow the lower-priority copy.

Official references: [Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file), [Setting guidelines for repository contributors](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors), and [About code owners](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners).

## AI instruction template changes

- Maintain the prompt catalogue in [PROMPTS.md](./ai/PROMPTS.md) and the skills catalogue in [SKILLS.md](./ai/SKILLS.md). Keep their entries distinct from templates, and do not claim automatic discovery for files stored under `docs/ai/`.
- Use `docs/ai/templates/PROMPT.md` as the generic prompt-writing reference and `docs/ai/templates/SKILL.md` as the Agent Skills reference. For target-specific runnable prompt files, follow the target platform's supported extension and discovery path; for portable skills, follow the Agent Skills specification.

- Root AGENTS.md is the single source of truth for project-wide coding-agent policy.
- Vendor/client entry points should be short compatibility adapters. Use a documented native import when supported; otherwise make the limitation explicit and direct the client to the canonical file.
- Never claim that a pointer guarantees host-level context loading. Check product, surface, and version independently.
- When changing compatibility claims, update [docs/ai/AGENT_ARCHITECTURE.md](./ai/AGENT_ARCHITECTURE.md) and [WORK_LOG.md](./development/WORK_LOG.md). Add a [CHANGELOG.md](../CHANGELOG.md) entry only when the change is notable for a planned or published release.
- Record durable decisions and rationale in the [decision register](./decisions/DECISIONS.md), linking to detailed policy documents instead of copying them.

## Documentation record conventions

Follow [INFORMATION_ARCHITECTURE.md](./documentation/INFORMATION_ARCHITECTURE.md): platform requirements take precedence over industry conventions, which take precedence over repository conventions; personal preferences apply only where none of those prescribe a location. Reusable configuration examples and templates belong under docs/<topic>/templates/ unless an ecosystem requires a specific discovery path. **When creating a directory that must remain empty for now, add a `NOTES.md` inside it** explaining its intended purpose, planned architecture, examples, relevant constraints, and the conditions for adding real files. Treat this as a planning note, not as a substitute for the eventual catalogue or operational files. Keep it current as the plan evolves.

Maintain these files according to their distinct purposes:

- [index.md](./index.md): concise entry point to populated, authoritative documentation and key repository records. Keep links valid; do not present empty placeholders as completed guidance.
- [WORK_LOG.md](./development/WORK_LOG.md): all commits, grouped first by UTC date (YYYY-MM-DD), then by logical change type, and then newest to oldest by 24-hour UTC time (HH:mm:ss UTC). Each commit entry must link to its GitHub commit. Include a short group-level summary, but do not copy commit subjects, authors, or file-level diff details into the prose.
- [CHANGELOG.md](../CHANGELOG.md): user-facing, notable changes by version. Follow [Keep a Changelog 2.0.0](https://keepachangelog.com/en/2.0.0/), keep [Unreleased] at the top, use the six standard change types when applicable, and list versions newest first. Do not turn it into a commit log.
- [VERSION.md](./releases/VERSION.md): expanded scope, status, compatibility notes, and links for the current release or prerelease. Never mark a release as published until its tag and GitHub release are verified.
- [docs/decisions/DECISIONS.md](./decisions/DECISIONS.md): durable decisions in descending ISO 8601 date order. Record rationale and consequences, not a chronology of file edits.
- [CHANGES.md](./CHANGES.md): parked legacy filename under review; not an active change log. Use the root [CHANGELOG.md](../CHANGELOG.md) for notable release changes, the work log for commit history, and the decision register for durable decisions.

## Release and tag workflow

Follow the repository's [release process](./releases/RELEASE_PROCESS.md), [tagging conventions](./releases/TAGGING.md), and [release checklist](./releases/RELEASE_CHECKLIST.md). A release tag must point to the intended release commit, not merely to the current branch head. Prepare release documentation before tagging; after tagging, avoid changing the release's scope or moving the tag.

## Validation and review

- Verify Markdown links and relative paths for every changed document.
- Validate JSON, YAML, and other structured files touched by the change with appropriate parsers.
- Review the complete diff for accidental changes, duplicate policy, and unsupported claims.
- Report checks actually run and any limitations. Do not claim that unexecuted client compatibility tests have passed.
