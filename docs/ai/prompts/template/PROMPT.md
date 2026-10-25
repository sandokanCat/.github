# Reusable prompt template

Use this structure for a single maintained prompt. Store each prompt in its own directory as `docs/ai/prompts/<slug>/PROMPT.md` and add it to the [prompt catalogue](../../PROMPTS.md).

## Purpose

Describe the task this prompt is intended to perform and when it should be used.

## Required context and inputs

List the source material, variables, permissions, tools, and other prerequisites the caller must provide. Do not assume access to files or services that have not been supplied.

## Prompt

> Replace this note with the complete, reusable prompt. State the role only when useful, define the task and scope, specify constraints, and describe the expected output. Do not duplicate the repository-wide rules in `AGENTS.md`.

## Expected output

Describe the output format and acceptance criteria.

## Validation

List checks the caller should perform before relying on the result.

## Maintenance notes

Record relevant platform/version assumptions and authoritative references. Revalidate them when the target tool changes.
