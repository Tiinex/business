# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Tooling](002-tooling-project.trace.md)
  - Origin:
    - [relative](002-tooling-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Integrity, Validation And Repair Toolchain
  - Status: draft/local

---

# Integrity, Validation And Repair Toolchain

## Objective

Provide reliable creation-time integrity, validation, graph inspection, repair planning/application, and evidence-aware publication/permalink maintenance without silently rewriting authored semantics.

## Done Criteria

- Tooling can distinguish valid, degraded, ambiguous, stale, missing, and repairable states.
- Repair planning is reviewable before mutation and repair application preserves authored content boundaries.
- Parent-target and self-integrity behavior is consistent across ordinary artifacts, packages, and cross-repository references.
- Validation results expose schema-capability gaps separately from artifact defects.

## Scope

- Do not convert warnings into automatic semantic rewrites.
- Do not claim publication/canonical authority from successful hashing or repository reachability.
- Keep repair operations bounded and reversible.

## Dependencies

- Current integrity validator and repair operations.
- Historical lineage repair/publication feedback.
- Core lineage/provenance semantics epic.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Tooling](002-tooling-project.trace.md)
  - Value: ttGDyrDpEo9mqBL7armC42aip4IaNFsx2NjAVwTP66Y

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 68DJZ4ogqB7XtkoPkhOvZIx2Aajv8Gc2vFLTFtGhBEc
