# First-release catalog

The first release includes three workflows. They cover the request-to-change loop: define a bounded task, verify the result, then coordinate independent work when needed.

| Priority | Skill | Audience | Trigger | Practical outcome | Evidence and selection reason |
| --- | --- | --- | --- | --- | --- |
| 1 | [scope-agent-task](../skills/scope-agent-task/SKILL.md) | People using a coding agent in an existing project | The agent must inspect project instructions or make repository edits | A bounded task packet, understood local rules, preserved existing work, and completion checks | The [Effective AI Workflow course](https://simeononsecurity.com/effective-ai-course-start/) teaches task packets, repository context, coding-agent work, and a capstone with observable evidence. This skill joins those steps into the most common starting workflow. |
| 2 | [verify-agent-work](../skills/verify-agent-work/SKILL.md) | People reviewing agent-written research, code, or operational reports | A result includes claims that affect a decision or handoff | Claims linked to sources or executed checks, with uncertainty labeled | The course defines source, diff, test, privacy, and cost evidence. The site article workflow distinguishes observed, measured, estimated, and recommended claims. This transfers that verification discipline beyond article work. |
| 3 | [delegate-bounded-work](../skills/delegate-bounded-work/SKILL.md) | People coordinating multiple agents | Independent subtasks can proceed with clear ownership | Disjoint assignments, structured reports, and a verified integration | The course's independent-worker lesson and the site's reviewer workflow specify separate scopes, review evidence, and integration. The skill keeps delegation optional and bounded. |

## Deferred candidates

- Repository-context authoring has strong source evidence, but overlaps the repository inspection and rule-loading work in `scope-agent-task`. Revisit if users need a standalone project-instructions workflow.
- Site article, media, Hugo, course, and browser-tool skills are proven but depend on one publishing repository and its scripts. Keep them in that site's existing skill set.
- Fleet, commerce, email, and account-specific workflows need a separate privacy and product-scope review. They are not part of this general first release.
- Third-party methodologies remain separate installs. See [provenance and licensing](provenance-and-licensing.md).
