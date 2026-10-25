# Tagging conventions

This repository uses [Semantic Versioning 2.0.0](https://semver.org/spec/v2.0.0.html) for version tags. Tags are immutable release anchors, not aliases for a moving branch.

## Naming

- Stable release: vMAJOR.MINOR.PATCH, for example v1.2.3.
- Prerelease: vMAJOR.MINOR.PATCH-IDENTIFIER, for example v0.1.0-alpha.1.
- Use lowercase prerelease identifiers such as alpha, beta, and rc; use numeric suffixes to distinguish iterations.
- Keep the leading v in Git tags. The version recorded in CHANGELOG.md and [VERSION.md](./VERSION.md) omits that prefix.

## Target and immutability

- Create a release tag only after selecting and reviewing the exact commit to publish.
- Never tag the current branch head by habit; confirm the commit SHA explicitly.
- Never move or force-update a published release tag. If a release is defective, publish a corrected version and document the issue.
- The GitHub Release must use the same tag and indicate prerelease status consistently with the version.
- Documentation commits added after a release tag do not change the contents of that release.

## First prerelease and subsequent work

The initial AI-template prerelease, [v0.1.0-alpha.1](https://github.com/sandokanCat/.github/releases/tag/v0.1.0-alpha.1), was published on 2026-10-25 and its tag is verified against [commit 48aa0d7082d75138c856e6b2428f9586d38df83d](https://github.com/sandokanCat/.github/commit/48aa0d7082d75138c856e6b2428f9586d38df83d). Later documentation changes on main do not alter that release.

The next candidate, v0.1.0-alpha.2, is still in progress. No target commit is approved. Do not create or publish that tag until the scope is complete, the entire diff is audited, and the release checklist passes. In particular, do not modify files under `_root/`. See the [release process](./RELEASE_PROCESS.md).
