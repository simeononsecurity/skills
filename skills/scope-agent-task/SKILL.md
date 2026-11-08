---
name: scope-agent-task
description: Scope a coding-agent task before repository edits. Use when an agent must change files in an existing project with local instructions, existing work, or multiple possible outcomes.
license: Apache-2.0
---

# Scope an agent task

Before editing, turn the request into a bounded task packet and inspect the repository's own rules.

1. State the requested outcome, affected paths, required deliverables, and observable completion checks. Preserve the user's wording when it defines an important boundary.
2. Find the repository root and read its agent bootstrap files. Follow their canonical source of instructions. Read every rule that applies to the task.
3. Inspect the current branch and working tree. Identify changes in the files you might touch. Preserve unrelated work and do not assume uncommitted changes belong to you.
4. Check that the requested tools, dependencies, credentials, and access exist before relying on them. Mark missing access as a limit, not as a completed step.
5. Separate reversible local work from actions that contact people, publish, deploy, spend money, delete data, or change a live service. Perform external actions only when the user authorized that specific action.
6. If the request contains independent workstreams, define disjoint file or research ownership and a compact handoff format before assigning work. Keep the lead agent responsible for integration and final checks.
7. Make the smallest change that satisfies the request. Keep temporary output outside the repository unless the project says otherwise.
8. Verify the changed files against the stated checks and applicable project rules. Report the paths changed, checks completed, and any unresolved limits.

Ask for clarification only when a missing decision materially changes scope, correctness, or authorization. Continue independent work while waiting.
