# Development summary

This file is the repository's chronological work log. It summarizes work by UTC date and logical change type; each entry links to its authoritative Git commit. It intentionally avoids duplicating diffs, author metadata, or detailed implementation records. Git history remains the source of truth for those details.

## Convention

- Group entries by commit author date in UTC (YYYY-MM-DD), newest first.
- Within each date, group commits by logical change type; each group starts with a short, high-level summary of that day's work in that area.
- Within each group, list commits newest first, using 24-hour UTC time (HH:mm:ss UTC). Every commit entry links to GitHub's commit view.
- Use concise, neutral descriptions rather than copying commit subjects or enumerating file-level changes. The link provides the full traceable record.
- Add entries for all commits, including maintenance and merge commits. Do not use this file as a substitute for [CHANGELOG.md](./CHANGELOG.md), which records notable changes by release, or [the decision register](./docs/decisions/DECISIONS.md), which records durable decisions.
- See [CONTRIBUTING.md](./docs/CONTRIBUTING.md) for maintenance rules and [docs/index.md](./docs/index.md) for the documentation entry point.

## 2026-10-24 (UTC)

### Documentation and release governance

Separated the repository's work log, release-facing history, version record, and durable decisions. The documentation catalog and its navigation were then consolidated and refined.

#### [23:14:57 UTC — Clarify community health file precedence and release metadata](https://github.com/sandokanCat/.github/commit/37d7687f8f4f4e035a6e886d83dd8fcaa2249c04)

#### [23:14:04 UTC — Record documentation work and keep prerelease status accurate](https://github.com/sandokanCat/.github/commit/7cae576b9d8fa977328270166cffd9fefd6a1a5b)

Separated the repository's work log, release-facing history, version record, and durable decisions. The documentation catalog and its navigation were then consolidated and refined.

#### [23:13:36 UTC — Correct catalog links relative to docs index](https://github.com/sandokanCat/.github/commit/b1f92a5059737809760f61fdf5ac75cf4d1e5b2d)

#### [23:13:19 UTC — Migrate and translate the full documentation catalog](https://github.com/sandokanCat/.github/commit/f5f10908b0ab05f236ac8518ee8345dd45ccb2e7)

#### [23:11:36 UTC — Separate work log, changelog, and release records](https://github.com/sandokanCat/.github/commit/381002e8abe47c2ad4d5e8d7b89689c4eb3796e3)

### AI instruction architecture

Established and extended a canonical instruction model with compatibility entry points for different agent products and generations. Compatibility remains client- and version-dependent.

#### [21:15:14 UTC — Cover nested and legacy AI instruction entry points](https://github.com/sandokanCat/.github/commit/48aa0d7082d75138c856e6b2428f9586d38df83d)

#### [21:14:42 UTC — Extend AI compatibility matrix and legacy adapters](https://github.com/sandokanCat/.github/commit/ea126d034d8ffd509f80f78423d05ffc70fb6dce)

#### [21:13:50 UTC — Add historical AI instruction compatibility template](https://github.com/sandokanCat/.github/commit/428da38ad7dcc889ef287d90dd2952a33bf357b3)

#### [21:02:27 UTC — Expand AI agent instruction compatibility survey](https://github.com/sandokanCat/.github/commit/fe2ddd77d8542ed3c31cd9a55ebf8ff54b1d6238)

#### [20:42:31 UTC — Unify AI coding instructions around AGENTS.md](https://github.com/sandokanCat/.github/commit/c994341caa160a9dfc3c428612d7da10a232c39b)

#### [19:56:15 UTC — Crear .claude/settings.json](https://github.com/sandokanCat/.github/commit/2f543bba0f7fe96ee130b46f7d58cef213cad712)

#### [19:54:50 UTC — Crear .aider.conf.yml](https://github.com/sandokanCat/.github/commit/8c2a88ead7a26ec804b3ea5b0f86783ada594930)

#### [19:51:25 UTC — Crear .config/opencode/AGENTS.md](https://github.com/sandokanCat/.github/commit/72f375b05c255c49adca5e1a0a477ac4f0324dcd)

#### [18:57:10 UTC — Actualizar copilot-instructions.md](https://github.com/sandokanCat/.github/commit/5e81cbf1ae6cccc2070ac8312bb772acc0070801)

