---
name: verify-agent-work
description: Verify an agent's research, code, or operational result before relying on or handing it off. Use when a result needs evidence beyond the agent's summary.
license: Apache-2.0
---

# Verify agent work

Check the result itself. Treat a completion message as a lead to evidence, not as evidence.

1. List the material claims, changed paths, commands, sources, or external actions in the report.
2. Classify each important claim as observed, measured, calculated, source-reported, inferred, recommended, or unverified. Keep estimates and expectations distinct from observed results.
3. For source-based claims, open the cited primary source and confirm it supports the exact statement. Check dates, versions, redirects, and relevant context when behavior changes over time.
4. For code changes, inspect the diff and nearby code. Run only the checks required by the user, repository instructions, or the task's acceptance criteria. Record the exact command and outcome. An exit code alone does not prove the output is correct.
5. For live or external state, use a current authorized read path. Do not infer a successful mutation from a draft, request, queued job, or stale report.
6. Compare the result with the requested scope. Confirm unrelated files stayed untouched and that no secret, personal data, or private system detail entered the deliverable.
7. Return a short evidence table with claim or artifact, evidence checked, status, and any correction needed. Mark unresolved claims explicitly.

Do not say you ran a check unless you ran it. If a tool or source is unavailable, state what remains unverified and what evidence would resolve it.
