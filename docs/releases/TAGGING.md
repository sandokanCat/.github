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

## First planned prerelease

The initial AI-template prerelease is planned as v0.1.0-alpha.1, anchored to [commit 48aa0d7082d75138c856e6b2428f9586d38df83d](https://github.com/sandokanCat/.github/commit/48aa0d7082d75138c856e6b2428f9586d38df83d). Publication remains pending until the tag and GitHub Release are created and verified. The follow-up v0.1.0-alpha.2 is reserved for the documentation and repository-layout work; do not publish it before alpha.1 is verified. Its target SHA must be filled in after the substantive preparation commit exists. See the [release process](./RELEASE_PROCESS.md).
