# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-12 22:33:28
  - Trace: [001-2-1-anchor-to-anchor-reduction-major-001-qualified-return.trace.md](../../processes/reduction/001-2-1-anchor-to-anchor-reduction-major-001-qualified-return.trace.md)
  - Origin:
    - [relative](../../processes/reduction/001-2-1-anchor-to-anchor-reduction-major-001-qualified-return.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-03 09:37:17
  - Authors: Anchor
  - Summary: Reduce terminal history across every carried Workspace, preserve unresolved/current work, then repair current broken survivors.
  - Status: ready/local

---

# Project-wide Lineage Reduction and Survivor Repair

## Objective

Reduce completed, accepted, superseded, and otherwise terminal historical Tiinex lineages across all currently carried Workspaces; physically remove only exact candidate sets whose recoverability and closure qualify; preserve unresolved or potentially current work; and repair surviving current broken lineages after the reduction pass.

## Done Criteria

- all carried Workspaces receive an explicit keep / reduce-delete / keep-and-repair disposition
- terminal historical lineages are represented by qualified Reduction material with immutable recovery for disappearing leaves or equivalent explicit recovery coverage
- destructive candidate sets pass the maintained exact `reduction-preflight` gate before local removal
- unresolved or potentially current lineages are not deleted
- current broken survivors are collected into a post-reduction repair frontier and repaired after historical noise is removed
- Workspace-level reductions compose into one project-level Reduction without treating status labels, timestamps, directories, or arrival order as standalone currentness authority
- a recoverable Handoff Package is manufactured before proceeding beyond each materially risky cleanup wave

## Scope

- all 17 Workspaces carried by carrier Major 015
- historical broken lineages may be deleted only when terminality, exact immutable recovery, Parent closure, and destructive eligibility are proven
- current or potentially current broken lineages are preserved for repair after reduction
- no remote Git/GitHub mutation is performed by this session
- Reduction remains distinct from lifecycle acceptance, destructive eligibility, and deletion authority

## Dependencies

- `tiinex.reduction.v1` and the qualified lineage-closure Reduction usage model
- Core Lineage Operative State, lineage traversal, lifecycle readiness, and `reduction-preflight`
- Reduction Major 001 project-wide classification as historical evidence to reconcile rather than a frozen current keep-list
- exact current Workspace material and immutable repository evidence where physical deletion is proposed

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-1-anchor-to-anchor-reduction-major-001-qualified-return.trace.md](../../processes/reduction/001-2-1-anchor-to-anchor-reduction-major-001-qualified-return.trace.md)
  - Value: X6W0_BwrMQCtEDT0oGbSbA0iitM2Dwr7UBtiEa-17Rs

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Csu5vJ5J_o6x96mUxzxkZr-NDmeIHEf9PYy9ZbvrXzg