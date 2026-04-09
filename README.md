<h3 align="center">Warren Command</h3>
<p align="center">A personal autonomous operating system — 6 integrated systems running 24/7 on a single VPS, coordinated by AI.</p>

<p align="center">
  <a href="https://warrencommand.dev"><img src="https://img.shields.io/badge/warrencommand.dev-0a1220?style=for-the-badge&logoColor=white" alt="Website" /></a>
  <a href="https://ops.warrencommand.dev"><img src="https://img.shields.io/badge/Ops_Dashboard-1a3a5c?style=for-the-badge&logoColor=white" alt="Ops Dashboard" /></a>
</p>

---

### What this is

Not a collection of repos — a unified system where an autonomous agent, a governance layer, a control plane, a monitoring stack, a prompt OS, and a cross-session memory layer all talk to each other. Every component exists because it solves a real problem in running AI infrastructure solo.

The goal: **an always-on intelligence layer that maintains, monitors, and improves itself** while I focus on building the next thing.

---

### The system

| System | What it does | Repo |
|--------|-------------|------|
| **Cortix** | Unified autonomous OS kernel — control plane, service coordination, progressive trust tiers | [`cortix`](https://github.com/wtchronos/cortix) |
| **Kairos** | Always-on AI agent — Telegram interface, 9 mixins, hash-chained audit trail, 3-tier LLM routing | [`kairos-w`](https://github.com/wtchronos/kairos-w) |
| **ANVIL** | Multi-agent governance — trust ledger, trigger engine, overnight build pipeline | [`anvil`](https://github.com/wtchronos/anvil) |
| **Prompt Foundry** | Local-first Prompt OS — version control for prompts, 7 MCP tools, template engine | [`prompt-foundry`](https://github.com/wtchronos/prompt-foundry) |
| **Nerve Center** | Real-time intelligence dashboard — health monitoring, SSE events, alerting | [`nerve-center`](https://github.com/wtchronos/nerve-center) |
| **WCM** | Warren Command Memory — Neon/pgvector, cross-session intelligence, proactive suggestions | [`wcm-server`](https://github.com/wtchronos/wcm-server) |

---

### How it works

**Cortix** is the kernel — it orchestrates every other system through a single control plane on the VPS. Trust tiers (T1-T4) gate what actions are allowed autonomously vs. what requires approval.

**Kairos** runs 24/7 on a DigitalOcean VPS. It polls Telegram for commands, runs scheduled health checks, and surfaces insights proactively. All actions go through a gateway pipeline with approval gates for anything above low risk. Nine systemd services keep it alive.

**ANVIL** enforces the rules. Every action gets a risk level. The overnight pipeline runs autonomous build loops while I sleep — with trust constraints that prevent anything destructive.

**Prompt Foundry** is the prompt engineering layer. Version-controlled prompts, a template engine, and MCP tools that any agent in the system can call.

**Nerve Center** watches everything. Service uptime, cost tracking, pattern detection. Alerts go to Telegram when something degrades. The live dashboard shows current state.

**WCM** gives the whole system memory. Neon Postgres with pgvector means context survives across sessions, models, and tools. Cross-model memory is what makes the system coherent over time.

---

### Stack

<p>
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /></a>
  <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" /></a>
  <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" /></a>
  <a href="https://react.dev/"><img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" /></a>
  <a href="https://neon.tech/"><img src="https://img.shields.io/badge/Neon_Postgres-4169E1?style=flat-square&logo=postgresql&logoColor=white" /></a>
  <a href="https://openrouter.ai/"><img src="https://img.shields.io/badge/OpenRouter-1a1a2e?style=flat-square&logoColor=white" /></a>
  <a href="https://www.digitalocean.com/"><img src="https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white" /></a>
  <a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" /></a>
</p>

| Layer | Technologies |
|-------|-------------|
| **Backend** | Python 3.12 (asyncio, FastAPI, Pydantic v2), httpx |
| **Frontend** | TypeScript, React, Vite, tRPC, Tailwind CSS, SSE |
| **Infrastructure** | DigitalOcean VPS, systemd (12 services), Caddy reverse proxy |
| **Data** | Neon Postgres + pgvector, SQLite, JSONL audit chains |
| **AI/LLM** | OpenRouter (Haiku/Sonnet/Opus routing), Claude Code (38+ custom skills) |
| **Automation** | Hammerspoon (Mac), Telegram Bot API, cron, systemd timers |
| **Security** | bubblewrap sandboxing, HMAC lease management, hash-chained audit logs |

---

### Pinned repos

> [`prompt-foundry`](https://github.com/wtchronos/prompt-foundry) / [`kairos-w`](https://github.com/wtchronos/kairos-w) / [`cortix`](https://github.com/wtchronos/cortix) / [`anvil`](https://github.com/wtchronos/anvil) / [`nerve-center`](https://github.com/wtchronos/nerve-center) / [`warren-ai-walkthrough`](https://github.com/wtchronos/warren-ai-walkthrough)

---

### By the numbers

| Metric | Value |
|--------|-------|
| Build sessions | 306+ |
| Systemd services running | 12 |
| Custom Claude Code skills | 38+ |
| VPS uptime target | 24/7/365 |
| Team size | 1 |

---

<p align="center">Built by one person. Runs 24/7.</p>

<p align="center">
  <a href="https://warrencommand.dev">warrencommand.dev</a>
</p>
