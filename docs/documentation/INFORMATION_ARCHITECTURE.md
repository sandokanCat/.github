# Information architecture and file-placement precedence

This repository supports GitHub account-level Community Health Files, coding-agent instruction discovery, developer tools, website metadata, and human-facing documentation. File placement is therefore a compatibility decision, not merely a stylistic choice.

## Mandatory precedence

Apply the following hierarchy in order:

1. **Platform requirements and discovery behaviour.** Keep files at the exact names and locations required by GitHub, coding-agent clients, build tools, browsers, crawlers, and other integrations. Do not move a file if doing so breaks discovery, processing, or a public URL. GitHub Community Health File (CHF) requirements take precedence over all lower levels.
2. **Documented industry conventions.** Where a platform permits several locations, follow the established convention for that file type, such as a root-level `LICENSE`, `README.md`, `CHANGELOG.md`, or `CITATION.cff`.
3. **Repository conventions.** Use the relevant `docs/` topic for maintained explanatory documentation, records, examples, and templates that do not need a platform-defined location.
4. **Personal organisation preferences.** Apply these only when the previous levels do not prescribe a location or impose a compatibility constraint.

If two platform requirements appear to conflict, verify the current official documentation for each affected platform and preserve both entry points when necessary. Do not assume that similarly named files serve the same function.

## Community Health Files

GitHub's official list of supported default Community Health Files includes `ACCESSIBILITY.md`, and its supported locations include the root, `.github/`, and `docs/`. Do not place it under `docs/<topic>/`. See the [official GitHub guidance](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).



This repository is named `.github` and supplies default community health content to eligible repositories owned by the account. Follow GitHub's official [default community health file guidance](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file). For supported file types, GitHub checks `.github/`, the repository root, and then `docs/`; other CHF types have specific locations. Do not relocate CHF files based only on the topic folders used for explanatory documentation.

Operational templates and configuration belong in their platform-defined locations. Explanatory documentation about a template may live under `docs/`, but is not a substitute for the operational file.

Keep the canonical operational `CODEOWNERS` file at `docs/CODEOWNERS`, following the repository's preferred organisational order: `docs/`, `.github/`, then root. Its wildcard assigns the repository to `@sandokanCat`; explicit rules are listed in the same preferred order: `/docs/CODEOWNERS`, `/.github/CODEOWNERS`, `/CODEOWNERS`. This is an organisational choice only. GitHub's technical selection precedence is `.github/CODEOWNERS`, root `CODEOWNERS`, then `docs/CODEOWNERS`, regardless of the order of rules inside the file. Rules inside `docs/CODEOWNERS` cannot stop a higher-priority file from shadowing it. Keep a single operational copy. `CODEOWNERS` alone does not enforce approval or prevent direct changes; configure branch protection or a ruleset requiring code-owner review, and review bypass permissions, if enforcement is needed.

## Coding-agent entry points

Root `AGENTS.md` is the canonical project-wide instruction source. Preserve it and any vendor/client entry points whose names or paths are required for discovery or backward compatibility. See [AGENT_ARCHITECTURE.md](../ai/AGENT_ARCHITECTURE.md). An adapter is not redundant merely because a newer client supports another filename.

## Conventional root files

Keep files in the root when the ecosystem convention or behaviour depends on it, including:

- `README.md`, `LICENSE`, and the repository-wide `CHANGELOG.md`;
- `CITATION.cff`, which GitHub uses for the repository citation interface;
- `AGENTS.md` and supported client-specific instruction/configuration entry points;
- Git configuration files such as `.gitignore`, `.gitattributes`, and `.gitmodules`;
- build-tool configuration files whose documented discovery expects the root;
- website metadata and verification files whose root-relative public paths are meaningful.

A file being empty does not prove that it is safe to move; check whether its name is an integration entry point before changing it.

## Documentation placement

Use topic-specific directories for non-mandatory human-facing material:

- `docs/ai/`: agent instruction architecture, compatibility notes, and skill templates.
- `docs/community/`: authorship, contributors, community participation, and collaboration.
- `docs/development/`: engineering workflow and the chronological commit work log.
- `docs/decisions/`, `docs/adr/`, and `docs/rfcs/`: durable decisions, architectural decisions, and proposals, respectively.
- `docs/legal/`: explanatory legal, citation, licensing, and notice guidance. The actual licence text remains in the root `LICENSE` file.
- `docs/releases/`: version records, release preparation, tagging, checklists, and release notes.
- `docs/documentation/`: documentation architecture, link policy, and maintenance conventions.
- Other `docs/` folders: use the topic that best matches the document's primary purpose.

Do not create duplicate authoritative records. If a file moves, update links and instructions in the same change. When a legacy root path is retained for compatibility, replace its contents with a short `# Deprecated` notice pointing to the canonical location.

## Planned empty directories

When a future directory is needed before its first operational or content file is ready, create a `NOTES.md` inside that directory rather than leaving an undocumented empty folder. Explain the directory's purpose, intended structure, likely file types, examples, platform-specific discovery constraints, and the conditions for adding real content. Clearly mark the directory as planned; do not imply that examples are already implemented. For example, `docs/ai/prompts/NOTES.md` and `docs/ai/skills/NOTES.md` describe planned collections. Link the note from the relevant catalogue or index where appropriate, and update or replace it when real content arrives. Avoid duplicating the full catalogue in `NOTES.md`.

## Reusable templates and configuration examples

Reusable examples that have no platform-defined root location belong under docs/<topic>/templates/, grouped by the domain they configure. For example, site-verification settings belong under docs/identity/templates/. Do not introduce or retain a generic root-level config.ini simply because a project-specific configuration format may be invented later. Keep root configuration files only when the relevant platform, tool, or established convention requires that exact path. When moving a template, update the index and every reference in the same change; delete an obsolete root stub when it has no compatibility purpose.

## Git ignore and archive caveats

A `.gitignore` rule prevents matching untracked files from being added by ordinary Git operations; it does not remove files already tracked. Renaming a tracked directory to an ignored path still leaves its files in Git history and in the current repository tree. A directory rename also does not, by itself, guarantee that Dependabot or another scanner will ignore its contents. Validate the relevant tool configuration separately.

The `_root/` directory is an archival copy of external project examples retained temporarily for personal reference. It is not part of this repository's active application, build, or instruction source. It may be removed once those examples are no longer needed.

## References

- GitHub: [Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- GitHub: [About citation files](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files)
- GitHub: [About code owners](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners)
- GitHub: [Dependabot options reference](https://docs.github.com/en/code-security/reference/supply-chain-security/dependabot-options-reference)
