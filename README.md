# SimeonOnSecurity Skills

A small collection of practical workflows for coding agents. The first release focuses on task scope, evidence-based verification, and bounded delegation.

## Skills

| Skill | Use it when | Outcome |
| --- | --- | --- |
| [scope-agent-task](skills/scope-agent-task/SKILL.md) | An agent needs to change an existing repository | A bounded task, understood project rules, and observable completion checks |
| [verify-agent-work](skills/verify-agent-work/SKILL.md) | An agent reports research, code, or operational results | A claim-by-claim evidence check with unresolved items stated |
| [delegate-bounded-work](skills/delegate-bounded-work/SKILL.md) | Independent work can proceed in parallel | Clear ownership, reviewable reports, and accountable integration |

## Format and use

Each skill follows the [Agent Skills format](https://agentskills.io/specification): one folder with a `SKILL.md` file, YAML metadata, and Markdown instructions. `agents/openai.yaml` supplies optional Codex interface labels. The instructions do not require a particular provider or MCP server. Host discovery and install locations differ. Use your agent's current documentation to install a skill folder, then restart or refresh discovery if the host requires it.

The skills were prepared for hosts that support the Agent Skills format. They have not been exercised in every Codex, Claude, Hermes, or OpenCode version. Treat host-specific invocation behavior as unverified.

## Scope

These skills guide local research, repository work, and review. They do not authorize contacting people, publishing, deploying, spending money, deleting data, or changing live services. Follow the user's request and the host's permissions for each task.

## Contributions

Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing a change. See [the catalog and selection notes](docs/catalog.md) and [provenance and licensing](docs/provenance-and-licensing.md) for source details.
