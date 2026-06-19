# Codex Quickstart

Riko AI OS is a personal operating system for using Codex on coding, AI apps, automation, research, planning, career, finance, events, and productivity projects.

Use `AGENTS.md` as the main control file. It tells Codex how to behave, which safety rules to follow, and how to choose agents, skills, and workflows.

## How To Use This Repo With Codex

1. Open a Codex thread for a personal project.
2. Point Codex at this repository or copy `AGENTS.md` into the project you want Codex to work on.
3. Start with a clear outcome, not a vague task.
4. Ask Codex to use the Orchestrator for multi-step work.
5. Ask Codex to use a specific agent or skill when you know what kind of help you need.
6. Keep private data out of prompts unless it is truly needed, and never provide secrets, work credentials, medical records, or customer private data.

## How Agents Are Selected

Agents are specialist roles in `agents/`. Codex should choose the smallest useful set of agents for the request.

Common routing:

- `orchestrator.md`: multi-step or unclear tasks.
- `ai-app-builder.md`: AI apps, LLM workflows, RAG, agentic features, and AI prototypes.
- `full-stack-developer.md`: Next.js, frontend, backend, API, and app implementation.
- `software-architect.md`: architecture, data flow, tradeoffs, and technical plans.
- `code-reviewer.md`: bug, security, regression, and missing-test review.
- `github-automation-specialist.md`: GitHub repo setup, issues, PRs, labels, and repo maintenance.
- `supabase-expert.md`: Supabase, Postgres, auth, RLS, storage, and migrations.
- `vercel-expert.md`: Vercel deployment, environment setup, build failures, and domains.
- `researcher.md`: current facts, tool comparisons, and source-backed decisions.
- `business-advisor.md`: business ideas, offers, operations, and planning.
- `finance-planning-advisor.md`: personal budget and scenario planning support.
- `resume-career-coach.md`: resumes, job applications, and interview prep.
- `event-production-advisor.md`: event planning and event business ideas.
- `personal-productivity-coach.md`: task systems, routines, and project organization.

## How Skills Are Used

Skills are reusable methods in `skills/`. They are not personas. Codex should use them when a task needs a repeatable process.

Common skills:

- `ai-app-building.md`: plan or build AI app features.
- `coding.md`: implement focused code changes.
- `api-integration.md`: connect external APIs safely.
- `supabase-setup.md`: design Supabase schema, auth, and policies.
- `vercel-deployment.md`: deploy and troubleshoot Vercel apps.
- `github-automation.md`: manage GitHub repo workflows.
- `research.md`: research current facts and compare options.
- `automation-planning.md`: design repeatable personal or business automations.
- `financial-planning.md`: compare personal finance scenarios.
- `resume-writing.md`: create career materials.
- `personal-productivity.md`: organize goals, tasks, and routines.

A good request can name both an agent and a skill:

```text
Use the AI App Builder agent and AI App Building skill. Plan a small invoice analyzer app using Next.js, Supabase, and Vercel. Do not code yet.
```

## Example Prompts

1. AI app planning:

```text
Using Riko AI OS, use the AI App Builder and Software Architect. Plan a small AI invoice analyzer app with Next.js, Supabase, and Vercel. Do not code yet. Give me the MVP, data model, risks, and files you would create.
```

2. GitHub cleanup:

```text
Using Riko AI OS, use the GitHub Automation Specialist. Review this repo structure, identify clutter, and propose a safe cleanup plan. Do not delete anything until you explain the changes.
```

3. Vercel deployment debugging:

```text
Using Riko AI OS, use the Vercel Expert and Troubleshooting skill. Help me diagnose this Vercel build error. Separate symptoms, likely causes, tests, and fixes.
```

4. Resume project:

```text
Using Riko AI OS, use the Resume Career Coach and Researcher. Tailor my resume for this job description without inventing experience. Give me revised bullets and keyword gaps.
```

5. Personal productivity:

```text
Using Riko AI OS, use the Personal Productivity Coach. Turn this messy task list into a realistic 3-day plan with priorities, next actions, and a daily review checkpoint.
```

## Safety Reminder

Do not put these into Codex prompts or repo files:

- Passwords, API keys, tokens, or private keys.
- Work credentials.
- TWG client data.
- Customer private data.
- Medical records.
- Fake secret values.

Use environment variable names only, such as `OPENAI_API_KEY`, without including actual values.
