# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Business Development](001-business-development-project.trace.md)
  - Origin:
    - [relative](001-business-development-project.trace.md)
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

- [Foundation Readiness And Operating Reconciliation](001-4-1-foundation-readiness-operating-reconciliation-task.trace.md)
- [Operating Overview And Monitoring](001-4-operating-overview-monitoring-task.trace.md)
- [Human Navigation And Active Frontier Experience](../initiatives/001-3-1-human-navigation-active-frontier-task.trace.md)
- Explicit recovery verification before destructive current-surface cleanup.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Business Development](001-business-development-project.trace.md)
  - Value: dxtfDTU66MwQI1ezqdpysgc1grW7UMmHOkoFRHyW3co

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: JtO0_iTYLLP5pmFo_C08nv_bAYeVTytR99TCeHKn4I8