#### [18:54:24 UTC — Crear .gemini/settings.json](https://github.com/sandokanCat/.github/commit/ebac9c8d77af3999929ae328d94072b42cc4cb15)

#### [18:51:26 UTC — Add reference to AGENTS.md in CLAUDE.md](https://github.com/sandokanCat/.github/commit/f7ed3f6b3bb4464d348878d55d9beec9f7a0de0d)

### Documentation and information architecture

Organized documentation entry points and repository-level reference material.

#### [10:06:09 UTC — Initialize changelog from repository history](https://github.com/sandokanCat/.github/commit/7cbc16e2ef723f3c592bdee4c4cc78e94b367c7f)

### Repository configuration and metadata

Maintained shared repository configuration and descriptive metadata.

#### [19:43:58 UTC — # example CITATION.cff](https://github.com/sandokanCat/.github/commit/c9eb55c5539aebc76eebbacd7048a2ea727bdc69)

#### [19:40:19 UTC — Crear config.ini](https://github.com/sandokanCat/.github/commit/d3c125ed4ac9babc8e9af5eb5f3c6ed74be531b5)

#### [19:28:15 UTC — Actualizar .gitignore](https://github.com/sandokanCat/.github/commit/7d2fb645ded92b293a8900795cda41b66f1b5edc)

#### [19:24:47 UTC — # example .gitmodules](https://github.com/sandokanCat/.github/commit/a7e516be6706b943496bbabce88534a127dd2c5a)

#### [19:10:57 UTC — Actualizar .gitattributes](https://github.com/sandokanCat/.github/commit/11337cb315a1aaf164a917091c976095abcd8b7f)

#### [19:06:43 UTC — Actualizar settings.json](https://github.com/sandokanCat/.github/commit/d5708aaeee910d687bf81b5b085e5968dd5cfbdc)

### Site metadata and discoverability

Maintained metadata used for site discovery, indexing, and machine-readable repository information.

#### [19:29:57 UTC — Actualizar site.webmanifest](https://github.com/sandokanCat/.github/commit/4bee7f733af6c7bfcdcf8433d671cf1b29db5ca1)

#### [19:13:24 UTC — Actualizar humans.txt](https://github.com/sandokanCat/.github/commit/35affa08b100ebf4db6964cf06616c7e216a0086)

#### [18:53:28 UTC — Actualizar humans.txt](https://github.com/sandokanCat/.github/commit/76af75ba246cf4187f4dbe89e20a1a60ecc0b97d)

#### [18:49:21 UTC — Add robots.txt with sitemap entries](https://github.com/sandokanCat/.github/commit/e06ef812d8c9803edfd263b423ae395f1e1c2d59)

### Licensing and project metadata

Maintained licensing and related project metadata.

#### [19:15:24 UTC — Actualizar LICENSE](https://github.com/sandokanCat/.github/commit/141228ae6024e15683f6a0fb2d829564020dd11f)

### Dependency maintenance

Applied or integrated automated dependency maintenance across auxiliary projects.

#### [19:16:40 UTC — Merge pull request #6 from…](https://github.com/sandokanCat/.github/commit/1a0b6704be29c3570c11f4f978f2265cd0f4e49a)

#### [19:16:26 UTC — Merge pull request #5 from sandokanCat/dependabot/uv/root/rendercv/uv-624cda2b71](https://github.com/sandokanCat/.github/commit/00398d3c30f81b32255ab643238cf72d366d5d20)

#### [11:07:59 UTC — Bump the npm_and_yarn group across 1 directory with 3 updates](https://github.com/sandokanCat/.github/commit/7a7e2e22ed75499e0939308a726084b93356544e)

#### [11:05:47 UTC — Bump the uv group across 1 directory with 3 updates](https://github.com/sandokanCat/.github/commit/26b64470d1b6ba649494be93ed3dc146959b6c0a)

#### [10:09:21 UTC — Merge pull request #3 from sandokanCat/dependabot/uv/root/rendercv/uv-bbf36862e1](https://github.com/sandokanCat/.github/commit/4ddc9a7250026cb0ade91f4e248bd265248544b4)

## 2026-10-23 (UTC)

### Dependency maintenance

