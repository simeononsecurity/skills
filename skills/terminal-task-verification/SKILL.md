---
name: terminal-task-verification
description: Verify a multi-step terminal task against its requested end state and authoritative verifier. Use when a multi-step terminal task needs a defined end-state check.
license: Apache-2.0
---
# Terminal Task Verification

Carry the task from initial evidence to a verified final state. Separate observations, actions, and outcomes so later steps use current evidence rather than assumptions.

Source inspiration: Junyao Yang et al., [Terminal-RSI, arXiv:2610.22192v3](https://arxiv.org/abs/2610.22192v3), 2026-10-30. This skill contains original workflow instructions and reproduces no paper text or training code.

## Establish the task contract

Use the current host's terminal or shell tool. If no suitable interface exists, report that limit and do not claim execution or verification.

- Identify the requested end state, constraints, and the authoritative verifier. Prefer protected tests, explicit acceptance checks, or a user-specified command over self-reported completion.
- Inspect the relevant repository or environment before changing it. Note existing user changes and preserve unrelated work.
- Keep task limits distinct from context limits. A shell session ending, a context summary, or a tool chunk boundary does not mean the task itself ended.

## Work in verifiable increments

- Choose the smallest action likely to advance the requested end state. After each material action, inspect its result before deciding what to do next.
- Record concise, decision-relevant evidence: command or action, observed result, and remaining uncertainty. Avoid copying long logs when a focused excerpt or structured result is enough.
- Treat local checks and intermediate milestones as partial progress. Do not promote them to full completion unless the full task contract passes.
- When a check fails, use its evidence to revise the diagnosis. Avoid repeating an unchanged action without a new reason.
- Respect task termination rules. Do not treat a sampling cutoff, context compaction, or computational partition as a user-requested stop condition.

## Verify the final state

- Run the authoritative verifier against the resulting environment, with the exact target, architecture, configuration, and relevant compatibility conditions in scope.
- Confirm the verifier covers the requested outcome. A passing subset of checks proves only those checks; call out material gaps such as untested architectures, hidden requirements, or unavailable verification.
- Report what changed, which checks passed or failed, and what remains unknown. Never claim success from an agent declaration alone.

## Boundaries

- A task request authorizes only work within its stated scope. Do not infer permission for destructive actions, external publication, deployment, purchases, or unrelated cleanup.
- Do not copy secrets, private harness messages, or environment-specific credentials into reusable notes or runbooks.
- This skill guides execution. It does not implement model training, reward optimization, or automatic policy updates.
