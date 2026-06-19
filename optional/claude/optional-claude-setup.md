# Optional Claude Setup

This repository is primarily for personal Codex use. Claude support is optional and should not shape the main system.

## When To Use

Use this only if a future project explicitly needs Claude Code alongside Codex.

## Optional Claude Rules

- Treat `AGENTS.md` as the source of truth for the operating system.
- Do not add Claude-specific assumptions to the main root files.
- Keep Claude-only configuration inside `optional/claude/`.
- Keep secrets, work credentials, customer data, and medical records out of prompts, files, logs, and memory.

## Suggested Claude Prompt

```text
Use this repository as a Codex-first personal operating system. Read AGENTS.md first. Use optional Claude notes only when they do not conflict with AGENTS.md.
```
