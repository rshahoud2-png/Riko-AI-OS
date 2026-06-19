# MCP Recommendations For General AI Assistants

## Core Tools

- Filesystem for approved local files.
- Browser or web search for current public facts.
- GitHub for repository collaboration.
- Playwright for browser verification.
- Context7 for current developer documentation.
- Memory/OpenMemory or Mem0 for durable, safe recall.
- Supabase/Postgres for database projects.
- Figma for product/design workflows.
- Sequential thinking for complex analysis.

## Selection Guidance

- Start with the fewest tools needed.
- Prefer local-first tools for private work.
- Prefer official APIs and documented MCP servers.
- Use read-only credentials until write access is truly needed.
- Review permissions quarterly.

## Security Rules

- No fake API keys in examples.
- No real secrets in config samples.
- No broad filesystem access unless the user explicitly approves it.
- No production writes without a rollback plan.
