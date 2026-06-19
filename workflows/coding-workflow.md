# Coding Workflow

Use for full-stack apps, AI app features, API integrations, Supabase changes, Vercel fixes, and GitHub-backed code work.

1. Confirm the user goal and acceptance criteria.
2. Inspect the existing repository or files before editing.
3. Choose the smallest safe implementation path.
4. Implement using existing project patterns.
5. Add or update focused tests when risk warrants.
6. Run available checks or explain why they could not run.
7. Review the diff for regressions, secrets, and unclear behavior.
8. Summarize files changed, validation, and next steps.

## Gates

- Requirements are clear enough to act.
- No secrets or fake credentials are added.
- User data and customer data stay out of code and logs.
- Deployment-impacting changes include rollback notes.
