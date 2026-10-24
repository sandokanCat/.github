# Version record

## Current release status

- **Prepared version:** 0.1.0-alpha.1
- **Release type:** prerelease (alpha)
- **Publication status:** pending
- **Intended tag target:** [48aa0d7082d75138c856e6b2428f9586d38df83d](https://github.com/sandokanCat/.github/commit/48aa0d7082d75138c856e6b2428f9586d38df83d)
- **Anchor commit date:** 2026-10-24 (UTC commit date)
- **Versioning scheme:** [Semantic Versioning 2.0.0](https://semver.org/spec/v2.0.0.html)

Do not describe this prerelease as published until the Git tag and GitHub prerelease have been created and verified. Once published, replace the pending status with the verified tag and release URLs. The release must remain anchored to the intended commit even if later documentation-only commits are added to main.

## Scope

This prerelease packages the initial reusable AI coding-agent instruction template. Root AGENTS.md is the canonical policy source, with client-specific entry points acting as compatibility adapters. The compatibility matrix documents native, legacy, version-dependent, and provisional support.

## Compatibility and limitations

- Support varies by client, product surface, and version.
- A textual instruction to read another file is not equivalent to a host-level import or guaranteed context injection.
- Validate the effective instruction context in each target client before relying on it.
- Emerging or insufficiently documented integrations remain provisional.

## Release documentation

- [Changelog](./CHANGELOG.md) — concise, release-oriented notable changes.
- [Development summary](./SUMMARY.md) — complete high-level commit log grouped by UTC date and logical type.
- [AI compatibility matrix](./docs/ai/AGENT_ARCHITECTURE.md) — entry-point architecture and compatibility caveats.
- [Release process](./docs/releases/RELEASE_PROCESS.md) — steps to prepare, publish, and verify a release.
- [Tagging conventions](./docs/releases/TAGGING.md) — immutable version anchors.
