<div align="center">

```
█████╗ ██╗   ██╗████████╗██╗██╗      █████╗ ██████╗ ██╗   ██╗███████╗
██╔══██╗██║   ██║╚══██╔══╝██║██║     ██╔══██╗██╔══██╗██║   ██║██╔════╝
███████║██║   ██║   ██║   ██║██║     ███████║██║  ██║██║   ██║███████╗
██╔══██║██║   ██║   ██║   ██║██║     ██╔══██║██║  ██║██║   ██║╚════██║
██║  ██║╚██████╔╝   ██║   ██║███████╗██║  ██║██████╔╝╚██████╔╝███████║
╚═╝  ╚═╝ ╚═════╝    ╚═╝   ╚═╝╚══════╝╚═╝  ╚═╝╚═════╝  ╚═════╝ ╚══════╝
```

**Multi-agent orchestration. Legion coordination. Terminal-first.**

[![Site](https://img.shields.io/badge/autiladus.wokspec.org-111118?style=flat-square&color=b31237)](https://autiladus.wokspec.org)
[![Discord](https://img.shields.io/badge/discord-T5KnUgAKK3-111118?style=flat-square&color=b31237)](https://discord.gg/T5KnUgAKK3)
[![GitHub](https://img.shields.io/badge/github.com%2Fautiladus-111118?style=flat-square&color=b31237)](https://github.com/autiladus)

</div>

---

## What Autiladus builds

Autiladus is a multi-agent orchestration framework. You describe a task. The orchestrator classifies complexity, decomposes it into work, and routes it to a coordinated fleet of specialist agents running in parallel. Results pass through a consensus engine before they surface.

Not a single-agent assistant. Not a wrapper. Infrastructure for agent swarms.

```
Prompt → Orchestrator → Task Planner → Agent Fleet (parallel)
                                              │
                    ┌─────────────────────────┼─────────────────────────┐
                    ▼                         ▼                         ▼
             Explorer Agent           Critic Agent              Tool Agent
             (discover, map)         (validate, score)         (execute, write)
                    │                         │                         │
                    └─────────────────────────┼─────────────────────────┘
                                              ▼
                                     Consensus Engine
                                   (vote → agree → ship)
```

---

## Core capabilities

- **Swarm orchestration** — parallel agent fleets with automatic task routing
- **Consensus engine** — multi-agent voting before results are returned
- **Complexity-aware routing** — simple tasks get 2 agents; complex ones get 5+
- **Forge / Crucible / Swarm** — CLI modes for one-shot, autonomous, and explicit swarm execution
- **Browser agent** — Playwright-powered web automation inside your own authenticated session
- **Ledger** — every run logged, every decision inspectable

---

## Repositories

| Repo | Description |
|------|-------------|
| [autiladus/autiladus](https://github.com/autiladus/autiladus) | Core platform — orchestration engine, swarm, CLI, web dashboard |

---

## Current phase

`feature/swarm-mvp-phase1` — Swarm MVP in active development.

Core swarm engine and consensus protocol are live. Dynamic scaling, hierarchical memory, and agent communication channels are next.

Build updates and early access → **[Discord](https://discord.gg/T5KnUgAKK3)**

---

## Stack

`TypeScript` · `Next.js 15` · `Node.js` · `Groq (Llama 3.3)` · `OpenAI` · `Playwright` · `BullMQ` · `Redis` · `Zod` · `Vitest`

---

## Contribute

Looking for: systems engineers, AI/agent developers, CLI developers.

→ [CONTRIBUTING.md](https://github.com/autiladus/autiladus/blob/main/CONTRIBUTING.md)  
→ [Open issues](https://github.com/autiladus/autiladus/issues)  
→ [Discord](https://discord.gg/T5KnUgAKK3)

---

<div align="center">

[autiladus.wokspec.org](https://autiladus.wokspec.org) · [discord.gg/T5KnUgAKK3](https://discord.gg/T5KnUgAKK3) · MIT · Part of [WokSpec](https://wokspec.org)

[![Twitter](https://img.shields.io/twitter/follow/autiladus?style=flat-square&logo=x&label=%40autiladus)](https://x.com/autiladus)

</div>
