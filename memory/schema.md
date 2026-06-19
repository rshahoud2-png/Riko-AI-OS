# Memory Schema

Use this schema when implementing memory in Mem0, OpenMemory, a database table, or a local knowledge store.

```yaml
id: string
category: identity | preference | rule | project | configuration | technical | business | relationship | decision
fact: string
importance: number
created_at: date
updated_at: date
source: string
scope: user | project | organization | session
expires_at: date | null
tags:
  - string
```

## Retrieval Pattern

1. Search project-scoped memories first.
2. Search user-scoped memories second.
3. Use only relevant memories.
4. Tell the user when memory materially affects a recommendation.
