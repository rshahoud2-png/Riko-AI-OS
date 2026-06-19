# How To Add New Agents

Add a new agent only when a recurring personal Codex need is not already covered.

Create one markdown file in `agents/` using kebab-case, for example `agents/travel-planner.md`.

## Required Sections

- `Role`
- `When To Use`
- `Inputs Needed`
- `Process`
- `Output Format`
- `Quality Checklist`
- `Escalation Rules`

## Design Rules

- Keep the agent narrow and practical.
- Make it personal-use friendly.
- Avoid TWG/client/vendor-specific assumptions unless intentionally added later.
- Include privacy and approval boundaries.
- Do not include secrets, credentials, customer data, medical records, or fake API keys.
- Do not copy external agent files.

## Before Adding

Ask:

1. Is this different from an existing agent?
2. Will I use it more than once?
3. Is a skill enough instead of a new agent?
4. Does it keep the system simpler?

## Template

```markdown
# Agent Name

## Role

## When To Use

## Inputs Needed

## Process

## Output Format

## Quality Checklist

## Escalation Rules
```
