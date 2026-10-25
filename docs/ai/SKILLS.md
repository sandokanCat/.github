# Agent skills catalogue

This file indexes maintained agent skills documented in this repository. A catalogue entry is not itself a runnable skill, and a file's presence under `docs/ai/` does not guarantee discovery by any particular agent client.

## Format and location

Use the open [Agent Skills specification](https://agentskills.io/specification) for portable skills. Each skill is a directory containing a `SKILL.md` file with YAML frontmatter; at minimum, the `name` and `description` fields are required. The directory name must match the skill name. Supporting files may be included when needed.

Repository reference layout:

```text
docs/ai/skills/<skill-name>/SKILL.md
```

This is the repository's catalogue layout, not a universal discovery path. Copy or install skills to the location supported by the target agent, and check the target's official documentation before claiming automatic discovery.

## Available skills

No task-specific skills have been published yet.

## Template

- [Agent skill template](./templates/SKILL.md) — a reference template, not an active skill.
