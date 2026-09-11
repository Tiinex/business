# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-11 12:38:12
  - Trace: [001-stream-day-parallel-major-001-orchestration.trace.md](001-stream-day-parallel-major-001-orchestration.trace.md)
  - Origin:
    - [relative](001-stream-day-parallel-major-001-orchestration.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-11 16:59:13
  - Authors: Anchor
  - Why: Correct repository-boundary placement prospectively without rewriting historical continuity.
  - Summary: Repository-boundary placement correction
  - Status: ready/local

---

# Repository-boundary placement correction

## Objective

Correct the current orchestration drift where specialist Tasks and Handoffs defaulted into Business. Business remains the cross-repository coordination, Role, priority and human-gate surface; specialist implementation continuity belongs in the owning repository.

## Done Criteria

- New specialist work artifacts use repository-local Parent continuity in their owning repositories.
- Business may reference specialist work and carry Role/human-gate context without becoming the default artifact Parent or storage location.
- Handoff packages may carry Business Role material as Required Context while the authoritative Handoff artifact remains in the owning repository.
- Existing historical Business artifacts remain preserved as historical truth; no mass rewrite or silent relocation is implied.
- New repository-local continuations avoid extending malformed historical cross-Workspace Parent locators.

## Scope

Placement and continuation policy for active Core, App/Site Viewer, Verse Playthings, VS Code and Chrome lanes. No product implementation or canonical schema change.

## Dependencies

- Current Turn-2 Business orchestration and repository-frontier intent.
- Core Carrier Major 002 lineage-safety repair for qualified cross-Workspace Parent handling and carrier allocation.
- Existing repository-local Turn-2 frontier artifacts in each owning repository.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-stream-day-parallel-major-001-orchestration.trace.md](001-stream-day-parallel-major-001-orchestration.trace.md)
  - Value: XVBIK1Q4XsLJQCqk_bq8MYdQKtMcwCt_2zSdwyHtSKQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: N6aESXBT7gissKfKMn5ju7hVnpb-y3o1kA0SpXsCcLg