Applied or integrated automated dependency maintenance across auxiliary projects.

#### [23:00:47 UTC — Bump pillow](https://github.com/sandokanCat/.github/commit/a72600a9c3e6a2516d983e5523ba22bdb544f3fd)

## 2026-10-22 (UTC)

### Site metadata and discoverability

Maintained metadata used for site discovery, indexing, and machine-readable repository information.

#### [07:20:23 UTC — Crear manifest.json](https://github.com/sandokanCat/.github/commit/97782bba9b6d0fb1061b1c3592eb8a9fc9a0c86e)

## 2026-10-21 (UTC)

### Repository configuration and metadata

Maintained shared repository configuration and descriptive metadata.

#### [22:29:23 UTC — Crear tasks.json](https://github.com/sandokanCat/.github/commit/2574b4925cf545bc0e414ae0b047e21931c21cc9)

### Licensing and project metadata

Maintained licensing and related project metadata.

#### [23:46:24 UTC — Crear LICENSE-EXCEPTION](https://github.com/sandokanCat/.github/commit/96f25d886806a9c07b3bbda4d6f3de294423a5e2)

## 2026-10-20 (UTC)

### AI instruction architecture

Established and extended a canonical instruction model with compatibility entry points for different agent products and generations. Compatibility remains client- and version-dependent.

#### [05:16:23 UTC — Add AGENTS.md](https://github.com/sandokanCat/.github/commit/6dc05f8c66b6a18cedd16eb62ab45a29a17f43e8)

#### [05:16:21 UTC — Add GEMINI.md](https://github.com/sandokanCat/.github/commit/989f5b825d75fd80c6efe52b19ae0456994338f5)

#### [05:16:19 UTC — Add CLAUDE.md](https://github.com/sandokanCat/.github/commit/12223ec97fda25963f10515d4e9f91c5f9dc3977)

#### [05:16:17 UTC — Add .github/copilot-instructions.md](https://github.com/sandokanCat/.github/commit/be3481f011cb7a00f5fc0ce62494c3244e0f2f45)

### Documentation and information architecture

Organized documentation entry points and repository-level reference material.

#### [06:14:53 UTC — Include Docusaurus sidebar configuration in catalog](https://github.com/sandokanCat/.github/commit/c681d70828f9a4581fde460f764ed880bf8ba08b)

#### [06:14:22 UTC — Add catalogued documentation placeholders and organize summary](https://github.com/sandokanCat/.github/commit/b85269fdde5506e96e43fc703507fb0e82bc0cbd)

#### [05:34:40 UTC — Organize summary and index all repository files](https://github.com/sandokanCat/.github/commit/a75818a2817defd6e5758e8b01c2f9365d833e4f)

#### [05:16:34 UTC — Add SUMMARY.md](https://github.com/sandokanCat/.github/commit/727d0d46bdd30d65a3638e2d5188f1e6ce83a9ac)

#### [05:16:28 UTC — Add docs/index.md](https://github.com/sandokanCat/.github/commit/fc8165f6d8b5c7860bfce5f306c92946b8a1201c)

### Repository configuration and metadata

Maintained shared repository configuration and descriptive metadata.

#### [10:17:22 UTC — Crear .editorconfig](https://github.com/sandokanCat/.github/commit/318c0484410c63bd8f7b632f6c268d31d558c34c)

#### [05:16:15 UTC — Add CITATION.cff](https://github.com/sandokanCat/.github/commit/408e55b8f0df3d3457e22d200c0f9c175843f419)

### Site metadata and discoverability

Maintained metadata used for site discovery, indexing, and machine-readable repository information.

#### [11:37:58 UTC — Actualizar ror.xml](https://github.com/sandokanCat/.github/commit/bc245508c702840fa9b1fd87614cbd7dc2ea204e)

#### [11:37:38 UTC — Actualizar sitemap.xml](https://github.com/sandokanCat/.github/commit/9d802d36b6d52f282bc5d8a651f56b69c895185c)

#### [11:37:22 UTC — Actualizar sitemap.html](https://github.com/sandokanCat/.github/commit/bfd97c0c317c25aff58b944c6638baad4d1cbf87)

### Community infrastructure

Established or refined reusable community-facing repository resources.

