# mcp-scanner · Roadmap

> Cadence: quarterly milestones through 2026. Subject to change as the MCP spec evolves.

## v0.1 · Passive Scan (target: 2026-06)

- [ ] MCP server metadata inspection (manifest, tool list, schema sanity)
- [ ] Tool manifest lint — dangerous patterns (arbitrary-file-write, shell-exec, credential-echo)
- [ ] Static ruleset v1 (10+ rules derived from OWASP LLM Top 10)
- [ ] CLI scaffold
- [ ] Basic JSON report output

## v0.2 · Active Probe (target: 2026-09)

- [ ] Prompt-injection probes against MCP tool metadata
- [ ] Unauthorized tool-chain detection (graph analysis)
- [ ] Credential-leakage probe (entropy + known-pattern detection)
- [ ] Authenticated & unauthenticated probe modes
- [ ] SARIF report export

## v0.3 · Integration (target: 2026-12)

- [ ] GitHub Action
- [ ] GitLab CI template
- [ ] Integration with LangChain / LlamaIndex / Dify / Coze
- [ ] Web UI (optional)

## Beyond 2026

- Fuzzing harness for MCP servers
- Research collaboration with MCP spec authors
- Published paper on Agent/MCP attack surface
