# Documentation architecture

## Authoritative entry points

- [index.md](../index.md) is the catalog and navigation entry point.
- [AGENTS.md](../../AGENTS.md) is the canonical project-wide coding-agent instruction source; platform-required adapters remain at their discovery paths.
- [CONTRIBUTING.md](../CONTRIBUTING.md) defines the contribution and documentation-maintenance workflow.
- [INFORMATION_ARCHITECTURE.md](./INFORMATION_ARCHITECTURE.md) defines the precedence used when deciding where a file belongs.
- [WORK_LOG.md](../development/WORK_LOG.md) records commit activity.
- [CHANGELOG.md](../../CHANGELOG.md) records notable changes by release.
- [VERSION.md](../releases/VERSION.md) records current and prepared release status.
- [DECISIONS.md](../decisions/DECISIONS.md) records durable decisions and their rationale.

## Record responsibilities

Keep the following records separate because they answer different questions:

| Record | Purpose | Do not use it for |
| --- | --- | --- |
| `WORK_LOG.md` | High-level, chronological work log with one link per commit, grouped by UTC date and logical type | Release notes or decision rationale |
| `CHANGELOG.md` | Curated, user-facing changes by version | A full commit-by-commit history |
| `VERSION.md` | Scope, status, compatibility, limitations, and target commit for a release | A list of every repository change |
| `DECISIONS.md` | Accepted decisions, rationale, and consequences | File-by-file history or an operational task list |
| Issue/task/plan records | Actionable work, owners, status, and acceptance criteria where a real tracking workflow exists | Durable architectural rationale |

Do not invent a task-management system merely because empty template filenames exist. Introduce practical task records only when there is a real workflow and a clear owner for keeping them current.

## Link policy

- Use the destination file's basename as the link text where that is unambiguous; explain its purpose in the surrounding prose.
- Prefer direct links to canonical files over chains of unnecessary index pages.
- Resolve relative paths from the source document's directory.
- Keep external convention links pointed to the official English-language source where available.
- Verify all links affected by a move, including links in instructions, release records, and archived examples.
- A `# Deprecated` marker should point directly to the replacement and must not retain stale policy.

## Empty placeholders

The repository contains empty documentation placeholders. A listed path is not an active policy until it has useful content. Do not infer requirements from empty files, and do not populate them merely to make the catalog look complete. Keep the index honest about which documents are implemented and which are planned.

## Planned empty directories

Do not leave a required future directory unexplained. Add a `NOTES.md` within it to record purpose, expected structure, examples, constraints, and next steps. Mark planned content as planned, and keep the note aligned with the relevant catalogue. Remove or revise the planning note when the directory becomes active; do not let it become a duplicate index.

## File-placement precedence

Follow [INFORMATION_ARCHITECTURE.md](./INFORMATION_ARCHITECTURE.md) for the single authoritative file-placement rule and its exceptions. Do not restate that policy here.
