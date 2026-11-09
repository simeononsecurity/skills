# Provenance and licensing

## Original skills

All eleven skills use original wording and include no copied third-party scripts or skill text. Most generalize public SimeonOnSecurity workflows. The two terminal skills also cite Terminal-RSI as conceptual inspiration; the source for each skill appears in the table:

| Skill | Source | Supported idea | Confidence |
| --- | --- | --- | --- |
| `scope-agent-task` | [Effective AI Workflow course](https://simeononsecurity.com/effective-ai-course-start/) | Task packets, repository context, coding-agent work, and acceptance evidence | High |
| `verify-agent-work` | [Effective AI Workflow course](https://simeononsecurity.com/effective-ai-course-start/) and the site's published writing workflow | Separate claims from evidence and record source, diff, test, privacy, and cost checks | High |
| `delegate-bounded-work` | [Effective AI Workflow course](https://simeononsecurity.com/effective-ai-course-start/) and [AI Collaboration course](https://simeononsecurity.com/ai-collaboration-course-start/) | Assign independent work, collect reviewer evidence, integrate, and hand off | High |
| `bound-agent-loops` | [Bounded AI Agent Loops](https://simeononsecurity.com/articles/effective-ai-bounded-agent-loops/) | Define observable state, retry budgets, new-cause checks, immediate stops, and a human handoff | High |
| `prepare-agent-handoffs` | [AI Context Window Management](https://simeononsecurity.com/articles/effective-ai-context-window-management/) and [Drift Recovery and Handoff Workflow](https://simeononsecurity.com/articles/ai-collaboration-drift-recovery-handoffs/) | Preserve verified state across sessions and reopen current sources before resuming | High |
| `guard-external-actions` | [Bounded AI Agent Loops](https://simeononsecurity.com/articles/effective-ai-bounded-agent-loops/) and [Drift Recovery and Handoff Workflow](https://simeononsecurity.com/articles/ai-collaboration-drift-recovery-handoffs/) | Require explicit authorization and inspect live state before retrying an uncertain external write | High |
| `evaluate-persistent-agents` | [Specialized Agent Evaluation](https://simeononsecurity.com/articles/effective-ai-specialized-agent-evaluation/) | Review scope, permissions, trigger conditions, pilot evidence, and delivery before enabling a persistent agent | High |
| `verify-tool-connections` | [MCP Server Setup](https://simeononsecurity.com/articles/effective-ai-mcp-server-setup/) | Distinguish configured, connected, discovered, executed, and verified states | High |
| `retrieve-authoritative-sources` | [AI Source Retrieval](https://simeononsecurity.com/articles/ai-collaboration-map-first-retrieval/) | Treat maps and indexes as pointers, then verify current authority, revision, access, and exceptions | High |
| `terminal-task-verification` | Junyao Yang et al., [Terminal-RSI, arXiv:2610.22192v3](https://arxiv.org/abs/2610.22192v3) | Separate intermediate progress from protected-verifier completion in terminal work | High |
| `terminal-runbook-refinement` | Junyao Yang et al., [Terminal-RSI, arXiv:2610.22192v3](https://arxiv.org/abs/2610.22192v3) | Retain verified procedures only after compatibility review and fresh replay | High |


Full citation: Junyao Yang, Zongxia Li, Yucheng Shi, Zhongzhi Li, Ruhan Wang, Ruiwen Zhou, Haitao Mi, Shuicheng Yan, and Leowei Liang. “Terminal-RSI: Recursive Self-Improving Terminal Agents via Recursive Self-Rewrite and Policy-Refine.” arXiv:2610.22192v3, 2026-10-30. [Paper](https://arxiv.org/abs/2610.22192v3).

The two terminal skills use original wording and procedures. They adapt the high-level ideas of protected-verifier completion and fresh replay. They include no paper text, benchmark data, or training code.

The skills generalize those ideas. They do not include site-specific commands, private infrastructure, customer information, or unpublished conversation text.

## License choice

Original files in this repository use Apache License 2.0. The Agent Skills specification supports a `license` field. Apache-2.0 is a permissive license with an express patent grant. See the [full license](../LICENSE) and the [Apache Software Foundation license text](https://www.apache.org/licenses/LICENSE-2.0.txt).

Every skill repeats `license: Apache-2.0` in its frontmatter. A future third-party package must keep its own license and notices. Do not assume a repository-level license applies to separately licensed files.

## External skills to install from their authors

These are recommendations, not included files.

### obra/superpowers

A broad coding-agent development methodology with skills for planning, implementation, and review. Its repository identifies an MIT license and documents multiple agent hosts. Install it using the instructions for your host in the [canonical repository](https://github.com/obra/superpowers). For OpenCode, use its [OpenCode installation guide](https://github.com/obra/superpowers/blob/main/docs/README.opencode.md). Do not copy its plugin or skill files into this repository.

### Anthropic `mcp-builder`

A focused option when you are building an MCP server. The [canonical skill folder](https://github.com/anthropics/skills/tree/main/skills/mcp-builder) includes a `LICENSE.txt`; the current file identifies Apache-2.0. To install the skill as a folder, clone the upstream repository and copy `skills/mcp-builder` into a skill directory supported by your host. Keep its `LICENSE.txt` with the skill. Review the current upstream instructions before installing because host support can change.

## Evidence ledger

Checked 2026-11-08. Confidence describes how directly the source supports the stated fact.

| Source | Date or version | Finding | Confidence |
| --- | --- | --- | --- |
| [Agent Skills specification](https://agentskills.io/specification) | Accessed 2026-11-08 | A skill needs a directory with `SKILL.md`; `name` and `description` are required. `license` and `compatibility` are optional fields. | High |
| [Agent Skills home](https://agentskills.io/) | Accessed 2026-11-08 | The format supports discovery through concise metadata and progressive loading of instructions and resources. | High |
| [obra/superpowers README](https://github.com/obra/superpowers) and [license](https://github.com/obra/superpowers/blob/main/LICENSE) | `main`, accessed 2026-11-08 | The project describes a multi-skill coding workflow and identifies MIT licensing. | High |
| [Superpowers OpenCode guide](https://github.com/obra/superpowers/blob/main/docs/README.opencode.md) | `main`, accessed 2026-11-08 | The upstream documents OpenCode plugin setup and version-specific configuration. | High |
| [Anthropic skills README](https://github.com/anthropics/skills/blob/main/README.md), [`mcp-builder` entrypoint](https://github.com/anthropics/skills/blob/main/skills/mcp-builder/SKILL.md), and its [`LICENSE.txt`](https://github.com/anthropics/skills/blob/main/skills/mcp-builder/LICENSE.txt) | `main`, accessed 2026-11-08 | Anthropic presents skills as self-contained folders. The current `mcp-builder` file refers to its bundled license, which identifies Apache-2.0. | High |
| [Bounded AI Agent Loops](https://simeononsecurity.com/articles/effective-ai-bounded-agent-loops/), [AI Context Window Management](https://simeononsecurity.com/articles/effective-ai-context-window-management/), and [Drift Recovery and Handoff Workflow](https://simeononsecurity.com/articles/ai-collaboration-drift-recovery-handoffs/) | Published source pages, accessed 2026-11-08 | Current public workflows for bounded retries, verified handoffs, and recovery after ambiguous writes. | High |
| [Specialized Agent Evaluation](https://simeononsecurity.com/articles/effective-ai-specialized-agent-evaluation/), [MCP Server Setup](https://simeononsecurity.com/articles/effective-ai-mcp-server-setup/), and [AI Source Retrieval](https://simeononsecurity.com/articles/ai-collaboration-map-first-retrieval/) | Published source pages, accessed 2026-11-08 | Current public workflows for persistent-agent pilots, tool-connection proof, and source authority checks. | High |
| [Terminal-RSI, arXiv:2610.22192v3](https://arxiv.org/abs/2610.22192v3) | v3, dated 2026-10-30; accessed 2026-11-08 | Source for the two terminal workflow ideas. The skills use original wording and include no paper text or training code. | High |
| [arXiv license information](https://info.arxiv.org/help/license/) | Accessed 2026-11-08 | arXiv says submitters choose a license and different versions may have different licenses. The specific v3 license was not exposed by the accessible page extraction, so this work does not claim permission to redistribute paper content. | High for policy, unverified for this version |
| [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt) | Version 2.0, January 2004 | Primary license text used for this repository's original files. | High |

## Research limits

The external skill and format references above were checked on 2026-11-08. Upstream branches, licenses, and host installation procedures can change. Confirm the current license and installation guide before adopting a third-party skill.
