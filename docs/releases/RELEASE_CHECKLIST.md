# Release checklist

Use this checklist for every release. See the [release process](./RELEASE_PROCESS.md), [tagging conventions](./TAGGING.md), [CHANGELOG.md](../../CHANGELOG.md), and [VERSION.md](./VERSION.md).

## Before tagging

- [ ] Confirm the version and whether it is a prerelease.
- [ ] Review the exact target commit and its diff.
- [ ] Ensure CHANGELOG.md contains only notable changes for this version and follows [Keep a Changelog 2.0.0](https://keepachangelog.com/en/2.0.0/).
- [ ] Ensure [VERSION.md](./VERSION.md) describes the scope, compatibility, and known limitations without falsely claiming publication.
- [ ] Check changed Markdown links and structured-file syntax.
- [ ] Confirm no unrelated or sensitive content is included.

## After tagging and publishing

- [ ] Verify that the tag points to the intended commit.
- [ ] Verify the GitHub Release tag, title, notes, and prerelease flag.
- [ ] Update [VERSION.md](./VERSION.md) with the verified release URL and published status.
- [ ] Confirm CHANGELOG.md links resolve to the intended tag and comparison.
