# Contributing

This repository provides reusable GitHub community-health files, shared repository configuration, and a compatibility template for coding-agent instructions. Keep changes scoped to the requested concern and preserve the canonical-source model described in [AGENTS.md](../AGENTS.md) and the [AI instruction architecture](./ai/AGENT_ARCHITECTURE.md).

## Before changing files

1. Read AGENTS.md, this guide, and the relevant populated documents linked from the [documentation index](./index.md).
2. Inspect the current tree, relevant file contents, and Git diff. Do not assume that a placeholder filename represents an active policy.
3. Prefer official primary documentation for external tool behavior. Clearly distinguish documented support from version-dependent, reported, or unverified behavior.
4. Keep the change minimal and avoid unrelated files. Do not duplicate policies that already have a canonical source.

## AI instruction template changes

- Root AGENTS.md is the single source of truth for project-wide coding-agent policy.
- Vendor/client entry points should be short compatibility adapters. Use a documented native import when supported; otherwise make the limitation explicit and direct the client to the canonical file.
- Never claim that a pointer guarantees host-level context loading. Check product, surface, and version independently.
- When changing compatibility claims, update [docs/ai/AGENT_ARCHITECTURE.md](./ai/AGENT_ARCHITECTURE.md) and [SUMMARY.md](../SUMMARY.md). Add a [CHANGELOG.md](../CHANGELOG.md) entry only when the change is notable for a planned or published release.
- Record durable decisions and rationale in the [decision register](./decisions/DECISIONS.md), linking to detailed policy documents instead of copying them.

## Documentation record conventions

Maintain these files according to their distinct purposes:

- [docs/index.md](./index.md): concise entry point to populated, authoritative documentation and key repository records. Keep links valid; do not present empty placeholders as completed guidance.
- [SUMMARY.md](../SUMMARY.md): all commits, grouped first by UTC date (YYYY-MM-DD), then by logical change type, and then newest to oldest by 24-hour UTC time (HH:mm:ss UTC). Each commit entry must link to its GitHub commit. Include a short group-level summary, but do not copy commit subjects, authors, or file-level diff details into the prose.
- [CHANGELOG.md](../CHANGELOG.md): user-facing, notable changes by version. Follow [Keep a Changelog 2.0.0](https://keepachangelog.com/en/2.0.0/), keep [Unreleased] at the top, use the six standard change types when applicable, and list versions newest first. Do not turn it into a commit log.
- [VERSION.md](../VERSION.md): expanded scope, status, compatibility notes, and links for the current release or prerelease. Never mark a release as published until its tag and GitHub release are verified.
- [docs/decisions/DECISIONS.md](./decisions/DECISIONS.md): durable decisions in descending ISO 8601 date order. Record rationale and consequences, not a chronology of file edits.
- [CHANGES.md](../CHANGES.md): deprecated; do not add content. Use the decision register instead.

## Release and tag workflow

Follow the repository's [release process](./releases/RELEASE_PROCESS.md), [tagging conventions](./releases/TAGGING.md), and [release checklist](./releases/RELEASE_CHECKLIST.md). A release tag must point to the intended release commit, not merely to the current branch head. Prepare release documentation before tagging; after tagging, avoid changing the release's scope or moving the tag.

## Validation and review

- Verify Markdown links and relative paths for every changed document.
- Validate JSON, YAML, and other structured files touched by the change with appropriate parsers.
- Review the complete diff for accidental changes, duplicate policy, and unsupported claims.
- Report checks actually run and any limitations. Do not claim that unexecuted client compatibility tests have passed.
