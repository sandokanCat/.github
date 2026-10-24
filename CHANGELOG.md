# Changelog

All notable changes to this project are documented in this file.

This file follows [Keep a Changelog 2.0.0](https://keepachangelog.com/en/2.0.0/) and uses [Semantic Versioning 2.0.0](https://semver.org/spec/v2.0.0.html). It records notable release changes, not individual commits. For day-to-day activity, see [SUMMARY.md](./SUMMARY.md); for the expanded release record, see [VERSION.md](./VERSION.md).

## [Unreleased]

## [0.1.0-alpha.1]

Prepared prerelease; publication is pending. Once the GitHub prerelease is published, add its publication date to this heading. This version is anchored to commit [48aa0d7082d75138c856e6b2428f9586d38df83d](https://github.com/sandokanCat/.github/commit/48aa0d7082d75138c856e6b2428f9586d38df83d).

### Added

- Prepared a broad set of native and legacy instruction entry points for coding-agent clients, alongside a compatibility matrix covering different products, interfaces, and generations.

### Changed

- Established root AGENTS.md as the canonical policy document; vendor- and client-specific entry points are compatibility adapters rather than independent policy copies.
- Documented that support depends on the client, product surface, version, and actual context-loading behavior. Textual pointers do not guarantee that a host resolves or injects the referenced instructions.

### Known limitations

- Compatibility is not universal or guaranteed. Some reported or emerging integrations remain provisional, and every target client must be checked against its official documentation and tested for effective instruction loading.

[Unreleased]: https://github.com/sandokanCat/.github/compare/v0.1.0-alpha.1...HEAD
[0.1.0-alpha.1]: https://github.com/sandokanCat/.github/releases/tag/v0.1.0-alpha.1
