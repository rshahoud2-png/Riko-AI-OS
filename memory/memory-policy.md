# Memory Policy

## Purpose

Memory exists to help future agents serve the user better. Most interactions should not create memory.

## Store Only Durable Facts

Good candidates:

- User preferences and standing rules.
- Project names, goals, and durable architecture decisions.
- Tooling choices and environment constraints.
- Long-lived business context.
- Important relationships or responsibilities.

Do not store:

- Secrets, passwords, tokens, keys, webhooks, recovery codes, or private certificates.
- One-time command output.
- Temporary errors.
- Sensitive personal details not needed for future work.
- Speculation, guesses, or unverified claims.

## Four Gates

Before storing a memory, ask:

1. Future utility: would a new agent benefit later?
2. Novelty: is it new or materially changed?
3. Factuality: is it concrete and actionable?
4. Safety: does it avoid secrets and sensitive data?

All four must pass.

## Categories

- `identity`
- `preference`
- `rule`
- `project`
- `configuration`
- `technical`
- `business`
- `relationship`
- `decision`

## Memory Shape

```yaml
category: project
importance: 0.75
source_date: 2026-06-19
fact: "Riko AI OS is a reusable agent/skill/workflow system for Codex and Claude Code."
```

## Review Cadence

Review durable memories monthly or before major project handoff. Delete stale memories when they no longer help.
