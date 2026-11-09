# SimeonOnSecurity Skills

A practical workflow collection for coding agents. It covers task scope, authoritative source retrieval, evidence checks, delegation, bounded retries, session handoffs, external-action boundaries, persistent agents and connected tools, plus terminal task verification and runbook refinement.

## Skills

| Skill | Use it when | Outcome |
| --- | --- | --- |
| [scope-agent-task](skills/scope-agent-task/SKILL.md) | An agent needs to change an existing repository | A bounded task, understood project rules, and observable completion checks |
| [verify-agent-work](skills/verify-agent-work/SKILL.md) | An agent reports research, code, or operational results | A claim-by-claim evidence check with unresolved items stated |
| [delegate-bounded-work](skills/delegate-bounded-work/SKILL.md) | Independent work can proceed in parallel | Clear ownership, reviewable reports, and accountable integration |
| [bound-agent-loops](skills/bound-agent-loops/SKILL.md) | A task needs retries or repeated checks | A finite loop with observed state, retry limits, and stop conditions |
| [prepare-agent-handoffs](skills/prepare-agent-handoffs/SKILL.md) | Work resumes after interruption or a new session | A concise handoff grounded in current sources and verified state |
| [guard-external-actions](skills/guard-external-actions/SKILL.md) | A tool call affects people, money, public content, or live services | A specific authorization check and a recovery path for uncertain outcomes |
| [evaluate-persistent-agents](skills/evaluate-persistent-agents/SKILL.md) | An agent will run on a schedule or without a live request | A scoped pilot decision covering access, triggers, delivery, and shutdown |
| [verify-tool-connections](skills/verify-tool-connections/SKILL.md) | A new MCP or connected tool appears configured | Evidence for permission, discovery, execution, and verified output |
| [retrieve-authoritative-sources](skills/retrieve-authoritative-sources/SKILL.md) | Search or retrieval results might be stale or conflict | A current, authorized source record with conflicts and limits exposed |
| [terminal-task-verification](skills/terminal-task-verification/SKILL.md) | An agent performs a multi-step terminal task | An authoritative end-state check with partial progress separated from completion |
| [terminal-runbook-refinement](skills/terminal-runbook-refinement/SKILL.md) | A verified terminal task should become reusable | A runbook replayed in a fresh target environment, with gaps recorded |

## Format and use

Each skill follows the [Agent Skills format](https://agentskills.io/specification): one folder with a `SKILL.md` file, YAML metadata, and Markdown instructions. `agents/openai.yaml` supplies optional Codex interface labels. The instructions do not require a particular provider or MCP server. Host discovery and install locations differ. Use your agent's current documentation to install a skill folder, then restart or refresh discovery if the host requires it.

The skills were prepared for hosts that support the Agent Skills format. They have not been exercised in every Codex, Claude, Hermes, or OpenCode version. Treat host-specific invocation behavior as unverified.

## Scope

These skills guide local research, repository work, and review. They do not authorize contacting people, publishing, deploying, spending money, deleting data, or changing live services. Follow the user's request and the host's permissions for each task.

## Contributions

Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing a change. See [the catalog and selection notes](docs/catalog.md) and [provenance and licensing](docs/provenance-and-licensing.md) for source details.
