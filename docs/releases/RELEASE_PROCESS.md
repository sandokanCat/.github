# Release process

This document defines the minimal release workflow for this repository. See [tagging conventions](./TAGGING.md), the [release checklist](./RELEASE_CHECKLIST.md), [CHANGELOG.md](../../CHANGELOG.md), and [VERSION.md](./VERSION.md).

## 1. Prepare the release

1. Decide the version using [Semantic Versioning 2.0.0](https://semver.org/spec/v2.0.0.html). Use a prerelease identifier such as -alpha.1 while compatibility or scope remains preliminary.
2. Confirm the intended release commit and inspect its complete diff. The tag must point to that exact commit.
3. Update CHANGELOG.md with only notable user-facing changes. Keep [Unreleased] at the top. A prepared version section may omit its date while publication is pending; add the actual publication date to the version heading after the GitHub Release is published.
4. Update [VERSION.md](./VERSION.md) with the intended version, scope, limitations, and status. Do not claim publication yet.
5. Verify links, syntax, and the release scope. Follow the [release checklist](./RELEASE_CHECKLIST.md).

If the available GitHub integration cannot create tags or releases, complete these steps through GitHub's release interface. Documentation preparation alone does not constitute publication.

## 2. Create the immutable tag and GitHub release

1. Create the tag using the exact name specified in the release plan, pointing at the intended commit.
2. Create a GitHub Release from that tag and mark it as a prerelease when the version contains a prerelease identifier.
3. Use concise release notes derived from CHANGELOG.md; do not paste the full commit log.
4. Verify that the tag resolves to the intended commit and the GitHub Release shows the expected tag and prerelease status.

Official references: [About releases](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases), [Managing releases in a repository](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository), and [Git references REST API](https://docs.github.com/en/rest/git/refs).

## 3. After publication

1. Update VERSION.md to reflect the verified published state and link to the release.
2. Keep follow-up documentation changes on the default branch without moving the published tag.
3. Add new work to [WORK_LOG.md](../development/WORK_LOG.md) as commits land. Add changes to CHANGELOG.md only when they are notable for a future release.
4. When preparing the next release, move the accumulated [Unreleased] entries into a new version section and leave a fresh [Unreleased] section at the top.


## 4. Verify archival and DOI metadata (when Zenodo integration is enabled)

1. After publishing the GitHub Release, check the repository status in [Zenodo GitHub integration](https://zenodo.org/account/settings/github/) and wait for the release record to appear. Zenodo only archives public GitHub repositories through this integration.
2. Open the resulting Zenodo record and verify that its version matches the GitHub tag. Copy the version-specific DOI and the concept DOI from the record itself; never construct or guess a DOI.
3. Add the verified version-specific DOI to the root `CITATION.cff` while its version metadata describes that release. Document the concept DOI separately if a stable project-wide citation link is useful.
4. If no record appears, verify that the repository toggle is enabled and that the GitHub Release is public. Do not create another GitHub release solely to retry; first diagnose the integration status.
5. Before treating the archived project as reusable software, ensure the root `LICENSE` contains the intended licence text. A DOI provides persistence and citation metadata, not a licence grant.

Zenodo assigns a DOI to each archived release and a concept DOI for the record across versions. See [GitHub's citation and Zenodo guidance](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content) and [Zenodo DOI versioning](https://zenodo.org/help/versioning).
