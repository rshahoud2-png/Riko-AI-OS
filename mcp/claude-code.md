# MCP Recommendations For Claude Code

## Recommended Baseline

- Filesystem: local project file access.
- GitHub: issues, pull requests, comments, and CI logs.
- Playwright or browser automation: UI testing and web workflows.
- Context7: current library and API documentation.
- Memory/OpenMemory or Mem0: durable user and project memory.
- Web search such as Tavily: current external research.
- Supabase/Postgres: database inspection and query support when approved.
- Figma: design inspection when available.
- Sequential thinking: complex planning and root cause analysis.

## Setup Notes

- Prefer project-specific MCP configuration for work tools.
- Keep API keys in the client secret store or environment variables, never in this repo.
- Give Claude only the filesystem roots it needs.
- Use read-only database credentials unless writes are explicitly required.
- Disable tools that are not needed for a project.

## Suggested Claude Rule

```text
Use Context7 for current API, framework, package, and platform documentation. Use memory only for durable facts that would help future sessions. Never store secrets.
```
