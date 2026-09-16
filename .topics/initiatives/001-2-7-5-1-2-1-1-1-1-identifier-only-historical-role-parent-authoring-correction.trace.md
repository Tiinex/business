# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 21:23:27
  - Trace: [001-2-7-5-1-2-1-1-1-identifier-only-historical-role-parent-cutover-semantics.trace.md](001-2-7-5-1-2-1-1-1-identifier-only-historical-role-parent-cutover-semantics.trace.md)
  - Origin:
    - [relative](001-2-7-5-1-2-1-1-1-identifier-only-historical-role-parent-cutover-semantics.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 21:59:25
  - Authors: Anchor
  - Why: Axiom accepted direct continuation with identifier-only historical schema authority; Core must preserve that weaker historical truth without substituting today's schema revision.
  - Summary: Coordinate the narrow Core correction required to continue Anchor and Prism from exact identifier-only historical Role Parents under one canonical holder cutover.
  - Status: ready/local

---

# Identifier-Only Historical Role Parent Authoring Correction

## Objective

Integrate Axiom's accepted identifier-only historical Role Parent semantics into the remaining canonical holder cutover so the active Anchor and Prism Roles can continue directly from their exact immutable historical Parents without rewriting history, inferring historical schema-revision equality, or creating a second active Role representation.

Coordinate one narrow Core correction that preserves identifier-only historical Parent schema authority as identifier-only while keeping the new child Role strictly governed by the exact current canonical `tiinex.party.role.v1` schema and direct canonical `Assignment Modes`.

## Done Criteria

- Loom qualifies the exact generic author/reference behavior defined by Axiom for identifier-only historical Role Parents.
- Exact historical Parent bytes, self-integrity, declared schema identifier and truthful recovery route remain required and fail closed on contradiction.
- The child `Parent Schema` remains the plain historical schema identifier unless an exact historical target is independently qualified; today's current schema target is never substituted as historical provenance.
- Current child Role validation remains strict against the exact current canonical Role schema, including direct canonical `Assignment Modes`.
- Anchor and Prism are both covered generically without Role-name/path exceptions.
- No history rewrite, revision inference, alternate Role format, legacy-positive holder authority, prose parsing, or executor-specific semantics are introduced.
- Loom returns qualified Evidence and one return Handoff for Anchor reconciliation.
- `LEGACY_ROLE_MAPPINGS` remains in place until the complete active Role migration is qualified; this Task does not authorize final removal.

## Scope

Business coordination for the one remaining Core author/reference correction required by the canonical holder hard cutover. No direct Core implementation by Anchor and no additional Docs semantic work unless Loom finds a concrete contradiction in Axiom's accepted rule.

## Dependencies

- Axiom `Identifier-Only Historical Role Parent Cutover Semantic Disposition`.
- Business `Identifier-Only Historical Role Parent Cutover Semantics` Task.
- Loom `Pre-Migration Role Parent Audit Cutover Correction Qualification`.
- Current partial active-Role migration state: Axiom, Loom, Sigma, Glimmer, Kodax and Pilot canonical; Anchor and Prism intentionally pending this correction.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-7-5-1-2-1-1-1-identifier-only-historical-role-parent-cutover-semantics.trace.md](001-2-7-5-1-2-1-1-1-identifier-only-historical-role-parent-cutover-semantics.trace.md)
  - Value: amoVp5X7FQ83c1SuPpW0Fw5PX_E6MTp7QwyyzrPscsw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: J6vISAbZ5HdMLrD25emWRHWNGgl6hlL9iZJV_IGMufg