# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-16 11:31:00
  - Trace: [001-2-7-5-1-5-forward-qualified-delegation-closure-projection.trace.md](001-2-7-5-1-5-forward-qualified-delegation-closure-projection.trace.md)
  - Origin:
    - [relative](001-2-7-5-1-5-forward-qualified-delegation-closure-projection.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-16 12:52:29
  - Authors: Anchor
  - Why: Real fresh-Anchor preflight shows the latest artifact-derived delegation projection incorrectly reuses the inbound recipient Role as the downstream delegate.
  - Summary: Separate current recipient/holder from the forward-selected downstream specialist in normal delegation grounding.
  - Status: ready/local

---

# Downstream Delegate Selection Projection Correction

## Objective

Correct the remaining delegation-readiness projection defect exposed by the real fresh-Anchor acceptance preflight: an inbound Anchor-to-Anchor Handoff correctly establishes the current recipient/holder as Anchor, but normal grounding currently reuses that recipient as the projected downstream delegate even when the controlling Task explicitly selects Axiom as the specialist whose review must be obtained.

Preserve the semantic distinction between current Handoff recipient/holder and downstream delegate selection. A fresh Anchor must be able to ground the current bounded Task and see the exact forward-qualified specialist selection without cached Role presence, Handoff endpoint labels, or repository inventory becoming delegation authority.

## Done Criteria

- Normal grounding of the bounded fresh-Anchor review carrier keeps the current recipient/holder as Anchor while projecting Axiom as the downstream selected specialist.
- Delegate/capability authority comes from an exact forward-qualified current-work selector plus exact Axiom Role material; it does not come from participant Role cache presence or the inbound Handoff `To` endpoint.
- Process applicability, target/source authority and return/reconciliation remain separately attributable and fail closed when absent.
- The projected normal next operations target Axiom, not Anchor, for the specialist Handoff.
- No arbitrary prose parsing, Role-name special case, hidden operator JSON, reverse Role/Relation inventory scan, or new Delegation/Participant schema is introduced.
- The model remains human-first/executor-neutral: current assignee and downstream delegate are separate organizational claims independent of chat/provider identity.
- Focused regression uses a real inbound Anchor-to-Anchor route plus a controlling Task selecting a different specialist Role.
- Full Core suite, portable smoke and embedded bootstrap qualification remain green.
- Loom returns qualified Evidence and one Loom-to-Anchor return Handoff.

## Scope

Core delegation-authority projection and focused regressions only. No Docs semantic rewrite, no Business mutation by Loom, no holder redesign, no product work, no generic receipt/UI redesign, and no unrelated refactor.

## Dependencies

- Axiom Qualified Delegation Grounding Semantic Disposition.
- Blank/minimal Workspace + Role-cache grounding semantics.
- Canonical holder cutover and active canonical Roles.
- Forward-Qualified Delegation Closure Projection implementation and its latest Loom return.
- Deterministic preflight of the fresh acceptance carrier showing `recipient/holder = Anchor` and incorrectly `delegate = Anchor` despite the controlling work explicitly selecting Axiom.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-7-5-1-5-forward-qualified-delegation-closure-projection.trace.md](001-2-7-5-1-5-forward-qualified-delegation-closure-projection.trace.md)
  - Value: uuKJfUqEV5wQyZw1pzRifnWDGvKTFBspIDHcGJs62aE

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: yCIqwxGqU4bka7SwoGorNSXFIEWAv_qdzbkyfRgQlCo