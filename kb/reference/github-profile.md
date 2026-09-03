---
title: "SoftSpark GitHub Profile Page"
category: reference
service: softspark
tags: [github-profile, company, founder, open-source, public-content]
created: "2026-07-27"
last_updated: "2026-09-03"
description: "Defines the content, evidence sources, and update procedure for the public softspark/softspark GitHub profile."
version: "1.2.0"
---

# SoftSpark GitHub Profile Page

## Purpose

The `softspark/softspark` repository is the public profile rendered at [github.com/softspark](https://github.com/softspark). The account is a personal GitHub account, not an organization.

The page explains two connected subjects:

- **SoftSpark as a company:** commerce engineering, infrastructure delivery, AI systems, operational enablement, and public modules.
- **Łukasz Krzemień as the founder:** hands-on ownership of architecture, implementation, delivery, and production operations.

The README must keep those subjects distinct. SoftSpark describes the delivery capability and public systems. The Founder section explains who performs and owns the engineering work.

## Repository Structure

```text
softspark/
  README.md
  LICENSE
  NOTICE
  CLAUDE.md
  kb/reference/github-profile.md
```

`README.md` is the public page. This document records its content contract and verification sources.

## Content Contract

The profile contains these sections in order:

1. **Header:** company scope, 12+ years of operator experience, website, and contact address.
2. **Founder:** Łukasz Krzemień, his hands-on engineering role, and the domains he works across.
3. **What We Build:** commerce platforms, infrastructure and delivery, AI delivery systems, and operational enablement.
4. **Commerce Engineering:** platform work, performance, product data, and operations.
5. **Infrastructure and Delivery:** provisioning, automation, CI/CD, observability, recovery, and the 99.95% stability target.
6. **AI Delivery:** ai-toolkit, jira-mcp, retrieval systems, dsh-codex, dsh-orchestrator, and control-plane guardrails.
7. **How We Work:** Diagnose, Design, Codify, Ship, Transfer.
8. **Typical Engagements:** concrete production and engineering-system work.
9. **Open Source:** six public Apache-2.0 modules with dynamic npm version badges.
10. **Selected Building Blocks:** technology badges relevant to the described work.
11. **Contact and License:** website, email, Apache-2.0, NOTICE, and linked-repository license boundary.

## Public Module Inventory

The Open Source table mirrors the current non-fork public repositories with a product surface:

| Repository | Distribution | Role |
|---|---|---|
| `softspark/ai-toolkit` | `@softspark/ai-toolkit` | Shared AI engineering toolkit for 12 developer-tool integrations |
| `softspark/jira-mcp` | `@softspark/jira-mcp` | Multi-instance Jira MCP server |
| `softspark/dsh-codex` | `@softspark/dsh-codex` | DeepSeek Harness Codex provider using local ChatGPT authentication |
| `softspark/dsh-orchestrator` | `@softspark/dsh-orchestrator` | DeepSeek Harness delegation bundle for Claude Code and Copilot Gemini |
| `softspark/gitspace` | `@softspark/gitspace` | Workspace-bound Git identity, GitHub account, SSH key, signing, and audit controls |
| `softspark/mage2x` | `@softspark/mage2x` | Magento container command runner with explicit target and production safeguards |

All six repositories use Apache-2.0 and `NOTICE`. npm badges resolve the current registry version dynamically, so the profile does not copy version numbers into prose.

## Evidence Sources

Use current public metadata before changing claims:

```bash
gh repo list softspark --visibility public --limit 100 \
  --json name,description,url,licenseInfo,isArchived,isFork,repositoryTopics

npm view @softspark/ai-toolkit version description --json
npm view @softspark/jira-mcp version description --json
npm view @softspark/dsh-codex version description --json
npm view @softspark/dsh-orchestrator version description --json
npm view @softspark/gitspace version description --json
npm view @softspark/mage2x version description --json
```

Do not list a private, archived, unlicensed, or placeholder repository. Do not copy claims from a local branch when the public repository or registry says something different.

## Update Procedure

1. Retrieve current GitHub and npm metadata using the commands above.
2. Update `README.md` and this reference in the same commit.
3. Keep the company description, Founder section, public module table, and contact details consistent.
4. Remove promotional adjectives that are not supported by a number, named capability, or public artifact.
5. Validate Markdown structure, links, licensing, and banned brand-voice patterns.
6. Review the rendered README on GitHub after push.

## Verification

```bash
git diff --check
python3 -c "from pathlib import Path; text='\n'.join(Path(p).read_text() for p in ('README.md','kb/reference/github-profile.md')); banned=(chr(0x2013),chr(0x2014),'cutting'+'-edge','game'+'-changer','revolution'+'ary','seam'+'less','state-of-the-'+'art'); assert not [value for value in banned if value in text]"
rg -n "dsh-codex|dsh-orchestrator|gitspace|mage2x|ai-toolkit|jira-mcp|Łukasz Krzemień" README.md kb/reference/github-profile.md
```

The Python assertion must exit zero. The `rg` command must find all six public modules plus the Founder identity in both documentation surfaces where applicable.

## License

`LICENSE` and `NOTICE` cover this repository's README, KB, and agent instructions. Linked repositories retain their own licenses. Keep the Open Source table aligned with the SPDX identifier GitHub detects for each project.
