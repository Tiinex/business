# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Core](001-core-project.trace.md)
  - Origin:
    - [relative](001-core-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Cross-Repository Coordination Semantics
  - Status: draft/local

---

# Cross-Repository Coordination Semantics

## Objective

Define how Projects, Tasks, Milestones, Schedules, Roles, Resources, Decisions, Handoffs, and relation/permalink references coordinate work across repositories without turning repository layout into semantic hierarchy.

## Done Criteria

- Initiatives can anchor cross-repository work while concrete Tasks remain in natural repositories.
- Direct Parent lineage and organizational/project association are distinguishable.
- Milestone and Schedule semantics can represent outcomes and ordering without becoming task boards or proof of execution.
- Roadmap composition requirements are known before portfolio and per-Initiative schedules are nested.

## Scope

- Do not introduce an Epic schema unless Task semantics prove insufficient.
- Do not force every artifact into Business.
- Do not make Schedule or Project a substitute for evidence, decisions, or execution lineage.

## Dependencies

- Current Project/Task/Milestone/Schedule/Relation/Handoff schemas.
- Business portfolio design and real cross-repository examples.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Core](001-core-project.trace.md)
  - Value: 2_rmvvAEq0llL5ah-e27rJ8AoITWCjGTPMJ-KzEdA_8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: aob0wtsV7mCHPjnJwPUefyuVHPz2_KMbc8IDR3feswQ
