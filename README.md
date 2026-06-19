# Riko AI OS

Riko AI OS is a reusable operating system for AI-assisted work in Codex and Claude Code. It gives each assistant a shared way to choose roles, run workflows, use skills, configure MCP tools, and preserve useful memory without copying outside repositories or storing secrets.

## What Is Included

- `AGENTS.md` for Codex operating rules.
- `CLAUDE.md` for Claude Code operating rules.
- `agents/` specialist role contracts.
- `skills/` reusable task methods.
- `prompts/` delegation and planning prompt templates.
- `workflows/` repeatable research, coding, documentation, and incident flows.
- `mcp/` recommended MCP profiles for Claude Code, Codex, and general assistants.
- `memory/` durable memory policy and schema.
- `docs/` setup and extension guides.

## Core Principles

1. Use the smallest capable agent for the task.
2. Ask for missing inputs only when a reasonable assumption would be risky.
3. Prefer current primary documentation for APIs, frameworks, cloud platforms, and vendor systems.
4. Keep secrets out of prompts, files, logs, screenshots, and memory.
5. Separate facts, assumptions, decisions, and recommendations.
6. Validate work before calling it done.
7. Store only durable, useful memory.

## Quick Start On Windows

```powershell
cd Riko-AI-OS
git init
git add .
git commit -m "Initial Riko AI OS setup"
```

For Claude Code, copy or reference `CLAUDE.md` from projects where you want this operating system active. For Codex, copy or reference `AGENTS.md`.

Optional global install locations:

```powershell
New-Item -ItemType Directory -Force "$HOME\.claude"
Copy-Item .\CLAUDE.md "$HOME\.claude\CLAUDE.md"

New-Item -ItemType Directory -Force "$HOME\.codex"
Copy-Item .\AGENTS.md "$HOME\.codex\AGENTS.md"
```

Project-local setup is safer when a project has its own rules:

```powershell
Copy-Item .\CLAUDE.md C:\path\to\project\CLAUDE.md
Copy-Item .\AGENTS.md C:\path\to\project\AGENTS.md
```

## Using With Claude Code

1. Put `CLAUDE.md` at the root of your project.
2. Ask Claude to use an agent by name, for example: `Use the Software Architect and Code Reviewer agents to plan this change.`
3. Add relevant skill files to the prompt when needed, or tell Claude: `Use the Root Cause Analysis skill.`
4. Configure MCP tools from `mcp/claude-code.md`.
5. Keep project-specific rules below the Riko rules if they are stricter.

## Using With Codex

1. Put `AGENTS.md` at the root of your project.
2. Ask Codex to delegate explicitly, for example: `Use the Researcher agent first, then the Full Stack Developer, then Code Reviewer.`
3. Keep implementation inside the workspace unless the user approves broader access.
4. Use `mcp/codex.md` as the recommended connector profile.
5. Add project-specific build, test, and deployment commands to the project `AGENTS.md`.

## Inspired By

This repository was synthesized after studying:

- `hesreallyhim/awesome-claude-code`
- `VoltAgent/awesome-codex-subagents`
- `Ischca/awesome-agents-md`
- `punkpeye/awesome-mcp-servers`
- `mem0ai/mem0`
- `upstash/context7`
- `ComposioHQ/awesome-codex-skills`
- `milisp/awesome-chatgpt-claude-agents`

The files here are original summaries and operating patterns, not copied source files.
