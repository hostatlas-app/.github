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
live in the open:

- [**mcp-server**](https://github.com/hostatlas-app/mcp-server) — MCP
  gateway giving AI agents live read + safe write access to your
  HostAtlas fleet. 22 tools, 3 resources.
- [**queue-monitor**](https://github.com/hostatlas-app/queue-monitor) —
  Push Redis / Database / SQS queue metrics into your HostAtlas
  dashboard.
- [**homebrew-hostatlas**](https://github.com/hostatlas-app/homebrew-hostatlas) —
  Homebrew tap for the HostAtlas CLI.

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
