# Code ownership

The operational ownership rules are maintained in [`docs/CODEOWNERS`](../CODEOWNERS). That file assigns `@sandokanCat` as the default owner for repository paths and explicitly lists the supported CODEOWNERS locations.

## What CODEOWNERS does

GitHub uses CODEOWNERS rules to identify people or teams responsible for paths and can request their review on pull requests. GitHub checks supported locations in technical priority order (`.github/`, root, then `docs/`). Because this repository keeps its canonical copy in `docs/`, a higher-priority CODEOWNERS file would shadow it, and rules in `docs/CODEOWNERS` cannot prevent that. This is a file-specific exception to the general placement rule in [INFORMATION_ARCHITECTURE.md](../documentation/INFORMATION_ARCHITECTURE.md).

## What CODEOWNERS does not do

A CODEOWNERS entry does not, by itself, prohibit edits, require an approval before merging, or prevent direct pushes. To enforce review, configure branch protection or a repository ruleset that requires code-owner approval. Review who can bypass those rules as well.

## Future team growth

Add path-specific ownership rules when maintainers join the project. Keep the global wildcard as the fallback owner unless the repository's governance model changes. Prefer GitHub usernames or team handles that exist and have appropriate repository access.
