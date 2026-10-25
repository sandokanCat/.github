# Planned skills directory

**Status:** planned collection; no task-specific skills are published yet.

## Purpose

Reserve this directory for maintained, reusable agent skills. This note describes the intended structure until the first skill is added; it is not an active skill and must not be presented as one.

## Intended layout

```text
docs/ai/
├── SKILLS.md
├── skills/
│   ├── NOTES.md
│   └── <skill-name>/
│       ├── SKILL.md
│       └── <optional-supporting-files>
└── templates/
    └── SKILL.md
```

Each skill lives in its own directory and has a `SKILL.md` with YAML frontmatter. Follow the [Agent Skills specification](https://agentskills.io/specification), including the required `name` and `description` metadata; the directory name must match the skill name. Add supporting files only when the skill needs them.

The layout under `docs/ai/skills/` is the repository's catalogue layout, not a universal discovery path. Check the target agent's official documentation before claiming that a skill will be discovered automatically; install or copy it to the supported location when needed.

## When adding a skill

1. Confirm the workflow is reusable and has a clear purpose.
2. Start from [the skill template](../templates/SKILL.md).
3. Keep the skill instructions focused; add references or scripts only when they materially help.
4. Add the skill to the [skills catalogue](../SKILLS.md).
5. Validate metadata, directory/name agreement, relative links, and target-client compatibility claims.

## Example

`docs/ai/skills/repository-audit/SKILL.md` could define a repeatable repository audit, with clear inputs, ordered checks, evidence requirements, and an output format. This is an illustrative future path, not a published skill.

## Maintenance

Update this note if the directory's purpose or layout changes. Do not duplicate individual skill descriptions here; maintain their catalogue entries in `SKILLS.md`.
