# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-29 08:56:00
  - Trace: [Current Business Surface Reconciliation](001-4-1-1-current-business-surface-reconciliation-task.trace.md)
  - Origin:
    - [relative](001-4-1-1-current-business-surface-reconciliation-task.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-29 09:10:00
  - Authors: Anchor; Sigma
  - Why: Human inspection showed that numeric and sibling-distinct prefixes were insufficient: several current semantic children did not carry their parent branch dimension forward in the filename, so the visual path disagreed with the declared Parent tree.
  - Summary: Lineage Path Filename Discipline Correction
  - Status: accepted/local

---

# Lineage Path Filename Discipline Correction

## Objective

Make current Business filenames project the same lineage shape as declared Parent ancestry so a human can scan a directory tree and understand branch depth before opening the artifacts.

## Done Criteria

- `001-roles` children use `001-1`, `001-2`, `001-3`, and `001-4`.
- `001-initiatives` children use `001-1`, `001-2`, and `001-3`; retained Tooling/Viewer work packages extend those project paths one additional segment.
- `001-financing` -> `001-1-funds` -> `001-1-1-bounty-fund` -> `001-1-1-1-bounty-model-decision` visibly follows the declared Parent chain.
- Business Development's already-correct `001 -> 001-N -> 001-N-M` paths remain unchanged.
- Validation rejects a non-root semantic child whose visible dimension path is not exactly its parent's path plus one segment.
- Relative references, self integrity, Parent integrity, and organization-root reachability remain valid after the repair.

## Scope

- Current pre-publication tiinex/business reconciliation candidate only.
- Do not renumber Git history or introduce fake semantic parents merely for storage folders.
- Top-level semantic branches may restart their local visible path at `001` directly under the Tiinex organization root; collection folders do not create extra segments.

## Dependencies

- Parent reconciliation: [Current Business Surface Reconciliation](001-4-1-1-current-business-surface-reconciliation-task.trace.md).
- Governing rule: [Business Lineage Structure](../decisions/001-business-lineage-structure-decision.trace.md).
- Human review of the condensed Business tree.

## Result

- Roles, Initiatives, and Financing now use full visible lineage paths consistent with their declared Parent chains.
- Whole-surface validation checks Parent-path correspondence rather than only numeric-prefix presence or sibling uniqueness.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Current Business Surface Reconciliation](001-4-1-1-current-business-surface-reconciliation-task.trace.md)
  - Value: OfAqlC0cPOKY2AVGZ3vqV3xoGSzXzcUNkbRqrtayCTA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: nHxP76YbigE6QONqTEouzGtu0uxN9nbwDmZvGTa8ji0
