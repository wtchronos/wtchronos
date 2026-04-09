<h3 align="center">Warren Command</h3>
<p align="center">Personal command infrastructure for turning open-ended work into routed, concrete outputs.</p>

<p align="center">
  <a href="https://warrencommand.dev"><img src="https://img.shields.io/badge/warrencommand.dev-0a1220?style=for-the-badge&logoColor=white" alt="Website" /></a>
</p>

---

### What this is

A command layer over specialized operators with clear boundaries.

Research, synthesis, and writing happen in one surface. Code and repo execution route to Claude Code. Technical challenge and adversarial review route to Codex. Scheduled follow-through routes to Kairos.

The point is not to simulate one all-purpose agent. It is to keep roles clear, preserve human control, and reduce drift. In practice, Warren Command turns messy inputs into briefs, drafts, decisions, and handoff packets that move directly into execution.

It sits between raw tools and finished work: close enough to the stack to be useful, narrow enough to stay honest about what it does. The result is a tighter operating loop, not a claim of autonomy.

---

### How it works

**Routing, not orchestration.** Every input gets classified and sent to the operator that handles it best. The command layer decides *where* work goes. Operators decide *how* it gets done.

**Execution packets.** Work moves between operators as sealed, immutable packets with objectives, scope constraints, verification criteria, and audit trails. Every decision compiles into a packet before any executor touches it.

**Progressive trust.** Operators start with read-only access and earn broader capabilities through demonstrated reliability. Destructive operations always require human approval.

---

### Systems

| System | Role |
|--------|------|
| **[Cortix](https://github.com/wtchronos/cortix)** | Control plane. Routes intent, checks trust, dispatches to executors, tracks completion. |
| **[Kairos](https://github.com/wtchronos/kairos-w)** | Always-on agent. Handles Telegram commands, scheduled tasks, VPS ops, and state reconciliation. |
| **[Anvil](https://github.com/wtchronos/anvil)** | Governance. Trust ledger, overnight automation pipeline, pattern-to-skill extraction. |
| **[Nerve Center](https://github.com/wtchronos/nerve-center)** | Monitoring. System health, service uptime, real-time alerts. |
| **[Prompt Foundry](https://github.com/wtchronos/prompt-foundry)** | Prompt OS. Version control, eval pipelines, and execution packet generation for managed prompts. |
| **[Warren Command](https://warrencommand.dev)** | The command layer itself. Synthesis, framing, routing, artifact production. |

---

### Stack

<p>
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /></a>
  <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" /></a>
  <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" /></a>
  <a href="https://neon.tech/"><img src="https://img.shields.io/badge/Neon_Postgres-4169E1?style=flat-square&logo=postgresql&logoColor=white" /></a>
  <a href="https://www.digitalocean.com/"><img src="https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white" /></a>
</p>

| Layer | Technologies |
|-------|-------------|
| **Backend** | Python 3.12, FastAPI, Pydantic v2, asyncio, httpx |
| **Infrastructure** | DigitalOcean VPS, systemd (9 services), Caddy reverse proxy |
| **Data** | Neon Postgres + pgvector, SQLite (local ledger), JSONL audit chains |
| **AI/LLM** | OpenRouter (model routing), Claude Code (27 custom skills), Codex (review) |

---

<p align="center">
  Built by one person. <a href="https://warrencommand.dev">warrencommand.dev</a>
</p>
