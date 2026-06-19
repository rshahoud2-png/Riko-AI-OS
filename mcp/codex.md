# MCP Recommendations For Codex

## Recommended Baseline

- GitHub connector for PRs, issues, reviews, and CI.
- Filesystem access scoped to the workspace.
- Playwright/browser tool for local app verification.
- Context7 or official docs search for current API behavior.
- Memory/OpenMemory or Mem0 for durable project/user facts.
- Web search such as Tavily for current research.
- Supabase/Postgres for approved database work.
- Figma for design-to-code tasks when available.
- Sequential thinking for complex investigation and planning.

## Operating Rules

- Prefer read-only tools for research and review agents.
- Use workspace-write only for agents that implement changes.
- Do not grant production write access by default.
- Do not log secrets or paste them into prompts.
- Verify current docs for unstable dependencies.

## Good Codex Prompt

```text
Use the Researcher agent to verify current docs, then the Full Stack Developer to implement, then the Code Reviewer to inspect the diff. Keep all edits scoped to this repository.
```
