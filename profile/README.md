# Autiladus — AI Swarm Platform

*Org: [github.com/autiladus](https://github.com/autiladus) · [autilad.us](https://autilad.us) · [Docs](https://autiladus.wokspec.org) · MIT*

---

You're juggling single-agent AI assistants. Debugging hallucinated code. Watching your AI produce plausible-but-wrong solutions.

**Autiladus deploys a swarm of specialist AI agents** — explorers, critics, implementers — that validate each other's work and reach consensus before shipping code.

---

## Why Autiladus?

| Problem | Solution |
|---------|----------|
| Plausible but incorrect code | **Critic Pool** validates every solution |
| Context window limits crash sessions | **Hierarchical Memory** (working/project/global) |
| No transparency in AI decisions | **Agent-by-agent audit trail** |
| Single point of failure | **Consensus Engine** — multi-agent agreement |
| Linear scaling | **Parallel swarm** — simultaneous work |
| Fixed agent count | **Dynamic Scaling** — 5/20/50+ agents |

---

## The Swarm Architecture

```
Request Orchestrator → Task Planner → Agent Pools → Consensus → Synthesizer
                                         ↓
              ┌──────────────────────────┼──────────────────────────┐
              ▼                          ▼                          ▼
        ┌──────────┐            ┌──────────┐            ┌──────────┐
        │ Explorer │            │  Critic  │            │   Tool   │
        │   Pool   │            │   Pool   │            │  Agents  │
        │(research)│            │(validate)│            │(execute) │
        └──────────┘            └──────────┘            └──────────┘
```

---

## Core Features

- **Forge** — plan → execute → verify with guardrails
- **Crucible** — max-autonomy runs with verification-first recovery
- **Swarm Mode** — deploy 5/20/50+ specialist agents
- **Hashline Editing** — content-hash anchored edits, zero stale-line errors
- **Consensus Engine** — voting, scoring, ranking
- **Memory Layers** — Redis (working), Vector DB (project), PostgreSQL (global)

---

## Dynamic Scaling

| Mode | Agents | Use Case |
|------|--------|----------|
| **Fast** | 5 | Quick fixes |
| **Balanced** | 20 | Feature development |
| **Deep Think** | 50+ | Complex architectures |

---

## Quick Start

```bash
# Install
bunx autiladus install

# Initialize
autiladus init

# Run a task
autiladus forge "add user authentication"

# Swarm mode
autiladus forge --deep "rearchitect the backend"
```

---

## Commands

| Command | Description |
|---------|-------------|
| `autiladus init` | Scaffold config |
| `autiladus forge "<task>"` | One-shot with verification |
| `autiladus crucible "<task>"` | Autonomous with retries |
| `autiladus autiloop <n> "<task>"` | Iterative refinement |
| `autiladus runs` | Inspect ledger |
| `autiladus doctor` | Verify integration |

---

## Environment Variables

```bash
GROQ_API_KEY           # Primary (Llama 3.3)
OPENAI_API_KEY         # Fallback
BROWSER_WS_ENDPOINT   # Remote browser
ANTHROPIC_API_KEY    # Claude
```

---

## Philosophy

1. **Automation ≠ black box** — Every decision is auditable
2. **Multiple eyes catch what one misses** — Critic Pool catches bugs
3. **Consensus over confidence** — Agreement > certainty
4. **Scale elastically** — Same tool, different scale
5. **Verify before commit** — Ledger preserves every run

---

## Documentation

- [Installation](https://github.com/autiladus/autiladus/blob/main/docs/guide/installation.md)
- [Architecture](https://github.com/autiladus/autiladus/blob/main/docs/architecture.md)
- [API Reference](https://github.com/autiladus/autiladus/blob/main/docs/api.md)
- [Configuration](https://github.com/autiladus/autiladus/blob/main/docs/configuration.md)

---

## Contribute

```bash
git checkout -b feature/your-feature
npm run dev
npm test
# Fork → branch → PR against main
```

---

## Support

- **Issues**: [github.com/autiladus/autiladus/issues](https://github.com/autiladus/autiladus/issues)
- **Discussions**: [github.com/autiladus/autiladus/discussions](https://github.com/autiladus/autiladus/discussions)
- **Security**: `security@wokspec.org`

---

MIT License · Built by [WokSpec](https://wokspec.org)
