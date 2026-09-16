# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 20:08:32
  - Trace: [001-2-7-5-1-2-1-canonical-role-authoring-cutover-enablement.trace.md](001-2-7-5-1-2-1-canonical-role-authoring-cutover-enablement.trace.md)
  - Origin:
    - [relative](001-2-7-5-1-2-1-canonical-role-authoring-cutover-enablement.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 20:52:23
  - Authors: Anchor
  - Why: The first real Business Axiom migration attempt still fails because common authoring re-audits the historical parent as a current Role and requires Assignment Modes on the old bytes.
  - Summary: Correct common Role authoring so genuine pre-migration parent bodies remain historical evidence while new canonical Role continuations validate strictly.
  - Status: ready/local

---

# Pre-Migration Role Parent Audit Cutover Correction

## Objective

Correct the remaining portable Role-authoring cutover defect exposed by the first real Business migration attempt: a canonical current Role continuation can stage with direct `Assignment Modes`, but overall authoring still fails because the exact pre-migration Parent Role is re-audited as though it were a current Role under the amended schema and therefore reports missing `Assignment Modes`.

The migration path must preserve the exact historical Parent bytes and provenance while validating the new candidate against the current canonical Role contract. Historical auditability must not become dual current authorization, and current Role validation must not be weakened.

## Done Criteria

- Reproduce the exact Business Axiom migration case from `business::.topics/roles/001-2-axiom-role.trace.md`, whose historical body has no `Assignment Modes`.
- A canonical Axiom Role continuation with direct `explicit-session, handoff` qualifies through ordinary `author` while preserving the historical Parent unchanged.
- Historical Parent qualification is evaluated as historical Parent evidence/provenance rather than reinterpreted as a current operational Role requiring the amended field.
- The new current candidate still fails closed when `Assignment Modes` is missing, empty, invalid, duplicated, aliased, prose-like, or out of canonical order.
- The correction introduces no Role-label/path special case, no schema bypass, no second Role format, no legacy-positive current holder authorization and no hand-written envelope path.
- Regression coverage uses at least one genuine pre-migration Role body lacking `Assignment Modes`; a fixture built from the current Role creation contract and merely given an old schema locator is not sufficient.
- Return exact Core evidence and one Loom-to-Anchor Handoff. Do not remove `LEGACY_ROLE_MAPPINGS` until Anchor has completed and qualified the active Business Role migration disposition.

## Scope

Portable common authoring/audit handling of exact historical Role Parents during the canonical holder cutover, plus focused regression coverage. No Business Role migration or Docs semantic amendment belongs to Loom.

## Dependencies

- Business `Canonical Role Authoring Cutover Enablement`.
- Axiom `Canonical Holder Assignment Mode Hard Cutover Semantic Disposition`.
- Loom `Canonical Role Authoring And Schema Packaging Cutover Qualification`.
- Exact failed migration receipt observed by Master Anchor: candidate staging recognizes canonical `Assignment Modes`, while workspace/audit errors target the pre-migration parent `001-2-axiom-role.trace.md` for missing `Assignment Modes`.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-7-5-1-2-1-canonical-role-authoring-cutover-enablement.trace.md](001-2-7-5-1-2-1-canonical-role-authoring-cutover-enablement.trace.md)
  - Value: 6JMU1QVWnVCv9VEH5e_l8uE_G64U5sA5DdtVYiP7zS4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 9U7jpleTHQpoQ5tJAkQoC35E3c5G64jXLZjmgAPZuGo