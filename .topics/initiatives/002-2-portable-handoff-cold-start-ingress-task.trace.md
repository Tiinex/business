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
  - Summary: Portable Handoff, Cold-Start And LLM Ingress
  - Status: draft/local

---

# Portable Handoff, Cold-Start And LLM Ingress

## Objective

Make portable Handoff manufacture, cold-start orientation, recipient grounding, role/participant routing, and continuation reliable and clean for fresh humans and LLMs across workspaces.

## Done Criteria

- Blank-recipient cold-start can reach Tiinex Tooling and the intended Handoff route with minimal explicit bootstrap actions.
- Carrier lineage dimensions preserve fixed-width labels such as 001 and Tooling regression tests fail on normalization drift.
- Recipient-V2 transport facts are no longer duplicated as JSON blobs inside every human-readable carrier artifact; machine transport projection has one bounded representation or is safely derived.
- Handoff packages preserve exact workspace bytes, required context qualification, roundtrip integrity, and clear human routing without hidden semantic authority.

## Scope

- Do not manually patch generated packages as the product solution.
- Transport metadata must not become semantic authority.
- Human-facing Tiinex artifacts should remain readable without repeated machine-only blobs.

## Dependencies

- Current recipient-v2 carrier implementation and bootstrap runtime.
- Historical cold-start/Handoff dogfood and fresh-recipient qualification.
- Axiom review where transport changes touch schema semantics.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Tooling](002-tooling-project.trace.md)
  - Value: 0zVe7vLWB7VMnz_nU766CpSRIadi72v6t8oX4sxuCxY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: sRhlQ3PmMPEgr18JtqR3Q9dG-8vAPNgG7knwkU-umeA
