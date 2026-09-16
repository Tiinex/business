# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 20:52:23
  - Trace: [001-2-7-5-1-2-1-1-pre-migration-role-parent-audit-cutover-correction.trace.md](001-2-7-5-1-2-1-1-pre-migration-role-parent-audit-cutover-correction.trace.md)
  - Origin:
    - [relative](001-2-7-5-1-2-1-1-pre-migration-role-parent-audit-cutover-correction.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 21:23:27
  - Authors: Anchor
  - Summary: Identifier-Only Historical Role Parent Cutover Semantics
  - Status: ready/local

---

# Identifier-Only Historical Role Parent Cutover Semantics

## Objective

Resolve the remaining canonical holder cutover boundary exposed by the real active Role migration: ordinary Role authoring now qualifies exact historical pre-migration Parents when their historical `Current Schema` has exact schema-reference authority, but the active Anchor and Prism Role continuations declare `Current Schema: tiinex.party.role.v1` without an exact target and therefore still cannot serve as direct migration Parents.

Determine the one canonical, human-first semantic rule for continuing an active Role lineage from such an immutable historical Parent without rewriting history, branching around the latest Role, pretending the historical artifact used the amended current schema revision, or introducing a permanent compatibility representation.

## Done Criteria

- Classify the exact historical-parent schema-authority state for the active Anchor continuation `business::.topics/roles/001-1-1-1-1-anchor-thin-lineage-orchestration-discipline-role.trace.md` and active Prism continuation `business::.topics/roles/001-8-1-prism-role.trace.md`.
- Decide whether a current canonical Role child may preserve direct Parent continuity when the historical Parent's exact bytes/integrity and Role schema identifier are qualified but its historical `Current Schema` target is identifier-only.
- Preserve the distinction between historical audit/provenance and current candidate validation; no inference that the historical Parent used the amended Assignment Modes schema revision is permitted.
- Preserve one active Role format and one canonical current Assignment Modes authority after cutover; no permanent legacy-positive holder path, hand-written envelope format, Role-name exception, or alternate migration Role type.
- Preserve human-first/executor-neutral Role semantics; do not introduce chat/LLM-specific schema authority to solve the authoring edge case.
- State the exact fail-closed/tooling consequence if the available historical evidence is insufficient to authorize direct continuation.
- Return a qualified Axiom semantic disposition for Anchor reconciliation and any narrowly required Loom mechanics.

## Scope

Historical Role Parent schema-reference authority during the canonical Assignment Modes hard cutover. Docs semantics/schema interpretation only; no Business Role mutation or Core implementation by Axiom.

## Dependencies

- Axiom `Canonical Holder Assignment Mode Hard Cutover Semantic Disposition`.
- Loom `Pre-Migration Role Parent Audit Cutover Correction Qualification`.
- Real Anchor migration failure: `portable.cli.author.parent.schema-authority.required` on the active thin-lineage Anchor Role whose historical `Current Schema` is identifier-only.
- Real Prism migration has the same identifier-only historical `Current Schema` shape and must be covered generically rather than by Role label.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-7-5-1-2-1-1-pre-migration-role-parent-audit-cutover-correction.trace.md](001-2-7-5-1-2-1-1-pre-migration-role-parent-audit-cutover-correction.trace.md)
  - Value: 9U7jpleTHQpoQ5tJAkQoC35E3c5G64jXLZjmgAPZuGo

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: amoVp5X7FQ83c1SuPpW0Fw5PX_E6MTp7QwyyzrPscsw