#### [05:34:25 UTC — Add docs/GOVERNANCE.md](https://github.com/sandokanCat/.github/commit/70bd2fbbdf6c3ccfc2a7271588ad5061d19883bf)

#### [05:34:23 UTC — Add .github/DISCUSSION_TEMPLATE/q-a.yml](https://github.com/sandokanCat/.github/commit/0dda5bfc4c89dfc025df4b3eb11cbeab6eab33b9)

#### [05:34:21 UTC — Add .github/DISCUSSION_TEMPLATE/ideas.yml](https://github.com/sandokanCat/.github/commit/5c4d5cb277f58f295bfe12e85dd2affa55aa9cba)

#### [05:34:18 UTC — Add .github/PULL_REQUEST_TEMPLATE.md](https://github.com/sandokanCat/.github/commit/1a1a398215822daa679a5753dcdbe62deed92f29)

#### [05:34:17 UTC — Add .github/ISSUE_TEMPLATE/feature_request.yml](https://github.com/sandokanCat/.github/commit/d50b711e098b08711fc481073e3ca8fd4360a5df)

#### [05:34:15 UTC — Add .github/ISSUE_TEMPLATE/bug_report.yml](https://github.com/sandokanCat/.github/commit/c7ca5207a4e7c8a116e9bee097934ee2baccc841)

#### [05:34:12 UTC — Add .github/ISSUE_TEMPLATE/config.yml](https://github.com/sandokanCat/.github/commit/329b1131ae368a6de8eeb64089a5d41c8959feeb)

#### [05:16:10 UTC — Add docs/SUPPORT.md](https://github.com/sandokanCat/.github/commit/b0433a46916ab861c3aea5b08b70a94df205a9e4)

### Licensing and project metadata

Maintained licensing and related project metadata.

#### [10:34:30 UTC — Add MIT License to the project](https://github.com/sandokanCat/.github/commit/d60ebbdd1344ecb9a8278899416308b23e15e7bf)

### Repository maintenance

Performed general repository setup and maintenance.

#### [11:58:52 UTC — Eliminar DESIGN.md](https://github.com/sandokanCat/.github/commit/e4d4521eb9a3f67b837cdf9134314a249f71c1d5)

#### [11:47:14 UTC — Rename skills directory to badges](https://github.com/sandokanCat/.github/commit/86969126fe0530dfdec2e5358a25a9e1f09be99c)

#### [11:35:22 UTC — Add root-level placeholders mirrored from cv](https://github.com/sandokanCat/.github/commit/c62fd91e4f00df516dc1903851d9e64da544bfa5)

#### [10:28:36 UTC — Crear DESIGN.md](https://github.com/sandokanCat/.github/commit/d9e0d44370ad5fe8ba50186d88561b70200198b5)

#### [05:34:10 UTC — Add .github/VULNERABILITY_REPORT.yml](https://github.com/sandokanCat/.github/commit/41dd7fbc9fcf254335c1e8d7b98ebd8cdd20bdda)

#### [05:34:02 UTC — Add docs/ACCESSIBILITY.md](https://github.com/sandokanCat/.github/commit/3d796a9ac997921a7070692fbb737fefa55925aa)

#### [05:16:32 UTC — Add docusaurus.config.js](https://github.com/sandokanCat/.github/commit/f18a6983ada427bfae2de6beeedfc7d1a8008a3b)

#### [05:16:30 UTC — Add mkdocs.yml](https://github.com/sandokanCat/.github/commit/61438317175734ed7f8c00f7d41971f65a973167)

#### [05:16:25 UTC — Add SKILL.md](https://github.com/sandokanCat/.github/commit/bc656e8041985a2bb099f0337fb0530ff09ad8d9)

#### [05:16:12 UTC — Add docs/CODEOWNERS](https://github.com/sandokanCat/.github/commit/cfdc49763d795f0cd0a4c0a5f044ff259e865260)

#### [05:16:08 UTC — Add docs/CODE_OF_CONDUCT.md](https://github.com/sandokanCat/.github/commit/08d67f707b3b46518370e24ec2303e103cad6cd5)

#### [05:16:06 UTC — Add docs/CONTRIBUTING.md](https://github.com/sandokanCat/.github/commit/0863b8610fc10ae067b1b115b0750d2faebaabdd)

