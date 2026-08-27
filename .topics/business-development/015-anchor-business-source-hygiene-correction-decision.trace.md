# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.feedback.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/feedback/tiinex.feedback.v1.schema.md)
  - Created At: 2026-08-28 00:06:00
  - Trace: [Business Checkpoint Source Hygiene Failed Before Commit](014-sigma-business-source-hygiene-and-dimension-prefix-feedback.trace.md)
  - Origin:
    - [relative](014-sigma-business-source-hygiene-and-dimension-prefix-feedback.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-28 00:09:00
  - Authors: Anchor; Sigma
  - Why: Convert Sigma's pre-commit source-tree review into a bounded repair and replacement checkpoint without publishing the rejected Business 002 source.
  - Summary: Withdraw Business 002 as a commit candidate, remove current `.cache` residue, normalize first-dimension filenames, relocate the Business Lineage Structure Decision for navigation hygiene, and require the replacement checkpoint to carry the full current semantic source with preserved evidence-asset boundary.
  - Status: accepted/local

---

# Anchor Business Source Hygiene Correction

## Decision

- State: accepted.
- Subject: repair of the uncommitted Business 002 checkpoint before Git durability.
- Decision: Business 002 is withdrawn as a commit candidate. The replacement source removes `.topics/.cache`, applies `001-` initial dimension prefixes to ordinary first-materialization semantic artifacts that lacked them, updates all affected local references and integrity, and moves the retained Business Lineage Structure Decision to `.topics/decisions/001-business-lineage-structure-decision.trace.md`. Its semantic Parent remains the Tiinex organization root; no artificial descendants or authority edges are introduced to make tree presentation prettier.

## Naming Correction

- Tiinex's own semantic `.trace.md` authoring uses an initial lineage dimension as the preferred filename form, including the organization root, now `.topics/001-tiinex.trace.md`. Dimensionless trace artifacts remain readable/valid where the format permits them, but Tooling and Tiinex-maintained examples should recommend the prefixed form. Workspace descriptors and schema snapshot filenames remain separate naming surfaces.
- Corrected ordinary semantic filenames include Roles/Initiatives/Financing branch anchors, Financing sub-branch anchors, fund resources, the personal tip instrument, and the Financing decisions that previously lacked an initial dimension.
- Human navigation is part of the naming contract: because ordinary file explorers are scanned left-to-right, putting the dimension first makes lineage participation visible before the descriptive name and also gives deterministic sibling ordering.
- The naming repair changes paths, not semantic identity or authority. References are rewritten to the new local paths and integrity is resealed from exact current bytes.

## Working-Set Cleanup

- `.topics/.cache` is removed from the replacement current source. Its predecessor material is already recoverable from published Git history and no current Business artifact declares the cache as semantic authority.
- Historical evidence assets referenced by accepted Business artifacts are not deleted merely because they are not ordinary Markdown artifacts. A destructive full-repository replacement must preserve or carry their exact bytes; otherwise use an overlay plus explicit cache deletion.

## Business Lineage Structure Placement

- The artifact is a Decision and therefore belongs on the Decision navigation surface when retained in the current tree.
- Its Parent remains `.topics/001-tiinex.trace.md`, so it is semantically a direct organization-root Decision and may be a leaf. That is truthful. Default active-frontier Discovery should later filter resolved/background Decisions rather than falsify lineage to avoid visible leaves.

## Git Gate

- Sigma confirmed no commit/push occurred for Business 002, so no remote rollback or history rewrite is required.
- Only the corrected successor checkpoint may be proposed for the next commit/push action.
- Anchor must verify the resulting remote commit after Sigma publishes it before treating cleanup and current-state continuity as durable.

## Follow-Up

- Tooling/Discovery should eventually expose current-vs-historical/superseded filtering so stable background Decisions do not dominate the active frontier.
- Tooling authoring guidance should recommend initial dimensions for Tiinex-authored `.trace.md` artifacts while continuing to read dimensionless artifacts when the schema/format allows them.
- Repository-hygiene work should continue from the published corrected checkpoint rather than from the rejected local package.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Business Checkpoint Source Hygiene Failed Before Commit](014-sigma-business-source-hygiene-and-dimension-prefix-feedback.trace.md)
  - Value: 5H4jnfJDMLEsVmYwLEUAoafO3NrAJe7ZqrzvRhJbxLM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:bMl9hoHulev-G3BUVBxJtvniSEW_HszDWF9LM-rPcyQ
