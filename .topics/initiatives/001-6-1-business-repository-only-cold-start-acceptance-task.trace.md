# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-29 01:20:00
  - Trace: [Foundation Readiness And Operating Reconciliation](001-6-foundation-readiness-operating-reconciliation-task.trace.md)
  - Origin:
    - [relative](001-6-foundation-readiness-operating-reconciliation-task.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-29 10:32:00
  - Authors: Anchor; Sigma
  - Why: Make Business semantic self-sufficiency independently testable instead of allowing Handoff, bootstrap, role pre-context, or conversation memory to hide missing organizational truth.
  - Summary: Business Repository-Only Cold-Start Acceptance
  - Status: draft/local

---

# Business Repository-Only Cold-Start Acceptance

## Objective

Prove that a generic LLM receiving only the current `Tiinex/business` repository — as if a person simply linked the repository into a fresh isolated project — can understand and describe Tiinex materially as truthfully, cautiously, and usefully as a correctly cold-started Anchor for organizational questions.

## Done Criteria

- The test starts with no Tiinex pre-context, no Anchor role prompt, no prior conversation, no Handoff supplied out of band, and **no Handoff package**.
- The model receives only the current Business repository and may use the files naturally discoverable inside that repository, including `.topics`, README, and `llms.txt` when present.
- Semantic understanding does not require Tooling bootstrap. Bootstrap is a separate operational capability; Handoff is a separate precise-continuation capability.
- From the repository alone, the model can explain: what Tiinex is; the problem it addresses; who the current evidenced audience is; what Tiinex is not; Core/Tooling/Viewer/Business boundaries; the current Foundation state; what the PoC does and does not prove; the Role/operating model; current priorities; external obligations; known resources; financing limits; and material unknowns.
- The model does not invent legal-company status, employees/headcount, budget/runway, production readiness, commercial positioning, roadmap, or schema/runtime completeness when Business does not establish them.
- The model can answer reasonable unexpected organizational questions by following current Business provenance instead of relying only on a memorized FAQ or one scripted prompt.
- The first-contact path remains usable through ordinary repository/web/LLM surfaces, including a mobile-first review. A local checkout, terminal, IDE, or remote PC must not be necessary merely to understand current organizational truth, priorities, blockers, or unknowns.
- Remote PC/local technical access is treated as escalation for implementation, Tooling execution, or deep source inspection rather than as a hidden prerequisite for executive operation.
- Material parity with a correctly cold-started Anchor means the important facts, authority boundaries, current-vs-unknown distinctions, and priority picture agree even when wording differs.
- A failure is repaired in Business authority or its first-contact projection when appropriate; it is not hidden by adding secret test-specific prompting to the isolated model.
- Final acceptance is based on Sigma-run isolated cold-start projects where the model receives the repository without prior Tiinex context.

## Scope

- This is a semantic/organizational cold-start gate, not a test that the model can execute Tiinex Tooling, mutate repositories, or continue a specific prior session.
- The model may read all current Business material but must not need external repositories to answer the core organizational questions above.
- External links may provide deeper evidence or operational continuation, but absence of external access must not make the Business identity, current state, or declared unknowns unintelligible.
- Do not optimize only for a fixed question list; test whether the repository carries enough bounded truth for novel questions.
- Mobile usability is an operating-quality condition, not a claim that every technical action should be performed from a phone.

## Dependencies

- [Foundation Readiness And Operating Reconciliation](001-6-foundation-readiness-operating-reconciliation-task.trace.md)
- [Tiinex Executive Grounding](../executive/001-executive-grounding.trace.md)
- [Repository LLM Cold-Start And Bootstrap Surface](001-8-1-repository-llm-cold-start-and-bootstrap-surface-task.trace.md)
- Current Business organization, Initiatives, Roles, financing, challenge, and public-surface artifacts.
- Sigma for the final isolated-project quality test.

## Evaluation Boundary

Three capabilities must remain distinct:

1. **Business repository only** — enough semantic truth to understand Tiinex and speak cautiously about the organization.
2. **Operational bootstrap** — enough qualified Tooling guidance to perform Tiinex operations safely when needed.
3. **Handoff / Handoff package** — enough explicit continuation state to resume one particular prior work boundary precisely.

Passing one does not imply the others, and none should be used to mask missing truth in another layer.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Foundation Readiness And Operating Reconciliation](001-6-foundation-readiness-operating-reconciliation-task.trace.md)
  - Value: iU8sDCJZpdCBP_MB6Rxk8InamgZBvbZXQnRPgy1dPM0

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:jMnkDwuaxJa8HCxHGFjWlyBw-LqBTSuzSDHOqTEZdXw
