# Memory Schema

Use this schema only if a memory tool or database is added later. This repository does not require memory tooling by default.

```yaml
id: string
category: identity | preference | rule | project | configuration | technical | business | career | finance | event | productivity | decision
fact: string
importance: number
created_at: date
updated_at: date
source: string
scope: personal | project | session
expires_at: date | null
tags:
  - string
```

## Retrieval Pattern

1. Search project-scoped memories first.
2. Search personal preferences second.
3. Use only relevant memories.
4. Never retrieve or store secrets, medical records, work credentials, or customer private data.
5. Tell the user when memory materially affects a recommendation.
