# GitHub Profile Page — softspark/softspark

## What This Is

Special GitHub repository whose `README.md` renders as the public profile at [github.com/softspark](https://github.com/softspark). This is a **personal account** profile (not an organization).

## How It Works

- Repo name matches the account name (`softspark/softspark`) — GitHub treats it as a profile repo
- `README.md` at the repo root is displayed on the profile page
- Supports full GitHub Flavored Markdown + limited HTML (`<p align>`, `<details>`, `<img>`, `<picture>`)

## Current Structure

```
softspark/
  README.md      # Profile page content
  .gitignore     # .idea/, .DS_Store
  kb/            # Knowledge base for RAG indexing
```

## Content Sections

1. **Header** — concise value proposition (12+ years tagline)
2. **Infrastructure — The System Behind the Revenue** — provisioning, automation, delivery stack table; 99.95% stability target
3. **Our Approach** — "What defines our work" and "What We Help Teams Fix" tables
4. **E-Commerce — Revenue Engine** — checkout, search/cache, PIM/data flow, ops coverage
5. **AI Delivery — AI Orchestration** — toolkits, knowledge (RAG), MCP, orchestration, SDK layers table
6. **Engineering Protocol — How We Work** — 5-step operating model (Diagnose → Design → Codify → Ship → Transfer)
7. **Working Style** — principles + "Typical Outputs" deliverables table
8. **Selected Building Blocks** — shields.io `for-the-badge` tech row (Docker, Terraform, Ansible, AWS, Hetzner, PHP, Python, Node.js, TypeScript, Magento, PostgreSQL, GitLab CI)
9. **Open Source** — table with public repos ([ai-toolkit](https://github.com/softspark/ai-toolkit) live) and upcoming (Jira MCP server)
10. **Footer** — website and email links

## How to Update

### Adding a public repository

Uncomment the table in the "Open Source" section and add a row:

```markdown
| [repo-name](https://github.com/softspark/repo-name) | Short description |
```

### Adding a tech badge

Add to the badge row:

```html
<img src="https://img.shields.io/badge/Name-COLOR?style=for-the-badge&logo=SLUG&logoColor=white" alt="Name">
```

Find logo slugs at [simple-icons.github.io/simple-icons](https://simple-icons.github.io/simple-icons/).

## Related

- **`.github` repo** (local, not yet pushed) — community health files: `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, `profile/README.md`. The `profile/README.md` only renders if the account converts to an organization.
- Remote: `git@softsparkrepo:softspark/softspark.git`
