# How To Add New Agents

Create one markdown file in `agents/` using kebab-case, for example `agents/payroll-advisor.md`.

## Required Sections

- `Role`
- `When To Use`
- `Inputs Needed`
- `Process`
- `Output Format`
- `Quality Checklist`
- `Escalation Rules`

## Design Rules

- Keep the agent narrow enough to be useful.
- State when not to use it if confusion is likely.
- Include approval boundaries.
- Avoid vendor claims unless verified.
- Do not include secrets, credentials, or private examples.

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
