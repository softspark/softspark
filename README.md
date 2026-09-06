# SoftSpark

> Commerce infrastructure, production delivery, and AI systems for teams that cannot afford fragile operations.

SoftSpark is a founder-led engineering company with 12+ years of operator experience. We design, build, and stabilize revenue-critical platforms. Our work stays close to production: architecture, infrastructure, releases, observability, recovery, and engineering automation.

[softspark.eu](https://softspark.eu) · [biuro@softspark.eu](mailto:biuro@softspark.eu)

## Founder

SoftSpark is built and led by **Łukasz Krzemień**, a software and infrastructure engineer who works directly on architecture, implementation, delivery, and production operations.

Łukasz combines commerce-platform experience with infrastructure automation and AI engineering. His work spans Magento and PHP systems, cloud and VPS infrastructure, CI/CD, observability, knowledge retrieval, MCP servers, coding-agent platforms, and multi-model orchestration.

The operating principle is simple: important systems need explicit ownership, measurable acceptance criteria, repeatable delivery, and a tested recovery path.

## What We Build

| Area | Scope | Typical stack |
|---|---|---|
| **Commerce platforms** | Catalog, checkout, search, cache, PIM, integrations, multi-store operations | Magento 2, PWA, Akeneo, Symfony, Pimcore |
| **Infrastructure and delivery** | Provisioning, containers, CI/CD, observability, backup, recovery | Terraform, Terragrunt, Ansible, Docker, AWS, Azure, Hetzner |
| **AI delivery systems** | Coding-agent rules, knowledge retrieval, MCP servers, model routing, multi-agent workflows | Claude Code, Codex, Copilot, Gemini, MCP, RAG, CRAG |
| **Operational enablement** | SOPs, runbooks, architecture decisions, incident workflows, team tooling | GitHub Actions, GitLab CI, OpenTelemetry, Prometheus, Grafana |

## Commerce Engineering

We work on the application paths where latency, deployment risk, and integration failures affect revenue.

| Capability | Delivery scope |
|---|---|
| **Platform engineering** | Magento 2 B2C and B2B, headless storefronts, middleware, extensions, upgrade paths |
| **Performance** | Varnish, OpenSearch, queues, cache policy, PHP runtime, database diagnostics |
| **Product data** | Akeneo PIM, catalog normalization, feeds, imports, exports, synchronization |
| **Operations** | Multi-store releases, monitoring, incident loops, rollback procedures, peak-readiness checks |

## Infrastructure and Delivery

Our infrastructure work targets repeatable changes and recoverable failures. The stability target for release-critical paths is **99.95%**.

| Layer | Implementation |
|---|---|
| **Provisioning** | Terraform and Terragrunt for Hetzner Cloud, AWS, Azure, and hybrid VPS environments |
| **Automation** | Containerized Ansible, explicit inventories, idempotent playbooks, configuration ownership |
| **Delivery** | CI/CD validation, zero-downtime deployment patterns, health checks, rollback gates |
| **Operations** | Structured logs, metrics, tracing, backups, restore tests, capacity and cost reviews |

## AI Delivery

We treat AI as an engineering system, not a chat window. Rules, permissions, retrieval, evaluation, and release gates remain explicit.

| Layer | SoftSpark implementation |
|---|---|
| **Engineering toolkit** | [ai-toolkit](https://github.com/softspark/ai-toolkit) distributes 114 skills, 44 agents, hooks, audits, and shared policies across 14 developer-tool integrations |
| **Work management** | [jira-mcp](https://github.com/softspark/jira-mcp) connects MCP clients to multiple Jira instances with ADF formatting, caching, and comment templates |
| **Knowledge** | Hybrid retrieval, corrective RAG, multi-hop search, reranking, evaluation sets, and knowledge-gap tracking |
| **Model access** | [dsh-codex](https://github.com/softspark/dsh-codex) connects DeepSeek Harness to a locally authenticated Codex app server using a ChatGPT subscription |
| **Orchestration** | [dsh-orchestrator](https://github.com/softspark/dsh-orchestrator) delegates bounded tasks to Claude Code and GitHub Copilot Gemini through native subscription logins |
| **Session tools** | [dsh-file-preview](https://github.com/softspark/dsh-file-preview) previews files inside a conversation; [dsh-process-console](https://github.com/softspark/dsh-process-console) shows agent and subagent activity with paired tool calls and results |
| **Control plane** | Approval gates, least-privilege tools, credential boundaries, SARIF audits, signed package provenance, human review |

## How We Work

1. **Diagnose.** Inspect architecture, release flow, runtime evidence, operational risk, and the actual bottleneck.
2. **Design.** Define ownership, interfaces, environments, migration steps, failure modes, and measurable acceptance criteria.
3. **Codify.** Implement infrastructure, services, pipelines, policies, tests, SOPs, and runbooks.
4. **Ship.** Release small reversible changes with automated gates, health verification, and a rollback path.
5. **Transfer.** Leave the team with documented systems, maintainable tooling, and evidence they can reproduce.

## Typical Engagements

- Stabilize Magento, PWA, search, cache, queue, or integration paths that affect conversion and release safety.
- Standardize infrastructure that has grown through manual changes and undocumented dependencies.
- Build CI/CD, observability, backup, restore, and incident procedures around an existing production platform.
- Convert AI experiments into governed tools with retrieval, permissions, evaluation, audit trails, and human approval.
- Create reusable engineering systems: modules, MCP servers, agent workflows, SOPs, runbooks, and knowledge bases.

## Open Source

| Project | Purpose | Distribution | License |
|---|---|---|---|
| [ai-toolkit](https://github.com/softspark/ai-toolkit) | Shared skills, agents, hooks, policies, audits, and cross-tool generators | [![npm](https://img.shields.io/npm/v/@softspark/ai-toolkit?label=npm)](https://www.npmjs.com/package/@softspark/ai-toolkit) | Apache-2.0 |
| [jira-mcp](https://github.com/softspark/jira-mcp) | Multi-instance Jira MCP server with ADF conversion and local task caching | [![npm](https://img.shields.io/npm/v/@softspark/jira-mcp?label=npm)](https://www.npmjs.com/package/@softspark/jira-mcp) | Apache-2.0 |
| [dsh-codex](https://github.com/softspark/dsh-codex) | DeepSeek Harness provider for locally authenticated Codex app-server sessions | [![npm](https://img.shields.io/npm/v/@softspark/dsh-codex?label=npm)](https://www.npmjs.com/package/@softspark/dsh-codex) | Apache-2.0 |
| [dsh-orchestrator](https://github.com/softspark/dsh-orchestrator) | DeepSeek Harness bundle for Claude Code and Copilot Gemini delegation | [![npm](https://img.shields.io/npm/v/@softspark/dsh-orchestrator?label=npm)](https://www.npmjs.com/package/@softspark/dsh-orchestrator) | Apache-2.0 |
| [dsh-file-preview](https://github.com/softspark/dsh-file-preview) | In-conversation file preview for DeepSeek Harness with a host Remote and browser modal | [![npm](https://img.shields.io/npm/v/@softspark/dsh-file-preview?label=npm)](https://www.npmjs.com/package/@softspark/dsh-file-preview) | Apache-2.0 |
| [dsh-process-console](https://github.com/softspark/dsh-process-console) | Live agent and subagent consoles for DeepSeek Harness with paired tool calls and results | [![npm](https://img.shields.io/npm/v/@softspark/dsh-process-console?label=npm)](https://www.npmjs.com/package/@softspark/dsh-process-console) | Apache-2.0 |
| [gitspace](https://github.com/softspark/gitspace) | Git identity, GitHub account, SSH key, signing, and audit controls bound to workspace directories | [![npm](https://img.shields.io/npm/v/@softspark/gitspace?label=npm)](https://www.npmjs.com/package/@softspark/gitspace) | Apache-2.0 |
| [mage2x](https://github.com/softspark/mage2x) | Magento and shell command runner for Docker, Podman, and Kubernetes with target and production safeguards | [![npm](https://img.shields.io/npm/v/@softspark/mage2x?label=npm)](https://www.npmjs.com/package/@softspark/mage2x) | Apache-2.0 |

Every public module starts at `1.0.0`, ships with Apache-2.0 and `NOTICE`, and uses automated supply-chain verification appropriate to its distribution channel.

## Selected Building Blocks

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Hetzner](https://img.shields.io/badge/Hetzner-D50C2D?style=for-the-badge&logo=hetzner&logoColor=white)
![Magento](https://img.shields.io/badge/Magento-EE672F?style=for-the-badge&logo=magento&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

## Contact

Architecture review, commerce stabilization, infrastructure automation, or AI delivery system:

[softspark.eu](https://softspark.eu) · [biuro@softspark.eu](mailto:biuro@softspark.eu)

This profile is licensed under [Apache-2.0](LICENSE). See [NOTICE](NOTICE). Linked repositories carry their own licenses.
