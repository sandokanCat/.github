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

## Next prepared prerelease

- **Prepared version:** 0.1.0-alpha.2
- **Publication status:** blocked pending verification of v0.1.0-alpha.1
- **Intended tag target:** `PENDING_FINAL_PREPARATION_COMMIT_SHA`
- **Scope:** documentation architecture, file placement, archive-directory rename, and reference updates.

Replace the target SHA placeholder in a follow-up documentation commit after the substantive preparation commit exists. Do not publish alpha.2 before alpha.1 is published and verified.

## Release documentation

- [CHANGELOG.md](../../CHANGELOG.md) — concise, release-oriented notable changes.
- [WORK_LOG.md](../development/WORK_LOG.md) — complete high-level commit log grouped by UTC date and logical type.
- [AGENT_ARCHITECTURE.md](../ai/AGENT_ARCHITECTURE.md) — entry-point architecture and compatibility caveats.
- [RELEASE_PROCESS.md](./RELEASE_PROCESS.md) — steps to prepare, publish, and verify a release.
- [TAGGING.md](./TAGGING.md) — immutable version anchors.
