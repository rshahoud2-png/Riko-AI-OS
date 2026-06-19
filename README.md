# Riko AI OS

Riko AI OS is my personal Codex operating system. It gives Codex a clean set of agents, skills, workflows, prompts, and memory rules for personal projects across software, AI apps, business automation, research, deployment, career work, event planning, finance planning, and productivity.

This repository is personal only. It is not optimized for Claude, TWG work, client delivery, or customer data workflows.

## What This Helps With

- Full-stack app development.
- AI app building.
- GitHub automation and repository maintenance.
- Vercel deployment and troubleshooting.
- Supabase setup and database design.
- API integrations.
- Business automation.
- Research and decision support.
- Resume and job applications.
- Lifestyle entertainment projects.
- Event planning and event business ideas.
- Financial planning support.
- Personal productivity systems.

## Structure

```text
Riko-AI-OS/
├── README.md
├── AGENTS.md
├── .gitignore
├── agents/
├── skills/
├── workflows/
├── prompts/
├── memory/
├── docs/
└── optional/
    └── claude/
```

## How Codex Should Use This Repo

1. Load `AGENTS.md` as the main control file.
2. Use `agents/orchestrator.md` for multi-step requests.
3. Pick focused agents from `agents/` only when they clearly help.
4. Use `skills/` as reusable methods for coding, research, automation, deployment, and planning.
5. Use `workflows/` for repeatable project flow.
6. Use `memory/` only for safe, durable personal/project facts.

## Safety Rules

Do not store or commit:

- TWG client data.
- Work credentials.
- Secrets, tokens, passwords, private keys, or API keys.
- Medical records.
- Customer private data.
- Fake API keys or fake credentials.
- Copyrighted source content from external repositories.

Patterns in this repo are adapted and simplified from public agent/skill conventions. No external repo content should be copied directly.

## Optional Claude Support

Claude support is not part of the main operating system. Optional notes live in `optional/claude/optional-claude-setup.md` only.
