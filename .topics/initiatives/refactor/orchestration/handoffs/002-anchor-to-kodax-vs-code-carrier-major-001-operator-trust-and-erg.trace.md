# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-11 12:43:13
  - Trace: [001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md](../vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md)
  - Origin:
    - [relative](../vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 12:44:03
  - Authors: Anchor
  - Why: Sigma approved semi-independent Kodax development against extension-vscode so Anchor can run additional Majors in parallel while retaining shared-boundary and recovery reconciliation.
  - Summary: Delegate the bounded VS Code Major 001 safety, workflow and finish lane with a short Sigma dogfood loop.
  - Status: ready/local

---

# Anchor to Kodax — VS Code Carrier Major 001 Operator Trust And Ergonomics

## Handoff Parties

- Purpose: delegate the approved VS Code carrier Major 001 implementation/dogfood lane to Kodax so Sigma can iterate with fewer Anchor stops while shared semantics, Major scope and final reconciliation remain bounded.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-kodax-role.trace.md)

## Transfers

- vscode-major-001-implementation
  - Transfer Kind: work-and-responsibility
  - Description: implement and locally qualify the safety, workflow and finish tranche defined by the controlling VS Code carrier Major 001 Task, working directly with Sigma's Windows observations/videos at meaningful dogfood gates.
  - Controlling Artifact: [VS Code Carrier Major 001](../vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md)
  - Boundary: extension-vscode source and extension-local UX/tests only unless a shared gap is explicitly returned to Anchor.

- sigma-dogfood-loop
  - Transfer Kind: responsibility
  - Description: keep the Sigma test loop short and evidence-driven: self-qualify deterministic/local behavior first, then request one bounded Windows/video observation when it can answer a real unknown; avoid asking Sigma to manually retest unchanged surfaces.
  - Controlling Artifact: [VS Code Carrier Major 001](../vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md)
  - Boundary: Sigma observations are feedback/evidence and do not automatically close the Major or authorize shared/release changes.

## Required Context

- extension-vscode-workspace
  - Material: complete carried current extension-vscode source and repo-local lineage.
  - Material Reference: [extension-vscode Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: writable implementation lane.
  - Availability: available

- core-workspace
  - Material: complete carried current Core source and package/authoring/Tooling contracts.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: exact shared mechanics dependency; read-only unless a shared gap is returned to Anchor.
  - Availability: available

- docs-workspace
  - Material: complete carried canonical Docs source.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: exact human-first Handoff/Workspace/lineage/schema boundaries; read-only.
  - Availability: available

- business-workspace
  - Material: complete carried Business source with Kodax Role, current orchestration and controlling Major Task.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: exact scope, role, return and human-gate authority.
  - Availability: available

## Reference Context

- site-workspace
  - Material: complete carried current thin Site source.
  - Material Reference: [Site Workspace](site::.topics/.workspaces/tiinex-site.workspace.md)
  - Purpose: read-only comparison context when reconciling shared human artifact-authoring/Handoff package ergonomics; Site is not writable through this lane.
  - Availability: available

- sigma-observation-channel
  - Material: Sigma can supply screenshots or short silent Windows videos during the lane.
  - Purpose: bounded real-host observation after deterministic local qualification, especially for Pack/Attach/staging/conditional-action behavior.
  - Availability: available

## Retained Responsibilities

- shared-semantics-and-cross-repo-routing
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
  - Responsibility: adjudicate/route Core, Docs, Site or cross-repository gaps; keep carrier Major progression separate from artifact filename lineage.
  - Boundary: Kodax returns a scoped blocker/change proposal instead of privately patching shared semantics.

- human-acceptance
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-sigma-role.trace.md)
  - Responsibility: Windows-host UX observation and human acceptance at bounded gates.
  - Boundary: technical PASS and videos do not create release or Major-closure authority by themselves.

- major-closure-and-recovery-merge
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
  - Responsibility: audit the return package, merge qualified deltas into the current full recovery, decide Major closure/progression, and refresh the full recovery carrier.
  - Boundary: child transport recency does not override the current full frontier wholesale.

## Exclusions And Dependencies

- branding-source-not-carried
  - Kind: unresolved-dependency
  - Description: Sigma requested the Tiinex primary logo from the organization's `.github/assets` source, but the current sixteen-Workspace recovery does not carry the `.github` repository. Do not guess/copy a lookalike; leave branding closure pending until Anchor supplies exact qualified source bytes.
  - Responsible Party Or Role: Anchor

- shared-repository-mutation
  - Kind: excluded-scope
  - Description: do not mutate Core, Docs, Site or Business source through this Handoff. Return exact evidence and the smallest change proposal if shared capability is missing.
  - Responsible Party Or Role: Anchor / owning specialist

- remote-release-publish
  - Kind: excluded-scope
  - Description: no Marketplace publication, release/version advance, remote push, Site deployment or other external mutation is authorized by this Handoff.
  - Responsible Party Or Role: Sigma / Anchor at a later explicit gate

- broad-new-features
  - Kind: excluded-scope
  - Description: unrelated extension features are deferred. Safety-critical findings may reorder work inside this Major but do not silently expand its outcome.
  - Responsible Party Or Role: Anchor

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return one normal Tiinex Handoff to Anchor carrying the complete current extension-vscode Workspace, technical evidence for each in-scope workflow, exact unresolved blockers/change proposals, and a concise statement of Sigma-observed behavior without converting observation into acceptance. The return must be auditable/mergeable against Anchor's latest full recovery.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Interpretation Limits

- Does Not Mean: Kodax owns Core/Docs/Site semantics, auto commit/push are already trusted, the requested branding source is carried, a video proves acceptance, or a long artifact filename indicates carrier Major progression.
- Must Not Be Used To Claim: release readiness, Marketplace readiness, final README/branding acceptance, shared semantic changes, or Major 001 closure without Anchor/Sigma reconciliation.
- Authority Limits: bounded extension-vscode implementation and technical qualification only.
- Transport Limits: carried sibling Workspaces are read-only context and must not be returned as replacement source outside the explicitly transferred extension-vscode lane.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md](../vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md)
  - Value: X6UqB50cTIcfgzXPh3UWJYac2PtLPpiwBcCfYIinCjM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: NRSMt0yDf5OSmpFFdz7OSPYXkYI_ZhejxBhK_ZDmuLU