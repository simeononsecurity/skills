---
name: evaluate-persistent-agents
description: Evaluate a recurring, scheduled, or always-on agent before enabling it. Use when an agent will retain access, wake on a trigger, or act without a live request.
license: Apache-2.0
---

# Evaluate persistent agents

Prepare a reviewable pilot decision before enabling a persistent agent or recurring trigger.

1. Define the job, owner, data sources, exact trigger condition, schedule, and what counts as a wrong result. Separate event-driven work from periodic checks.
2. Inventory the agent's account access, tools, data flow, storage, retention, logs, and external write capabilities. Verify actual permissions in the host and connected services.
3. Limit the pilot to the smallest useful scope. Prefer synthetic or non-sensitive data, read-only access, and manual triggering until the workflow passes its checks.
4. Define duplicate handling, failure behavior, retry limits, notification destination, silence conditions, stop rule, and a way to disable the agent.
5. Test the trigger, no-trigger case, denied-access case, delivery path, and recovery steps. Confirm the user receives an alert when the defined condition occurs.
6. Record evidence and recommend accept, revise, or reject. Do not enable schedules, broaden access, or authorize external actions without the user's specific approval.

A working prompt or successful one-time run does not prove a persistent agent is safe or useful. Review the full trigger-to-delivery path.
