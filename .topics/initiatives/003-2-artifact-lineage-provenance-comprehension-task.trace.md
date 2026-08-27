# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Viewer](003-viewer-project.trace.md)
  - Origin:
    - [relative](003-viewer-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Artifact, Lineage And Provenance Comprehension
  - Status: draft/local

---

# Artifact, Lineage And Provenance Comprehension

## Objective

Make individual Tiinex artifacts and their lineage/provenance understandable to humans, including Parent, Origin, integrity, boundaries, related work, evidence, and uncertainty.

## Done Criteria

- Artifact reading distinguishes semantic content from transport/runtime metadata.
- Lineage views preserve direct Parent meaning while showing related cross-repository context separately.
- Integrity, source, publication, and uncertainty states are visible without implying stronger authority than evidence supports.
- Human-readable schema companions cover the active artifact families needed by current Initiatives.

## Scope

- Do not hide critical provenance behind hover-only or machine-only state.
- Do not flatten Parent, Origin, relation, and project membership into one generic link.
- Presentation must not rewrite artifact truth.

## Dependencies

- Core lineage/provenance semantics epic.
- Tooling integrity/discovery APIs.
- Real Business and historical Site artifacts as dogfood.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Viewer](003-viewer-project.trace.md)
  - Value: bTq9sIP2kEnVOJ5A6oUEQMVFXF9n8wjj6IdtzSTUpKU

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: yaCGkfi8U5MeRgMUeDur6U6O1QTiEqGDcyaslfD3bcM
