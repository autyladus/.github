# Autiladus · Open automation that plans, executes, and verifies

> Model-agnostic harness for browser + agent workflows. Plan → execute → verify with guardrails, zero vendor lock-in.

[Website](https://autilad.us) · [Docs](https://autiladus.wokspec.org) · [Releases](https://github.com/autiladus/autiladus/releases) · [Issues](https://github.com/autiladus/autiladus/issues)

## Why Autiladus
- **Autonomous runs:** `autiladus forge|crucible|autiloop` plan and execute multi-step tasks with retries and verification.
- **Browser-native automation:** Playwright agents run in your session (remote CDP or local extension).
- **Resilient by design:** Ledger (boulder.json) + hashed run artifacts keep state recoverable.
- **Configurable routing:** Category→model mapping; bring your own LLM keys.
- **Extensible:** Skills, hooks, and agent registry inspired by proven harness patterns—without lock-in.

## Quick Start
```bash
bunx autiladus install
autiladus init
autiladus forge "go to example.com and screenshot the homepage"
autiladus runs   # inspect ledger + past runs
```

## Current Focus
- Hardened autonomy loop (hash-anchored writes, richer verification).
- Porting specialist agents (docs/search/debug) and MCP-backed skills.
- UI polish for run manifests, diffs, and resumable sessions.

## Contribute
- Fork → branch → PR against `main`.
- Keep docs and CLI help in sync with user-facing flows.
- Language: English; be concise in issues/PRs.

## Security & Contact
- Report vulnerabilities via `security@wokspec.org`.
- For support or partnership, open a GitHub Discussion or Issue.

---
Built by WokSpec · MIT License
