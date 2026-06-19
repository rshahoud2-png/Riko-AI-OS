# Windows Setup For Personal Codex Use

## Prerequisites

- Git for Windows.
- PowerShell 5.1 or newer.
- Node.js 18 or newer for most modern app projects and optional Context7 tooling.
- Python 3.11 or newer only when a project needs Python.

## Use In A Project

Copy or reference `AGENTS.md` from this repository in a personal project where you want Codex to follow Riko AI OS.

```powershell
Copy-Item .\AGENTS.md C:\path\to\personal-project\AGENTS.md
```

## Optional Tool Checks

```powershell
git --version
node --version
npm --version
python --version
```

## GitHub Use

For this repository, prefer the GitHub plugin instead of local Git operations when creating, updating, or deleting files.

## Safety

Do not paste API keys, tokens, work credentials, customer data, or medical records into repository files.
