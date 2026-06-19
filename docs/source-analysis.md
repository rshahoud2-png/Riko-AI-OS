# Source Analysis

## Repositories Studied

- `hesreallyhim/awesome-claude-code`: Claude Code ecosystem curation, skills, hooks, tools, and emphasis on originality/security.
- `VoltAgent/awesome-codex-subagents`: Codex-native subagent structure, explicit delegation, model/sandbox fields, and category taxonomy.
- `Ischca/awesome-agents-md`: AGENTS.md examples and root instruction patterns.
- `punkpeye/awesome-mcp-servers`: MCP categories and tool selection patterns.
- `mem0ai/mem0`: memory categories, memory safety gates, retrieval concepts, and durable fact patterns.
- `upstash/context7`: current documentation retrieval for library/API work.
- `ComposioHQ/awesome-codex-skills`: skill file shape and practical workflow style.
- `milisp/awesome-chatgpt-claude-agents`: agent ecosystem categories and multi-agent workflow references.

## Patterns Adapted

- Root instruction files for assistant behavior.
- Specialist role files with clear invocation rules.
- Skill files as reusable task methods.
- Explicit multi-agent orchestration instead of implicit spawning.
- Read-only versus write-capable role separation.
- Current-docs retrieval for API and platform work.
- Memory gates for durable, safe facts.
- MCP profiles grouped by assistant environment.

## Patterns Intentionally Avoided

- Copying full third-party agent or skill files.
- Installing large toolchains by default.
- Storing API keys or placeholder secrets.
- Recommending every MCP server in an awesome list.
- Overly autonomous workflows without human approval gates.
