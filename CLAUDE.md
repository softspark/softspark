# SoftSpark GitHub Profile

## Overview
GitHub profile repository (softspark/softspark) — renders as the public organization page at github.com/softspark. Content-only repo, no runnable application.

## Tech Stack
- **Language**: Markdown
- **Framework**: N/A (static GitHub profile)
- **Database**: N/A

## Commands
```bash
# Dev: N/A — edit README.md directly
# Test: N/A
# Lint: N/A
# Build: N/A
```

## Key Conventions
- README.md is the sole deliverable — it renders as the GitHub org profile page
- Conventional commits: `feat:`, `fix:`, `docs:`, `chore:`
- No AI co-authorship lines in commits
- KB reference docs live in `kb/reference/`
- Git remote uses custom domain: `git@softsparkrepo:softspark/softspark.git`

## MCP Servers
- **filesystem** — local file access via `@modelcontextprotocol/server-filesystem`
- **github** — GitHub API integration via `@modelcontextprotocol/server-github` (requires `GITHUB_PERSONAL_ACCESS_TOKEN`)
