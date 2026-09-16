# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 17:24:06
  - Trace: [001-2-7-5-1-2-canonical-holder-assignment-mode-normalization.trace.md](001-2-7-5-1-2-canonical-holder-assignment-mode-normalization.trace.md)
  - Origin:
    - [relative](001-2-7-5-1-2-canonical-holder-assignment-mode-normalization.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 20:08:32
  - Authors: Anchor
  - Why: Axiom accepted the hard cutover, but the first qualified Business Role migration attempt is blocked because current portable authoring cannot qualify the pre-migration Role parent against the amended governing Role schema.
  - Summary: Enable canonical Role revision against the amended holder Assignment Modes schema without retaining dual current authority.
  - Status: ready/local

---

# Canonical Role Authoring Cutover Enablement

## Objective

Enable the active Business Role migration required by the accepted Axiom canonical holder hard-cutover semantics by ensuring current Tooling can author/revise `tiinex.party.role.v1` artifacts against the amended Docs Role schema with direct canonical `Holder Relationship -> Assignment Modes` authority.

The current migration attempt is blocked before any active Business Role can be revised: portable Role authoring preserves an older unresolved Parent Schema locator from the pre-migration Role and fails candidate qualification with `schema.reference.target-unqualified` even when the revised body carries canonical Assignment Modes. This is a schema-material/authoring qualification gap, not justification for hand-editing Roles or retaining dual current holder authority.

## Done Criteria

- Current portable Role authoring can create a Role continuation whose Parent is an exact qualified pre-migration Role while qualifying the governing amended Docs `tiinex.party.role.v1` schema material.
- The authored Role carries direct canonical `Assignment Modes` and qualifies against the amended current Role creation contract.
- The authoring path does not require hand-written envelopes, bypassed validation, permissive legacy Role formats, Role-name special cases, prose parsing, or a second active Role representation.
- Schema provenance remains exact and auditable; historical Role bytes remain historical evidence rather than current positive assignment authority.
- After this enablement returns, Master Anchor can migrate and explicitly declare the complete active Business Role set before Loom removes the temporary legacy holder mapping from current runtime authorization.

## Scope

Portable Role authoring/schema-material packaging and exact Parent-schema qualification needed to perform the already-accepted canonical holder hard cutover. No Business Role migration is performed by Loom in this Task and no legacy bridge removal occurs before Anchor supplies qualified complete migration evidence.

## Dependencies

- Business `Canonical Holder Assignment Mode Normalization` Task.
- Axiom `Canonical Holder Assignment Mode Hard Cutover Semantic Disposition` and amended Docs `tiinex.party.role.v1` schema.
- Observed portable authoring blocker `schema.reference.target-unqualified` when revising an exact qualified pre-migration Axiom Role with direct canonical Assignment Modes.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-7-5-1-2-canonical-holder-assignment-mode-normalization.trace.md](001-2-7-5-1-2-canonical-holder-assignment-mode-normalization.trace.md)
  - Value: sHcRIrW-bE0NbTMBahP5wbeJg3VVtpaeU5wqWGajp_0

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 6JMU1QVWnVCv9VEH5e_l8uE_G64U5sA5DdtVYiP7zS4