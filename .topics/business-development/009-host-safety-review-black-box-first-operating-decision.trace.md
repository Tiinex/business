# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-27 12:25:00
  - Trace: [Tooling And Workflow Iteration Efficiency](../initiatives/002-6-tooling-workflow-iteration-efficiency-task.trace.md)
  - Origin:
    - [relative](../initiatives/002-6-tooling-workflow-iteration-efficiency-task.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-27 13:23:00
  - Authors: Anchor; Sigma
  - Why: Repeated benign Tiinex development turns showed a large difference between useful black-box Tooling runtime and host-observed wall-clock when additional safety review appeared, so future roles need a durable efficiency rule that avoids unnecessary source/runtime inspection without attempting to bypass host safety policy.
  - Summary: Adopt black-box-first Tiinex operation, bounded source inspection, focused validation, and explicit latency attribution as the default cross-role efficiency practice while preserving all host safety checks and required qualification gates.
  - Status: accepted/local

---

# Host Safety Review And Black-Box-First Operating Guidance

## Decision

- State: accepted
- Subject: cross-role Tiinex operating behavior when routine work can be completed through portable Tooling without source/runtime inspection
- Decision: Anchor, Axiom, Loom, Sigma-assisted workflows, and future Tiinex roles should use qualified black-box Tiinex operations first when those operations can answer the current question or complete the bounded task. Source-code inspection, runtime archaeology, and focused implementation tests should be entered only when a concrete defect, implementation change, or qualification gap requires them. This is an efficiency and provenance rule, not a safety-evasion rule: host safety checks remain intact, required validation must still run, and wording or execution must not be altered merely to avoid classification.

## Basis

- A comparable Anchor commit-gate audit using black-box Tooling only completed with ChatGPT reporting `Worked for 1m 41s`, while earlier otherwise similar Tiinex turns that entered source/runtime inspection repeatedly experienced roughly 20–30 minute user-visible wall-clock and an additional safety-check notice.
- In the 1m 41s baseline, the measured CLI operations themselves were approximately 0.4 seconds for Business audit, 1.0 second for Docs audit, 1.5 seconds for Site audit, and about 0.3 seconds per Business lineage search.
- In observed safety-review cases, cold-start, Handoff qualification, workspace materialization, and broad audit had already completed before the safety notice appeared. The notice correlated more closely with later source/runtime inspection or focused implementation-test activity, including work around portable lineage implementation. This is correlation evidence, not proof of the host classifier trigger.
- The work is benign provenance, lineage, developer-tooling, and human/LLM interoperability engineering. No decision is made to bypass, suppress, disguise, or defeat host safety systems.
- [Black-box baseline screenshot](assets/009-1-black-box-baseline-1m41.png) preserves Sigma's observed `Worked for 1m 41s` comparison point.
- [Safety-review timing screenshot](assets/009-2-safety-review-near-source-test.png) preserves an observed case where the additional-check path appeared after substantial normal work and near source/test activity.

## Operating Consequences

- Portable Discovery, lineage search/resolution, schema resolution, validation, audit, Handoff orientation, and other qualified Tooling surfaces are the default interface when they are sufficient.
- Do not inspect Tooling implementation merely to reassure oneself that the black-box result is correct. Inspect source when a result is inconsistent, a bounded defect must be repaired, an implementation artifact is the work product, or qualification explicitly requires implementation evidence.
- Prefer focused validation/tests for the changed semantic surface during ordinary iteration. Run broader suites at integration, stabilization, release, or other explicit gates where their broader cost is justified.
- When source/runtime inspection is required, keep it bounded to the owning surface and preserve why the deeper inspection was necessary.
- Record useful timing evidence separately from host wall-clock. Distinguish Tooling execution, test execution, Handoff manufacture, model/host overhead, visible additional safety review, and unknown time instead of treating the host `Worked for` value as Tooling runtime.
- Additional safety review is never treated as an error merely because it adds latency. Roles must not attempt prompt wording tricks, file disguises, test suppression, disabled checks, or other classifier-avoidance behavior.
- If a human stops a long-running host turn because the delay is operationally expensive, durable lineage/Handoff/checkpoint state should make the work recoverable without reconstructing the conversation from memory.
- Delegated parallel work should prefer minimal qualified Handoff closure where appropriate, while Anchor retains the full-source integration context required for reconciliation and merge qualification.
- After the first Git durability checkpoint, historical working-set reduction may be tested as an explicit performance experiment. Compare package size, artifact count, operation timing, observed safety-check frequency, and wall-clock before and after; do not claim causal improvement without evidence.

## Cross-Role Applicability

- Practitioner baseline: meaningful friction in the human or LLM workflow is product evidence and should be surfaced when it suggests a repeatable improvement.
- Anchor: prefer Tooling-level architectural evidence before implementation archaeology; require deeper inspection only when integration or defect diagnosis warrants it.
- Axiom: resolve schema contracts and semantic authority through qualified schema surfaces before inspecting implementation details unrelated to the semantic question.
- Loom: use focused source/test work when implementing or diagnosing Tooling, and avoid broad unrelated source scans or suites during bounded repairs.
- Sigma: human observations of delay, ergonomics, screenshots, stop decisions, and acceptance remain first-class provenance inputs rather than being reduced to AI-only conclusions.

## Review Conditions

- Revisit this guidance if measured evidence shows that black-box-first operation misses necessary defects, materially weakens qualification, or does not improve iteration cost.
- Revisit attribution hypotheses if safety-review notices occur consistently during transport/bootstrap alone, or if source/runtime work no longer correlates with the observed delays.
- This Decision does not define host policy, claim access to internal safety-classifier state, or prove the reason for any individual additional safety check.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tooling And Workflow Iteration Efficiency](../initiatives/002-6-tooling-workflow-iteration-efficiency-task.trace.md)
  - Value: o0aXOVASCLNdE-yQ_hmWtcMSRtJh6QlukqgPotWamm8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:QZ5z145PHaXbQuN_cYgJWbTmCBB6oh8ohfCKpvVvShI
