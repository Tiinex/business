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
  - Summary: Process Artifact And Execution Semantics
  - Status: draft/local

---

# Process Artifact And Execution Semantics

## Objective

Resolve a reusable Process model in which a Process definition can point to real artifact/lineage steps, actual runs preserve what happened, and multiple roles can follow the same process without duplicating instructions.

## Done Criteria

- Process definition versus execution/run semantics are explicit.
- Step ordering, optional/conditional/repeat/parallel behavior is representable without hiding state.
- Actual work artifacts can reference Process/step membership without corrupting natural Parent lineage.
- Deviation and observed behavior can feed later Process revisions through evidence.

## Scope

- Defer final schema authoring until real artifact sequences provide enough evidence.
- Do not encode role authority inside Process merely because a role commonly executes it.
- Do not make static Process definition the Parent of every execution artifact by default.

## Dependencies

- Historical Process semantic feedback.
- Business Development repeatable-process epic.
- Real completed artifact sequences.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Core](001-core-project.trace.md)
  - Value: 2_rmvvAEq0llL5ah-e27rJ8AoITWCjGTPMJ-KzEdA_8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 704UQPqu6r_RZSNkPD91oUiTE44eYcca8EoohXhNp64
