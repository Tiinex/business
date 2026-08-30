# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:57:00
  - Trace: [Initiatives](001-initiatives.trace.md)
  - Origin:
    - [relative](001-initiatives.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-27 23:54:00
  - Authors: Anchor; Sigma
  - Why: Turn the current public-facing and working-tree cleanup concerns into one recoverability-gated professionalization tranche instead of ad-hoc README edits or destructive repository cleanup.
  - Summary: Public-surface and repository-hygiene epic covering GitHub organization entrypoints, tiinex.dev Workspace entry, repository first-contact surfaces, current/history separation, architecture-vision refresh, and safe working-set reduction.
  - Status: accepted/local

---

# Public Surfaces And Repository Hygiene

## Objective

Make Tiinex public entrypoints and repository working surfaces accurately project current provenance, while keeping historical material recoverable in Git instead of letting it dominate ordinary discovery.

## Done Criteria

- The GitHub organization profile, repository first-contact material, and tiinex.dev describe the same current Tiinex identity and current-vs-historical boundary expressed by provenance.
- Contribution, security/support, governance, and funding guidance are understandable without requiring internal archaeology and do not become competing semantic authority.
- Repository working trees favor current material; superseded intermediate artifacts are removed from current HEAD only when Git history or another explicit recovery boundary preserves them.
- Public claims about release/functioning are limited to what current Site/Docs/Tooling evidence actually qualifies.
- Presentation remains shorter and easier to scan than internal provenance, while deeper artifact paths stay available for people who need exact evidence.

## Scope

- Public `.github`, README/orientation material, repository metadata, tiinex.dev entry surfaces, and current/history presentation boundaries.
- Current working-tree hygiene where stale material interferes with comprehension.
- Do not rewrite historical artifacts merely to make old lineage resemble the current organization.

## Dependencies

- [Foundation Readiness And Operating Reconciliation](001-6-foundation-readiness-operating-reconciliation-task.trace.md)
- [Human Navigation And Active Frontier Experience](001-3-1-human-navigation-active-frontier-task.trace.md)
- Explicit recovery verification before destructive current-surface cleanup.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Initiatives](001-initiatives.trace.md)
  - Value: ooAvsZ-ZLG6eafU4w8lMBq8-Zj5rrurJeLA_o2dMh0I

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 225g3JxSdVX1aAzXu1aN84JgQXKvijyvtHMhx1HN_i8
