# HostAtlas

> Server monitoring + audit for teams who actually run their own infrastructure.

HostAtlas is a hosted infrastructure observability platform — live
metrics, plan-aware alerts, scheduled audits, and on-demand forensics
for fleets from one VPS to a few hundred hosts. Operated by
**HostAtlas Technologies LLC**, currently in private beta.

## What it does

- **Live fleet visibility** — servers, containers, databases, domains,
  SSL certs, scheduled jobs, backups.
- **Audit + recipes** — periodic config audits surface security and
  performance issues; safe one-click remediation via signed agent
  commands.
- **Alerts that aren't noise** — per-server thresholds, multi-channel
  notifications (Slack, Telegram, Discord, webhook), incident handoff
  workflow.
- **Diagnostic captures** — on-demand CPU + DB forensics when a host
  misbehaves; samples top processes and slow queries on the live fleet.
- **Agent-friendly** — MCP server for Claude Code, Cursor, Windsurf and
  other agents to query the live state with permissioned tools.

Marketing site + product details at
[hostatlas.app](https://hostatlas.app).

## Public repositories here

Most of HostAtlas itself is closed-source, but a few integration pieces
live in the open. This list refreshes automatically from the GitHub API:

<!-- REPO_LIST_START -->
- [**homebrew-hostatlas**](https://github.com/hostatlas-app/homebrew-hostatlas) — Homebrew tap for HostAtlas CLI — infrastructure monitoring from your terminal
- [**mcp-server**](https://github.com/hostatlas-app/mcp-server) — MCP server for HostAtlas infrastructure monitoring. 22 tools for managing servers, alerts, incidents, domains, backups, and attack mode. 3 resources for real-time context. Works with Claude Code, Cursor, Windsurf. Auto-config from CLI login
- [**queue-monitor**](https://github.com/hostatlas-app/queue-monitor) — Laravel package to push queue metrics (Redis, Database, SQS) to HostAtlas. Auto-detects queues, tracks size, failed jobs, processing count, and workers. Supports Laravel, BullMQ, Sidekiq, and Celery. One command: php artisan hostatlas:queue-metrics.
<!-- REPO_LIST_END -->

## Free open-source tools

We also publish a set of free, MIT-licensed CLI tools at
[hostatlas-labs](https://github.com/hostatlas-labs) — Sentinel,
AtlasMap, DockerTop, PortWatch. Single binary, no signup, no telemetry.

```bash
curl -fsSL https://tools.hostatlas.app/install.sh | sh -s sentinel
```

## Contact

- **Product:** [hostatlas.app](https://hostatlas.app)
- **Support:** [hello@hostatlas.app](mailto:hello@hostatlas.app)
- **Issues:** per-repo within this org

---

**HostAtlas** is operated by **HostAtlas Technologies LLC**, an
[Akyros Labs](https://akyroslabs.com) brand.  
[www.hostatlas.app](https://hostatlas.app) · [hello@hostatlas.app](mailto:hello@hostatlas.app)
