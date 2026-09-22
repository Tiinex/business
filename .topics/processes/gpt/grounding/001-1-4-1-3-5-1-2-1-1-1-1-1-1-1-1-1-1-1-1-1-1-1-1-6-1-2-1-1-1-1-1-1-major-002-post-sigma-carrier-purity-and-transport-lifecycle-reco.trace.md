# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.decision.v1
  - Created At: 2026-09-21 21:55:40
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-keep-major-002-open-and-parallelize-final-recovery.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-keep-major-002-open-and-parallelize-final-recovery.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-keep-major-002-open-and-parallelize-final-recovery.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 21:56:14
  - Authors: Anchor
  - Why: Latest Sigma replay narrowed remaining Major 002 risk to bounded Core/VS Code seams that can be recovered in parallel.
  - Summary: Close carrier purity, multi-route Transport, Outgoing discovery and host lifecycle defects without regressing the working primary path.
  - Status: ready/local

---

# Major 002 — Post-Sigma Carrier Purity And Transport/Lifecycle Recovery

## Objective

Close the bounded defects exposed by Sigma's latest real VS Code replay without regressing the now-working primary single-Handoff flow or moving shared semantics into the host.

## Scope

- Remove the recipient-v2 compatibility JSON sidecar from the normal recipient-facing Handoff carrier contract by completing/adopting the existing artifact-first clean-carrier mechanics at the correct Core boundary.
- Make multi-Handoff route projection and Transport deterministic for each exact qualified route.
- Bound live Outgoing Workspace discovery to explicit operator roots/qualified Workspace artifacts.
- Requalify or visibly invalidate stale Outgoing source state after Workspace identity/qualification changes.
- Reject duplicate Attach by exact Handoff identity and decouple tree refresh from notification lifecycle.
- Preserve successful single-Handoff Attach -> Pack -> Transport behavior.

## Done Criteria

- A newly manufactured normal Handoff package contains no `tiinex-recipient-v2.transport.json`; orient, validate, ground and transport projection remain qualified from visible Tiinex artifacts + exact payload bytes.
- No equivalent hidden/derived compatibility JSON becomes semantic authority or a required recipient input.
- A package with two qualified Handoff routes can be queued to Transport and each route produces its own exact transport text/recipient projection; explicit route selection remains fail-closed on a genuinely invalid route.
- A single-route package remains green.
- Production Outgoing Workspace choices do not include nested test/acceptance Workspaces outside explicit operator roots even when their `.topics` material remains in the repository.
- Existing Outgoing state does not retain a stale qualified source override after Workspace target bytes/qualification change; requalification/invalidation occurs before late Pack work.
- Attaching the same exact Handoff twice is rejected or idempotently represented without duplicate semantic attachment.
- Tree/Outgoing state visibly refreshes without requiring dismissal of a notification.
- Regression coverage drives production Core/controller paths rather than synthetic substitutes and preserves the exact Sigma reproductions as negative/positive cases.
- Loom and Kodax return exact deltas, tests, unresolved ownership findings and qualified Handoffs to Anchor with no remote mutation.

## Dependencies

- Latest Sigma carrier purity and lifecycle Evidence.
- Exact product-generated two-route Handoff package and its carried Business/Core/VS Code Workspaces.
- Current canonical Docs semantics remain read-only authority.
- Existing clean-carrier Phase 2 Core implementation is implementation context, not automatic acceptance.

## Ownership Boundaries

- Docs semantics remain unchanged unless a precise contradiction is returned to Anchor/Axiom.
- Core owns carrier construction/inspection, transport route projection and shared source qualification mechanics.
- VS Code owns operator-root selection, controller/state lifecycle, presentation and host invocation; it must not reconstruct semantic authority privately.
- Fixtures may remain; production discovery must be correct in their presence.

## Exclusions

- No fixture deletion/move as the primary fix.
- No post-build deletion of `tiinex-recipient-v2.transport.json` while runtime still depends on it.
- No host-only filtering that masks a shared Core projection defect.
- No schema loosening, remote commit/push/release/deploy, or Sigma promotion from specialist-local tests.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-keep-major-002-open-and-parallelize-final-recovery.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-keep-major-002-open-and-parallelize-final-recovery.trace.md)
  - Value: 9t0Nqr2fEUy6m61S4E8RZTV-aUpbKw92QKSl-4wHG4o

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: w33mim_up_Sdg6cT-JYt_OX_4p4ytCepkj1yPyBeE_0