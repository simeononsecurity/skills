---
name: prepare-agent-handoffs
description: Prepare a concise handoff for an agent resuming work after interruption, context compaction, delegation, or a new session. Use when the next agent needs verified state without replaying the full conversation.
license: Apache-2.0
---

# Prepare agent handoffs

Write the handoff for the next action. Keep source facts, observations, decisions, and proposals distinct.

Include:

- The objective and its current boundary.
- The authoritative files or records, with revision, date, or other stable locator when available.
- The current branch or workspace and the exact paths changed.
- Checks actually run and their observed results.
- Decisions already made, permissions granted for this task, and actions still awaiting authorization.
- Pending work, unresolved conflicts, and the next useful action.

Before resuming, the next agent must reopen the named current sources and inspect the current workspace. If the source revision or live state changed, update the handoff and resolve the conflict before acting. Treat a summary as navigation, not as current authority. Do not paste secrets, credentials, private conversation, or unnecessary user data into a handoff.
