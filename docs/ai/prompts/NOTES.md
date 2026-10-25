# Planned prompt directory

**Status:** planned collection; no task-specific prompt files are published yet.

## Purpose

Reserve this directory for maintained, reusable task prompts. This note records the intended use until the first prompt is added; it is not itself a runnable prompt.

## Intended layout

Start with a flat collection:

```text
docs/ai/
├── PROMPTS.md
├── prompts/
│   ├── NOTES.md
│   └── <descriptive-name>.prompt.md
└── templates/
    └── PROMPT.md
```

Use descriptive filenames. Use the `.prompt.md` suffix when targeting VS Code or GitHub Copilot prompt-file conventions, and follow the target product's required discovery path and frontmatter. A file under `docs/ai/prompts/` is a repository catalogue item, not automatically discovered by every agent client.

## When adding a prompt

1. Confirm the task is reusable and has a clear, bounded purpose.
2. Start from [the prompt template](../templates/PROMPT.md).
3. State the intended tool/client, inputs, expected output, constraints, and any validation steps.
4. Add the prompt to the [prompt catalogue](../PROMPTS.md).
5. Check relative links and verify any platform-specific format against official documentation.

Keep the collection flat by default. Give a prompt its own subdirectory only when it needs supporting files or examples; document that structure in the prompt itself.

## Example

`docs/ai/prompts/review-security.prompt.md` could define a repeatable security-review task, specify which files and evidence to inspect, and require findings to include severity, impact, and remediation. This is an illustrative future filename, not a published prompt.

## Maintenance

Update this note if the directory's purpose or layout changes. Do not turn it into a duplicate prompt catalogue; keep prompt entries and status in `PROMPTS.md`.
