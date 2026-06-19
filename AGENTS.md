# AGENTS.md

These instructions define how Codex should work inside projects that use Riko AI OS.

## Operating Mode

- Read project context before editing.
- Prefer existing project patterns over new abstractions.
- Make focused changes and verify them.
- Use explicit delegation when specialist agents help.
- Keep secrets out of files, logs, memory, and examples.
- Do not invent API behavior. Use current docs through Context7, official docs, or web search when behavior may have changed.
- Treat high-risk work, security changes, deployment changes, and financial/legal advice as requiring extra verification and user confirmation.

## Delegation

Codex does not automatically spawn every specialist. The parent assistant should choose agents intentionally:

1. Use `agents/orchestrator.md` for multi-stage or ambiguous work.
2. Use `agents/researcher.md` for unknown technologies, vendors, or current facts.
3. Use implementation agents only after scope is clear.
4. Use `agents/code-reviewer.md` before finalizing code changes.
5. Use domain agents for vendor-specific work such as Supabase, Vercel, Avigilon, Peplink, networking, or security systems.

## Default Workflow

1. Clarify objective, constraints, and success criteria.
2. Inspect local files and existing patterns.
3. Plan only as much as needed.
4. Implement in small steps.
5. Run relevant checks.
6. Summarize what changed, what was verified, and what remains.

## Quality Bar

- Every recommendation names assumptions.
- Every implementation has a validation path.
- Every document is actionable for a future operator.
- Every escalation explains risk, impact, and required decision.

## Memory

Use `memory/memory-policy.md`. Store durable facts only when they would help a future agent. Never store credentials, tokens, private keys, passwords, or sensitive personal data.
