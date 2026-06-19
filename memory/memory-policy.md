# Memory Policy

## Purpose

Memory helps future Codex sessions remember safe, durable personal and project context. Most interactions should not create memory.

## Store Only Durable Safe Facts

Good candidates:

- Personal workflow preferences.
- Standing rules for Codex behavior.
- Active personal project names, goals, and durable decisions.
- Tooling choices and environment constraints.
- Long-lived business, career, event, or productivity context.

Do not store:

- TWG client data.
- Work credentials.
- Secrets, passwords, tokens, keys, webhooks, recovery codes, or private certificates.
- Medical records.
- Customer private data.
- One-time command output.
- Temporary errors.
- Sensitive personal details not needed for future work.
- Speculation, guesses, or unverified claims.

## Four Gates

Before storing a memory, ask:

1. Future utility: would a new Codex session benefit later?
2. Novelty: is it new or materially changed?
3. Factuality: is it concrete and actionable?
4. Safety: does it avoid secrets, medical records, customer data, and work credentials?

All four must pass.

## Categories

- `identity`
- `preference`
- `rule`
- `project`
- `configuration`
- `technical`
- `business`
- `career`
- `finance`
- `event`
- `productivity`
- `decision`

## Memory Shape

```yaml
category: project
importance: 0.75
source_date: 2026-06-19
fact: "Riko AI OS is a personal Codex operating system for software, AI apps, automation, research, planning, and productivity."
```

## Review Cadence

Review durable memories monthly or before major project changes. Delete stale or unsafe memories.
