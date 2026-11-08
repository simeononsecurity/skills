---
name: bound-agent-loops
description: Set explicit state checks, retry limits, and stop conditions for an agent repeating work toward a defined task. Use when a task needs more than one attempt or automated retry.
license: Apache-2.0
---

# Bound agent loops

Use this skill for a finite task loop. Do not turn a work loop into a recurring monitor.

1. Define one observable goal, the authoritative input, the files or services in scope, and the baseline state.
2. Write a loop contract with each action, its success check, its retry budget, and immediate stop conditions. Include a human handoff condition.
3. After every action, inspect the actual result and changed state before choosing the next attempt. Record the command or tool call and its output.
4. If a check fails, name a new cause to investigate before retrying. Do not repeat an unchanged prompt or action without evidence of a different cause.
5. Stop at once for conflicting requirements, unexpected scope changes, exposed sensitive data, blocked permissions, uncertain external writes, or a result you cannot verify.
6. Stop when the retry budget ends. Hand off the current state, last verified result, remaining failure, and the decision or evidence needed to continue.

A recurring monitor needs a separate contract with a schedule, exact trigger threshold, notification route, and disable condition. Do not enable a monitor as a side effect of a task loop. External actions still require specific user authorization.
