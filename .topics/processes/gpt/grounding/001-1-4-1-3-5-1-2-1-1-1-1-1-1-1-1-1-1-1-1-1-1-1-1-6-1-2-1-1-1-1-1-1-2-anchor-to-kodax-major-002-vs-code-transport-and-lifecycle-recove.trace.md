# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 21:56:14
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 21:57:02
  - Authors: Anchor
  - Why: Latest Sigma replay leaves bounded VS Code-owned controller and lifecycle defects.
  - Summary: Repair live Outgoing discovery, stale-state lifecycle, duplicate Attach, refresh and host multi-route invocation.
  - Status: ready/local

---

## Handoff Parties

- Purpose: close the remaining VS Code-owned discovery, Transport invocation and lifecycle defects exposed by the latest Sigma replay while preserving Core semantic authority.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- outgoing-workspace-discovery
  - Transfer Kind: work-and-responsibility
  - Description: make Select Outgoing Workspaces use only explicit operator Workspace roots and qualified Workspace artifacts; nested test/acceptance Workspaces must not become live choices because the extension repository contains them.
  - Boundary: keep fixtures present; fix production source scope rather than hiding evidence.

- stale-outgoing-requalification
  - Transfer Kind: work-and-responsibility
  - Description: when Workspace target/source identity changes, deterministically requalify or visibly invalidate existing Outgoing source state before Pack; eliminate late stale `workspace-source-override-unqualified` surprises.
  - Boundary: do not reseal/normalize semantic artifacts in the host to force qualification.

- duplicate-attach-and-refresh
  - Transfer Kind: work-and-responsibility
  - Description: reject/idempotently handle duplicate attachment of the same exact Handoff identity and ensure tree/Outgoing refresh does not depend on notification/toast dismissal.
  - Boundary: Handoff identity comes from qualified exact artifact/source truth, not display label alone.

- multi-route-transport-host-seam
  - Transfer Kind: work-and-responsibility
  - Description: reproduce Sigma's two-route Transport failure using the exact carried package and verify the host invokes Core route projection with exact qualified selectors for every route. Fix host invocation/selection only where proven; return shared projection defects to Loom.
  - Boundary: do not locally reconstruct route semantics or filter a Core failure into false green.

- real-host-regression
  - Transfer Kind: work-and-responsibility
  - Description: extend production-controller regression to cover single-route success, multi-route Transport, explicit operator-root Workspace discovery, stale Outgoing invalidation, duplicate Attach and refresh independence.
  - Boundary: fixtures may drive the host but must not become live production authority.

- kodax-return
  - Transfer Kind: responsibility
  - Description: return exact VS Code delta, tests/real-host receipts available, residual risks and one qualified Kodax-to-Anchor Handoff.
  - Boundary: candidate for Anchor fan-in only; no Sigma self-promotion.

## Required Context

- controlling-task
  - Material: exact Post-Sigma Carrier Purity And Transport/Lifecycle Recovery Task.
  - Material Reference: [Recovery Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md)
  - Purpose: controlling objective and Done Criteria.
  - Availability: available

- sigma-evidence
  - Material: exact Anchor-preserved latest Sigma replay Evidence.
  - Material Reference: [Sigma Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-major-002-latest-sigma-carrier-purity-and-lifecycle-evidence.trace.md)
  - Purpose: exact observed failures and product-output package reproduction.
  - Availability: available

- vscode-workspace
  - Material: exact VS Code Workspace carried by the latest Sigma product package.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: writable host/controller/test source.
  - Availability: available

- core-workspace
  - Material: exact Core Workspace carried by the latest Sigma product package.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: read-only shared projection/tooling authority until Loom return fan-in.
  - Availability: available

## Reference Context

- latest-product-carrier
  - Material: exact `tiinex-vscode-001-sigma-to-anchor.handoff-package.zip` produced during the latest Sigma replay.
  - Purpose: concrete two-route carrier reproduction and recipient-surface evidence; it is observational product output, not current-work authority.
  - Availability: available

## Retained Responsibilities

- shared-carrier-and-route-projection
  - Retained By: Loom
  - Retained By Reference: [Loom Role](business::.topics/roles/001-3-1-loom-canonical-holder-cutover-role.trace.md)
  - Responsibility: recipient carrier purity, shared multi-route projection and shared source qualification mechanics.
  - Boundary: Kodax returns Core-owned defects rather than duplicating mechanics.

- fan-in-and-sigma
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: reconcile returns and decide the next Sigma gate.
  - Boundary: no specialist-local acceptance promotion.

## Exclusions And Dependencies

- no-fixture-deletion-workaround
  - Kind: excluded-scope
  - Description: do not remove/move fixtures merely to make live choices disappear.
  - Responsible Party Or Role: Kodax.

- no-private-semantic-engine
  - Kind: excluded-scope
  - Description: no local recreation of Role/Handoff/route/material semantics or Core transport truth.
  - Responsible Party Or Role: Kodax.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, release, publication or deployment.
  - Responsible Party Or Role: Anchor / release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return the bounded VS Code repair/evidence and one Kodax-to-Anchor Handoff, or stop at the first exact shared dependency blocker.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: VS Code owns carrier semantics, host filtering can replace Core qualification, or test fixtures may be removed to hide a production leak.
- Must Not Be Used To Claim: local extension tests alone establish Major 002 acceptance.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md)
  - Value: w33mim_up_Sdg6cT-JYt_OX_4p4ytCepkj1yPyBeE_0

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: g314MyDyXpKrh0ozvF_GAKR-5RcQepOJmjHPAmlVhGY