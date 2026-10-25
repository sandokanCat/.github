# Reusable prompt template

Use this template for a standalone, reusable prompt. Keep the filename descriptive and use the `.prompt.md` suffix when targeting VS Code or GitHub Copilot prompt-file conventions (for example, `review-code.prompt.md`). Store catalogue entries under `docs/ai/prompts/` and add each maintained prompt to [PROMPTS.md](../PROMPTS.md).

## Purpose

Describe the task this prompt performs and when it should be used.

## Required context and inputs

List source material, variables, permissions, tools, and prerequisites the caller must provide. Do not assume access to files or services that have not been supplied.

## Prompt

Replace this note with the complete reusable prompt. State a role only when useful; define the task and scope, specify constraints, and describe the expected output. Do not duplicate repository-wide policy from the root `AGENTS.md`.

## Expected output

Describe the output format and acceptance criteria.

## Validation

List checks the caller should perform before relying on the result.

## Maintenance notes

Record relevant platform/version assumptions and authoritative references. Revalidate them when the target tool changes.
