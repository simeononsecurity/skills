# First-release catalog

The collection follows an agent-work lifecycle: scope the task, retrieve and verify evidence, act within authorization, manage retries and continuity, and evaluate persistent tools or agents. Each skill has one trigger and a distinct result.

| Priority | Skill | Audience and trigger | Practical outcome | Evidence and reason |
| --- | --- | --- | --- | --- |
| 1 | [scope-agent-task](../skills/scope-agent-task/SKILL.md) | People using an agent to change an existing project | A bounded task, local rules, preserved work, and completion checks | The [Effective AI Workflow course](https://simeononsecurity.com/effective-ai-course-start/) teaches task packets, repository context, and coding-agent work. This is the common starting point. |
| 1 | [verify-agent-work](../skills/verify-agent-work/SKILL.md) | People reviewing agent research, code, or operational reports | Claims tied to sources or executed checks, with uncertainty labeled | The course's capstone requires source, diff, test, privacy, and cost evidence. The site writing workflow separates observed, measured, estimated, and recommended claims. |
| 1 | [delegate-bounded-work](../skills/delegate-bounded-work/SKILL.md) | People coordinating multiple agents | Disjoint assignments, structured reports, and verified integration | The course delegation lesson and [AI Collaboration course](https://simeononsecurity.com/ai-collaboration-course-start/) document independent work and review. |
| 1 | [bound-agent-loops](../skills/bound-agent-loops/SKILL.md) | People running iterative agent tasks | A finite contract with state checks, retry budget, stop rules, and a handoff | [Bounded AI Agent Loops](https://simeononsecurity.com/articles/effective-ai-bounded-agent-loops/) explains retry contracts, new-cause checks, and stopping on ambiguous external outcomes. This adds retry behavior absent from the first three skills. |
| 1 | [prepare-agent-handoffs](../skills/prepare-agent-handoffs/SKILL.md) | People resuming work after context compaction, interruption, or delegation | A short record of current sources, observed state, decisions, checks, and next steps | [AI Context Window Management](https://simeononsecurity.com/articles/effective-ai-context-window-management/) and [Drift Recovery and Handoff Workflow](https://simeononsecurity.com/articles/ai-collaboration-drift-recovery-handoffs/) teach fresh-source checks and verified handoffs. |
| 1 | [guard-external-actions](../skills/guard-external-actions/SKILL.md) | People using tools that send, publish, spend, submit, delete, or change live state | A specific authorization check and a safe recovery path after uncertain results | The bounded-loop and drift-recovery articles identify duplicate actions and interrupted publication as distinct risks. The skill makes the approval boundary explicit. |
| 2 | [evaluate-persistent-agents](../skills/evaluate-persistent-agents/SKILL.md) | People considering scheduled or always-on agents | A limited pilot decision covering trigger, access, delivery, and shutdown | [Specialized Agent Evaluation](https://simeononsecurity.com/articles/effective-ai-specialized-agent-evaluation/) specifies access, trigger, environment, and pilot checks. |
| 2 | [verify-tool-connections](../skills/verify-tool-connections/SKILL.md) | People configuring MCP or another connected tool | Separate proof for configuration, connection, discovery, execution, and output | [MCP Server Setup](https://simeononsecurity.com/articles/effective-ai-mcp-server-setup/) shows why configuration alone does not prove a tool call worked. |
| 2 | [retrieve-authoritative-sources](../skills/retrieve-authoritative-sources/SKILL.md) | People searching across maps, documents, or retrieval systems | A current authorized record, revision, exception, and explicit conflict status | [AI Source Retrieval](https://simeononsecurity.com/articles/ai-collaboration-map-first-retrieval/) distinguishes discovery maps and summaries from the authoritative source, with access checks. |

## Why these belong together

The first three skills cover task scope, evidence, and delegation. The added skills fill gaps visible in actual workflows: retries need a finite contract, long work needs a fresh-source handoff, external mutations need specific authorization and recovery, and connected or persistent agents need permission and delivery checks. Retrieval needs a current source and access check before an answer is trusted.

## Deferred candidates

- Repository-context authoring overlaps repository inspection and rule loading in `scope-agent-task`. Revisit if users ask for a standalone instructions-file workflow.
- Site article, media, Hugo, course, and browser-tool skills are proven but depend on one publishing repository and its scripts. Keep them in that site's skill set.
- Fleet, commerce, email, and account-specific procedures need separate privacy and product-scope review. They are outside this general collection.
- Third-party methodologies remain separate installs. See [provenance and licensing](provenance-and-licensing.md).
