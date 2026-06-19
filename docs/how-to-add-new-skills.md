# How To Add New Skills

Add a new skill only when a repeatable method is missing from personal Codex work.

Create one markdown file in `skills/` using kebab-case, for example `skills/vendor-evaluation.md`.

## Required Sections

- `Purpose`
- `Use When`
- `Inputs`
- `Method`
- `Output`

## Design Rules

- A skill is a repeatable method, not a persona.
- Keep it tool-neutral unless the tool is essential.
- Include verification steps.
- Include privacy boundaries for secrets, medical records, work credentials, and customer data.
- Keep it short enough for Codex to use quickly.
- Do not copy external skill files.

## Before Adding

Ask:

1. Is this a method I will reuse?
2. Does an existing skill already cover it?
3. Would this be better as a workflow or prompt?
4. Does it keep the repo easier to use?

## Template

```markdown
# Skill Name

## Purpose

## Use When

## Inputs

## Method

## Output
```
