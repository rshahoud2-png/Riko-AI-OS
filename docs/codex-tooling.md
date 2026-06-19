# Codex Tooling

This repo is designed for personal Codex use. Configure only the tools needed for the project at hand.

## Recommended Tools

- GitHub plugin for repository files, issues, pull requests, and repo automation.
- Filesystem access scoped to the active workspace.
- Browser or Playwright tools for local web app testing.
- Current documentation lookup for framework, API, Vercel, Supabase, and package behavior.
- Web search for current research and recommendations.
- Supabase/Postgres tooling only when database access is required and approved.
- Memory tooling only for safe, durable personal/project facts.

## Operating Rules

- Use the GitHub plugin for this repository whenever possible.
- Keep write access scoped and intentional.
- Do not store credentials in workflow files.
- Do not add fake API keys.
- Verify current docs for unstable dependencies.
- Prefer simple automations over complex systems.

## Good Codex Prompt

```text
Use AGENTS.md as the control file. Use the Orchestrator if this has multiple stages. Keep the work personal-only, avoid secrets, and verify the result before summarizing.
```
