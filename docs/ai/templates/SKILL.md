# Agent skill template

This is a documentation template, not an active skill. Do not place it inside the discoverable `skills/` collection or claim that an agent can load it directly from this location.

For a real skill, create `docs/ai/skills/<skill-name>/SKILL.md`, ensure the directory name matches the skill's `name` metadata, and add the skill to [SKILLS.md](../SKILLS.md). Check the target agent's supported discovery location before copying or publishing it.

## Required metadata

Start a real skill with YAML frontmatter. The open Agent Skills specification requires `name` and `description`; follow its current naming constraints and any target-platform requirements.

```yaml
---
name: example-skill
description: Describe what the skill does and when an agent should use it.
---
```

## Instructions

Write the actual reusable workflow here. Include clear steps, constraints, expected outcomes, and relevant safety boundaries. Keep the main instructions concise; place substantial supporting material in separate files within the skill directory and link to them.

## Supporting resources

Add only resources that the skill genuinely needs, such as `references/`, `scripts/`, or examples. Do not create empty subdirectories speculatively.

## Validation and maintenance

Describe how to verify the skill's output and note platform/version assumptions. Check that the skill's directory name matches its metadata and validate the final file against the current Agent Skills specification.
