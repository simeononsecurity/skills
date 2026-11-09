---
name: terminal-runbook-refinement
description: Turn verified terminal work into a replayable runbook. Use when extracting a reusable procedure from a task whose authoritative verifier passed.
license: Apache-2.0
---
# Terminal Runbook Refinement

Extract reusable procedures from verified terminal work. Retain only instructions that survive review and a fresh run under the intended target environment.

Source inspiration: Junyao Yang et al., [Terminal-RSI, arXiv:2610.22192v3](https://arxiv.org/abs/2610.22192v3), 2026-10-30. This skill contains original workflow instructions and reproduces no paper text or training code.

## Build from evidence

Use the current host's terminal or shell tool. If no suitable interface exists, report that limit and do not claim execution or verification.

- Start from a completed task whose authoritative verifier passed. If the task failed, record it as an unresolved diagnostic lead, not a proven solution.
- Extract the task contract, prerequisites, decision points, actions, expected observations, recovery limits, and final verifier.
- Preserve the order and multiplicity of verified steps when those affect the result. Label optional branches and environment assumptions.
- Separate public task requirements from private harness instructions, credentials, local secrets, and reviewer discussions. Exclude private material from the runbook.

## Review for fit

- Check the runbook against the intended target environment for required artifacts, compatibility, architecture, configuration, and permissions.
- Keep task-specific values explicit and replace private identifiers with safe placeholders. Do not imply a runbook applies to environments it has not covered.
- Check whether the verifier measures the requested outcome or only a proxy. A runbook that passes narrow checks might still miss untested requirements.
- Preserve useful partial diagnostics when verification fails, but label them as partial and keep them separate from successful procedures.

## Fresh replay

- Before replay, confirm the user authorized terminal execution in the intended target and that the task scope covers the planned changes. Use a disposable, synthetic, or otherwise approved target when available. Do not replay against production or another live system without specific authorization. If no safe authorized target exists, keep the runbook labeled unverified and state the evidence needed for replay.
- Execute the runbook in a fresh target run. Do not count its source trajectory, planner notes, or an agent's completion statement as replay evidence.
- Apply the full task verifier to the replay result. Retain the runbook as verified only when the fresh execution passes.
- If replay fails, compare the fresh observations with the expected results, update the runbook only from supported evidence, and replay again within the user's authorized scope. Stop when the scope or retry limit is reached.
- Keep provenance: task or environment class, verifier result, replay date, and known coverage gaps. Avoid retaining sensitive raw logs when a sanitized summary suffices.

## Boundaries

- Do not silently edit this skill or broader agent policy based on one run. A runbook may be updated within the requested deliverable; changes to reusable skill instructions require the user's request or approval.
- Passing replay establishes evidence only for the tested target and verifier. It does not prove universal compatibility or that every useful behavior was retained.
- Prompt-level runbook review and replay do not reproduce reinforcement learning, critic handoff, reward calibration, or token-level advantage estimation.