#### [05:16:03 UTC — Add docs/SECURITY.md](https://github.com/sandokanCat/.github/commit/c5ec236f46a76dc925d1b687f961615024e7cdde)

## 2026-10-18 (UTC)

### Community infrastructure

Established or refined reusable community-facing repository resources.

#### [16:01:05 UTC — Create README.md for archived workflows](https://github.com/sandokanCat/.github/commit/f1f8cd815d1c73fb8d827a9b9893aa8c2bdf79fb)

### Community and funding metadata

Maintained community support and funding metadata.

#### [21:21:59 UTC — Actualizar FUNDING.yml](https://github.com/sandokanCat/.github/commit/e629e7ad0aa89d81f0ea40c149532bc191265de2)

#### [21:15:18 UTC — Actualizar FUNDING.yml](https://github.com/sandokanCat/.github/commit/7637eeb86bf7ff435be270abbdb2bb4a6f105d0e)

#### [21:14:16 UTC — Actualizar FUNDING.yml](https://github.com/sandokanCat/.github/commit/e8d5a652fd30a5abe1cda785a84909b76bc40079)

#### [21:12:30 UTC — Actualizar FUNDING.yml](https://github.com/sandokanCat/.github/commit/dd186e284deec93826b378084ad3b999a28c6eac)

### Dependency maintenance

Applied or integrated automated dependency maintenance across auxiliary projects.

#### [16:24:56 UTC — Merge pull request #2 from…](https://github.com/sandokanCat/.github/commit/bdf2dca689704d56261271d2f43cf5a27538f54d)

#### [13:17:20 UTC — Bump axios](https://github.com/sandokanCat/.github/commit/8cc8a70c127301000a8d9749975854ec81bcbf1a)

#### [13:14:03 UTC — Merge pull request #1 from sandokanCat/dependabot/uv/root/rendercv/uv-c6f3ecd35a](https://github.com/sandokanCat/.github/commit/f24601004ebc6124ab8c701bc719a74a3db0d36f)

#### [12:51:23 UTC — Bump the uv group across 1 directory with 11 updates](https://github.com/sandokanCat/.github/commit/5b977f9b7ac7814da86de03265daad5f4ca24c89)

### Repository maintenance

Performed general repository setup and maintenance.

#### [15:59:10 UTC — Add workflow to sync with upstream repository](https://github.com/sandokanCat/.github/commit/cfc3d33a176925ba356001086cbcc12b4c0a6cd2)

#### [12:46:08 UTC — Copy auxiliary files from rendercv and github-stats-extended](https://github.com/sandokanCat/.github/commit/705f85cd558b262d070c8c385815ef77a8792d4d)

#### [11:49:34 UTC — Consolidate shared VS Code configuration](https://github.com/sandokanCat/.github/commit/df6203477c9d0b19e35de6ab9472306b8989b852)

#### [11:36:27 UTC — Move skills and VS Code configuration into shared repository](https://github.com/sandokanCat/.github/commit/0e20cd6774e312305211b1cd3aa3e596ea8370df)

## 2026-10-11 (UTC)

### Community and funding metadata

Maintained community support and funding metadata.

#### [17:57:27 UTC — Change Patreon username to sandokanLair](https://github.com/sandokanCat/.github/commit/23cd26fe5d67e9f107cfedfa80fe54e73be77979)

## 2026-10-05 (UTC)

### Community infrastructure

Established or refined reusable community-facing repository resources.

#### [16:37:13 UTC — Initialize README with community health information](https://github.com/sandokanCat/.github/commit/f720acfd2b25c7a90df8698104e1ba2e99a768a3)

### Community and funding metadata

Maintained community support and funding metadata.

#### [16:26:27 UTC — Remove root FUNDING.yml after moving it](https://github.com/sandokanCat/.github/commit/038d5b204ca4b958b0b13f7ae3e784be8b16bcdf)

#### [16:26:11 UTC — Move FUNDING.yml to .github directory](https://github.com/sandokanCat/.github/commit/6556990c2b31504a90f7576b9eccbfe5cfc565d0)

#### [16:13:03 UTC — Add default FUNDING configuration](https://github.com/sandokanCat/.github/commit/752a3377673a3862b62479c5e96db23f383bcb9d)
