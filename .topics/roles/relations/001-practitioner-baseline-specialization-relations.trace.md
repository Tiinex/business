# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 23:39:00
  - Trace: [Axiom Business Lineage And Composition Gap Disposition](../../decisions/001-axiom-business-lineage-and-composition-gap-disposition.trace.md)
  - Origin:
    - [relative](../../decisions/001-axiom-business-lineage-and-composition-gap-disposition.trace.md)
- Current
  - Current Schema: [tiinex.relation.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/relation/tiinex.relation.v1.schema.md)
  - Created At: 2026-08-27 12:58:00
  - Authors: Anchor
  - Why: Materialize the accepted Practitioner specialization model as a typed non-Parent relation without duplicating the shared working-method baseline inside each specialized Role.
  - Summary: Typed role-specialization relations linking Anchor, Axiom, Loom, and Sigma to the Tiinex Practitioner baseline without granting authority through inheritance.
  - Status: accepted/local

---

# Practitioner Baseline Specialization Relations

## Relation Declaration

- Relation Type: incorporates role baseline
- Relation Direction: specialized Tiinex roles -> Tiinex Practitioner baseline
- Relation Scope: shared working-method obligations, observation, friction detection, and continuous-improvement heuristics only

## Relation Target

- Target: [Anchor Role](../001-anchor-role.trace.md)
  - Relation Type: Anchor incorporates Practitioner baseline
  - Relation Direction: Anchor -> Tiinex Practitioner
  - Relation Scope: shared working-method baseline only
- Target: [Axiom Role](../001-axiom-role.trace.md)
  - Relation Type: Axiom incorporates Practitioner baseline
  - Relation Direction: Axiom -> Tiinex Practitioner
  - Relation Scope: shared working-method baseline only
- Target: [Loom Role](../001-loom-role.trace.md)
  - Relation Type: Loom incorporates Practitioner baseline
  - Relation Direction: Loom -> Tiinex Practitioner
  - Relation Scope: shared working-method baseline only
- Target: [Sigma Role](../001-sigma-role.trace.md)
  - Relation Type: Sigma incorporates Practitioner baseline
  - Relation Direction: Sigma -> Tiinex Practitioner
  - Relation Scope: shared working-method baseline only
- Baseline: [Tiinex Practitioner](../001-practitioner-role.trace.md)

## Relation Boundary

- These are typed specialization/composition relations, not Tiinex continuity Parents.
- Tiinex Practitioner contributes common working-method expectations but does not widen any specialized Role's `May Do`, holder state, delegation, decision rights, representation authority, or other authority boundary.
- Each specialized Role remains authoritative for its own explicit scope and limitations.
- Future versions of a logical Role use Parent for same-role continuity; Practitioner specialization remains separate from that version lineage.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Axiom Business Lineage And Composition Gap Disposition](../../decisions/001-axiom-business-lineage-and-composition-gap-disposition.trace.md)
  - Value: -Y37Kk6OhdyZomqLWO6iMFUy1xp1TYM9cIAH_h5RjWc

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:aO68JZ6RWAizNUjW4UflVUYx30K79acrLd_ux2RGbHw
