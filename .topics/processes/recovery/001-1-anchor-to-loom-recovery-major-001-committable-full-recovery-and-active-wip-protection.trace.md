# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-13 16:11:30
  - Trace: [001-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md](001-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md)
  - Origin:
    - [relative](001-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-13 16:11:46
  - Authors: Anchor
  - Why: Full Recovery must be stable and committable for Sigma, but the latest landing over active WIP staged destructive rollback/deletion scope instead of failing closed.
  - Summary: Route bounded Recovery-integrity mechanics to Loom with explicit direct return reservation 1.
  - Status: ready/local

---

# Anchor To Loom — Recovery Major 001 Committable Recovery And WIP Protection

## Handoff Parties

- Purpose: make Full Recovery landings fail closed on unaccepted/divergent target WIP instead of silently staging deletions/reversions, and add a coarse Recovery acceptance audit suitable for Master Anchor.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role — Successor Evolution Continuation](business::.topics/roles/001-1-1-1-anchor-successor-evolution-role.trace.md)
- To: Loom
- To Kind: role
- To Reference: [Loom Role](business::.topics/roles/001-3-loom-role.trace.md)

## Transfers

- recovery-integrity-and-landing-preflight
  - Transfer Kind: work-and-responsibility
  - Description: implement the bounded Recovery Major 001 objective using existing host-neutral compare/reconcile/landing mechanics where possible, so accepted Recovery cannot silently destroy newer target WIP.
  - Boundary: preserve accepted-state semantics and fail closed rather than auto-importing unaccepted WIP into Recovery.

- recovery-acceptance-audit
  - Transfer Kind: responsibility
  - Description: expose enough deterministic evidence for Anchor to verify a manufactured Full Recovery as stable, restartable, and committable before Sigma receives it.
  - Boundary: this is a coarse recovery-integrity gate, not artifact-by-artifact semantic validation.

- reserved-return-package-sibling-index
  - Transfer Kind: responsibility
  - Description: Master Anchor explicitly reserves package sibling index 1 for the direct Loom → Anchor return from this delegation.
  - Boundary: this reservation applies only to this direct return and creates no general allocation authority.

## Required Context

- controlling-task
  - Material: Recovery Major 001 — Committable Full Recovery And Active-WIP Protection.
  - Material Reference: [Recovery Major 001](business::.topics/processes/recovery/001-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md)
  - Purpose: bounded objective, reproduced evidence, and acceptance criteria.
  - Availability: available

- current-recovery
  - Material: current Full Recovery controlling context carried by this package.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: current accepted program/recovery authority.
  - Availability: available

## Reference Context

- reproduced-diff
  - Material: Anchor audit found the Recovery snapshot unchanged across the two compared Recovery carriers, while the current VS Code candidate had 28 current-only files and 36 changed files relative to that snapshot.
  - Purpose: distinguish a destructive target-landing problem from an unproven claim that Reduction pruned the Recovery itself.
  - Availability: available

## Retained Responsibilities

- recovery-acceptance
  - Retained By: Anchor
  - Responsibility: final integration, Full Recovery acceptance, program-map reconciliation, and Sigma-facing committable guarantee.

- canonical-semantics
  - Retained By: Axiom
  - Responsibility: any canonical schema/method meaning change must be separately routed.

- human-gate
  - Retained By: Sigma
  - Responsibility: human product/host acceptance only; Sigma is not asked to repair source, reconstruct Recovery, or debug reconciliation.

## Exclusions And Dependencies

- no-wip-promotion
  - Kind: excluded-scope
  - Description: do not merge unaccepted local WIP into Master Recovery merely to make the target checkout clean.

- no-artifact-cleanup
  - Kind: excluded-scope
  - Description: do not mass-delete, rename, reparent, or normalize historical Tiinex artifacts in this Major.

- semantic-boundary
  - Kind: unresolved-dependency
  - Description: if the repair requires canonical semantics rather than host-neutral Tooling mechanics, return an exact Axiom-owned follow-up instead of inventing semantics.
  - Responsible Party Or Role: Loom

## Completion Expectation

- Signal Kind: return
- Signal Meaning: one qualified Loom → Anchor carrier through reserved sibling index 1, carrying the bounded Recovery-integrity implementation, broad validation, and exact evidence that divergent active WIP fails closed before destructive landing while exact-safe recovery remains green.
- Return To: Anchor
- Return To Reference: [Anchor Role — Successor Evolution Continuation](business::.topics/roles/001-1-1-1-anchor-successor-evolution-role.trace.md)

## Acceptance Evidence

- exact-safe Full Recovery landing remains green;
- current-only/divergent target state is detected before mutation and does not become silent deletions/reversions;
- reconciliation is explicit when needed;
- accepted Recovery does not silently absorb unaccepted WIP;
- Recovery acceptance audit exposes unexplained removal/change evidence suitable for Anchor disposition;
- focused and broad Core/Tooling validation passes on exact candidate bytes;
- direct return manufactures through the reserved sibling index without Sigma repair.

## Interpretation Limits

- Does Not Mean: a Full Recovery must contain every local experimental/WIP byte in a developer checkout.
- Must Not Be Used To Claim: target WIP is accepted merely because Recovery preserves or detects it.
- Authority Limits: Loom owns bounded Tooling/recovery mechanics; Anchor retains orchestration, acceptance, and recovery disposition.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md](001-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md)
  - Value: -_YX-EmvHd9U_9qEosRUJkRhZVOx-w4-r-LdCiBhudQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: xzbFm8w-iXRSE6KHEof2uyCeGRN0Dwn7FUqT7ofahWo