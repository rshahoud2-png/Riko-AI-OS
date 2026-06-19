# Windows Setup

## Prerequisites

- Git for Windows.
- PowerShell 5.1 or newer.
- Node.js 18 or newer if using Context7, Playwright, or Node-based MCP servers.
- Python 3.11 or newer if using Python-based tools.

## Initialize Repository

```powershell
cd Riko-AI-OS
git init
git add .
git commit -m "Initial Riko AI OS setup"
```

## Optional Tool Installs

Only install what you need:

```powershell
node --version
npm --version
git --version
```

For Context7, follow current official setup:

```powershell
npx ctx7 setup
```

Do not paste API keys into repository files.
