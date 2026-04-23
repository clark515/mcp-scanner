# mcp-scanner

> Security scanner for **MCP (Model Context Protocol)** servers and Agent ecosystems.

![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/status-early--dev-orange)

**Status**: 🚧 Early development · Roadmap stage · Contributions welcome

---

## Why

As MCP becomes the de-facto protocol for Agent ↔ tool integration, a new class of security risks emerges that traditional scanners don't cover:

- **Malicious MCP servers** hijacking Agent behavior via crafted tool manifests
- **Over-permissive tool invocations** leaking secrets or triggering destructive actions
- **Prompt injection through tool metadata** (description, schema, examples)
- **Credential leakage** via tool arguments forwarded to provider APIs
- **Tool-chain attacks** — one tool's output becoming another's malicious input

`mcp-scanner` is a dedicated security audit toolkit for the MCP layer — passive inspection, active probing, and CI/CD integration.

## Quick Start

> Coming in v0.1. Watch the repo to get notified.

```bash
# Planned interface
mcp-scanner inspect --server https://example.com/mcp
mcp-scanner audit   --config ./mcp-config.json
mcp-scanner probe   --target <mcp-endpoint> --ruleset owasp-agent-top10
```

## Features (planned)

- 🔍 **Metadata inspection** — manifest sanity, tool permission lint
- 🕵️ **Prompt-injection probes** — payload library for MCP tool descriptions
- 🧾 **Credential-leakage detection** — patterns & entropy analysis on tool args
- 🔗 **Tool-chain graph analysis** — identify dangerous transitive flows
- 📋 **Report export** — SARIF, HTML, JSON
- 🧩 **CI/CD plugin** — GitHub Action + GitLab CI

See [ROADMAP.md](./ROADMAP.md) for the full plan.

## Related Research

- Model Context Protocol specification — <https://modelcontextprotocol.io>
- OWASP LLM Top 10 — <https://owasp.org/www-project-top-10-for-large-language-model-applications/>
- OWASP Agent Top 10 (draft) — tracking

## Contributing

Issue reports, rule contributions, and research collaborations are welcome. Open an issue or reach out via `lostpoet515 [at] gmail.com`.

## License

MIT © [Clark (clark515)](https://github.com/clark515)
