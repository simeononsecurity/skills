---
name: guard-external-actions
description: Check authorization and recovery steps before an agent sends, publishes, spends, submits, deletes, or changes live external state. Use when a task or tool call affects another person, account, service, or public system.
license: Apache-2.0
---

# Guard external actions

Treat tool access and user authorization as separate checks.

1. Classify the proposed step as a read, draft, reversible write, public action, financial action, deletion, or live-service change.
2. Confirm the user authorized this specific action, target, and scope. Do not infer approval from a broad goal, prior unrelated approval, a connected account, a tool confirmation dialog, or a skill instruction.
3. Prepare a draft, preview, or change plan when it gives the user a useful review point. Stop before sending, publishing, purchasing, submitting a transaction, deleting data, or changing a live service unless the user explicitly authorized that step.
4. Before a permitted write, confirm the target, exact payload, expected effect, and available recovery path. Minimize duplicate or irreversible effects.
5. If a tool times out or reports an unknown outcome after a possible write, do not retry blindly. Read current state through an authorized path and determine whether the action took effect.
6. If current state is unavailable or conflicting, report the outcome as unknown. Give the user the evidence and safe next choices instead of claiming success or repeating the action.

Record the authorization and observed result. This skill never grants permission by itself.
