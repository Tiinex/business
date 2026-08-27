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
  - Summary: Lineage, Provenance And Publication Semantics
  - Status: draft/local

---

# Lineage, Provenance And Publication Semantics

## Objective

Make Parent, Origin, integrity, publication, permalink, provider evidence, and graph-recovery semantics coherent enough that later readers and Tooling can recover truthful lineage across local, unpublished, published, and packaged states.

## Done Criteria

- Parent remains direct continuity ancestry and is not overloaded for project membership or process participation.
- Origin/publication/permalink evidence can represent unpublished and published states without fabricating canonical authority.
- Integrity and graph recovery rules distinguish missing evidence, stale links, mutation, and qualified repair opportunities.
- Cross-repository lineage remains inspectable through stable qualified references.

## Scope

- Do not rewrite historical evidence solely to make graphs look clean.
- Do not treat repository location or package carriage as publication/canonical authority.
- Repair semantics must preserve authored body meaning unless a separate decision authorizes change.

## Dependencies

- Existing lineage-integrity and publication feedback.
- Integrity validator semantics.
- Tooling repair/publication evidence work.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Core](001-core-project.trace.md)
  - Value: iPnUakoUgOJxovtSJtf3TEcAIJrfOv7NTah1MIagOMU

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: EwM6PvjrIOluPMbz0XpuRFJgHaAxnBa6-R3_-zpGdOk
