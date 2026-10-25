# Decision register

This document records durable project and team decisions, not a file-by-file change history. Entries are ordered by decision date in descending ISO 8601 order. Each entry should capture the decision, its rationale, important consequences, and links to the documents that define or implement it. Do not duplicate detailed policies maintained elsewhere.

## 2026-10-25 — Establish file-placement precedence

**Status:** Accepted

**Decision:** Apply this order when placing files: (1) platform-mandated names and locations, including GitHub Community Health Files and coding-agent discovery entry points; (2) documented industry conventions; (3) repository-specific conventions; and (4) personal organisation preferences only where no higher-priority rule applies. Do not move a file when doing so breaks platform discovery or tooling.

**Rationale:** The repository supports multiple platforms and agent clients. A consistent precedence rule avoids breaking integrations for cosmetic organisation.

**Consequences:** Keep mandatory entry points in their required locations. Move other maintained documentation to the relevant `docs/` category, retain `# Deprecated` markers at legacy paths where useful, and update links in the same change.

## 2026-10-25 — Separate work history, release history, and decisions

**Status:** Accepted

**Decision:** Keep distinct records for distinct purposes:
- [WORK_LOG.md](../development/WORK_LOG.md) is this repository's own documented convention for a complete, high-level commit work log, grouped by UTC date and logical type, with a link for every commit. It is not a universally mandated repository filename or a replacement for Git history.
- [CHANGELOG.md](../../CHANGELOG.md) is a curated record of notable changes by release, following Keep a Changelog.
- [VERSION.md](../releases/VERSION.md) describes the current release or prerelease in more detail.
- This file records durable decisions and their rationale.
- [docs/index.md](../index.md) is the documentation entry point; [CONTRIBUTING.md](../CONTRIBUTING.md) defines how to maintain these records.

**Rationale:** A commit log, a release changelog, a release description, and a decision register answer different questions. Combining them creates duplicated content and makes the release changelog less useful.

**Consequences:** Update only the record whose purpose matches the change. A single change may be summarized in more than one place only when each summary serves a distinct audience and purpose.


## 2026-10-25 — Preserve GitHub's supported accessibility file location

**Status:** Accepted

**Decision:** Keep the default `ACCESSIBILITY.md` at `docs/ACCESSIBILITY.md`. GitHub explicitly lists this as a supported location for a default community health file. Do not move it into a topic-specific subdirectory, even if that would otherwise be tidy.

**Rationale:** Platform discovery requirements take precedence over the repository's preferred documentation taxonomy.

**Consequences:** The documentation index must link to `docs/ACCESSIBILITY.md`; the file may be empty while still a placeholder, but its location must remain compatible with GitHub.
