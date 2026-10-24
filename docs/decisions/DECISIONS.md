# Decision register

This document records durable project and team decisions, not a file-by-file change history. Entries are ordered by decision date in descending ISO 8601 order. Each entry should capture the decision, its rationale, important consequences, and links to the documents that define or implement it. Do not duplicate detailed policies maintained elsewhere.

## 2026-10-25 — Separate work history, release history, and decisions

**Status:** Accepted

**Decision:** Keep distinct records for distinct purposes:
- [SUMMARY.md](../../SUMMARY.md) is the complete, high-level commit work log, grouped by UTC date and logical type, with a link for every commit.
- [CHANGELOG.md](../../CHANGELOG.md) is a curated record of notable changes by release, following Keep a Changelog.
- [VERSION.md](../../VERSION.md) describes the current release or prerelease in more detail.
- This file records durable decisions and their rationale.
- [docs/index.md](../index.md) is the documentation entry point; [CONTRIBUTING.md](../CONTRIBUTING.md) defines how to maintain these records.

**Rationale:** A commit log, a release changelog, a release description, and a decision register answer different questions. Combining them creates duplicated content and makes the release changelog less useful.

**Consequences:** Update only the record whose purpose matches the change. A single change may be summarized in more than one place only when each summary serves a distinct audience and purpose.
