# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 18:35:26
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 18:36:29
  - Authors: Anchor
  - Why: The real gate exposed host authority leakage and state behavior that must be repaired without recreating Core semantics.
  - Summary: Delegate VS Code endpoint discovery/presentation/session recovery and real-host regressions from the failed Sigma gate.
  - Status: ready/local

---

# Anchor To Kodax — Real-Host Sigma Gate Host-Boundary Recovery

## Handoff Parties

- Purpose: independently recover the VS Code host/controller failures exposed by Sigma while consuming shared Core truth without inventing endpoint, participant or material authority.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- live-endpoint-projection
  - Transfer Kind: work-and-responsibility
  - Description: repair production endpoint discovery/presentation so live choices are sourced only from explicit qualified Workspace/Core endpoint projections. Audit the concrete `endpointCatalog()` path that combines carried/local artifacts with `loadHandoffEndpointChoices(this.extensionPath)`, and remove any route by which nested repository test fixtures/schema examples become live production candidates without qualified Workspace authority.
  - Controlling Artifact: [Recovery Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Boundary: fixtures may remain repository-owned; fix authority scoping rather than deleting tests to hide leakage.

- exact-candidate-presentation
  - Transfer Kind: work-and-responsibility
  - Description: remove host-side semantic collapse by Role label/recency. Exact endpoint candidates with the same human label must remain disambiguated or unresolved according to Core truth; canonical Business Sigma must not be silently shadowed by fixture Sigma or another same-label Role.
  - Controlling Artifact: [Sigma Gate Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-sigma-real-host-gate-blocker-evidence.trace.md)
  - Boundary: presentation can clarify source/Workspace but cannot choose semantic authority by itself.

- host-state-and-byte-trace
  - Transfer Kind: work
  - Description: reproduce the Outgoing-context hydration inconsistency and independently trace Workspace bytes across Incoming/Replace, Local switching, authoring and Pack. Repair only host-owned state/byte mutation proven in VS Code; if exact bytes remain unchanged and Core rejects them, return that ownership evidence to Anchor/Loom.
  - Controlling Artifact: [Recovery Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Boundary: do not normalize/reseal semantic artifacts in the host merely to make Pack pass.

- real-host-regression
  - Transfer Kind: work-and-responsibility
  - Description: extend repository-owned acceptance to reproduce Sigma's real path, including live endpoint source qualification, a positive multi-participant case, supported authoring/Attach/Pack, Workspace-only Pack after Replace/Local/restart, and a hard negative that nested test fixtures/schema examples never appear as live endpoint choices in a normal production Workspace.
  - Controlling Artifact: [Recovery Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Boundary: test adapters remain at VS Code-owned seams and must drive production controllers rather than substitute direct Core results.

- kodax-return
  - Transfer Kind: responsibility
  - Description: return exact Extension VS Code delta, exact tests/real-host receipts available, ownership findings, residual risks and one qualified Kodax-to-Anchor Handoff; return shared Core gaps instead of recreating shared semantics locally.
  - Controlling Artifact: [Recovery Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Boundary: candidate-for-Anchor-reconciliation only; no Sigma promotion.

## Required Context

- controlling-task
  - Material: exact Real-Host Sigma Gate Root-Cause Recovery Task.
  - Material Reference: [Recovery Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Purpose: shared objective, Done Criteria and cross-layer ownership boundaries.
  - Availability: available

- sigma-gate-evidence
  - Material: exact Anchor-observed real-host Sigma blocker Evidence.
  - Material Reference: [Sigma Gate Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-sigma-real-host-gate-blocker-evidence.trace.md)
  - Purpose: actual operator reproduction target and source labels/error boundaries.
  - Availability: available

- extension-vscode-workspace
  - Material: exact failed-gate Extension VS Code candidate.
  - Material Reference: [Extension VS Code Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: writable host/controller/test implementation source.
  - Availability: available

- core-workspace
  - Material: exact current accepted Core source.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: read-only shared Tooling authority and Local-mode dependency until Loom returns a reconciled update.
  - Availability: available

- docs-workspace
  - Material: exact canonical Docs source.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: read-only semantic/schema authority; prevent host from inventing endpoint requirements.
  - Availability: available

- business-workspace
  - Material: exact current Business authority including gate Evidence, Decision and Task.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: work authority, Role references and bounded Evidence/return authoring.
  - Availability: available

## Reference Context

- prior-host-audit
  - Material: prior Kodax independent VS Code host-boundary audit and accepted repair history.
  - Material Reference: [Kodax Host Audit Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-3-1-kodax-vs-code-host-boundary-audit-evidence.trace.md)
  - Purpose: historical architecture boundary only; real Sigma evidence controls current defects.
  - Availability: available

## Retained Responsibilities

- shared-core-repair
  - Retained By: Loom
  - Retained By Reference: [Loom Role](business::.topics/roles/001-3-1-loom-canonical-holder-cutover-role.trace.md)
  - Responsibility: endpoint/material/packing semantics and shared integrity mechanics plus exact ownership diagnosis.
  - Boundary: Kodax returns shared gaps rather than implementing copies in the extension.

- integration-and-sigma-sequencing
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: reconcile parallel returns, prove the combined source and decide the next Sigma gate.
  - Boundary: Kodax cannot self-promote host acceptance to product acceptance.

## Exclusions And Dependencies

- no-shared-semantic-reimplementation
  - Kind: excluded-scope
  - Description: no private Role/Handoff/material/participant semantic engine in VS Code and no host-side resealing or authority inference.
  - Responsible Party Or Role: Kodax.

- no-fixture-deletion-workaround
  - Kind: excluded-scope
  - Description: repository test fixtures may not simply be deleted/moved to make the symptom disappear unless test architecture independently requires it; production discovery must remain correctly scoped even when nested fixture `.topics` exist.
  - Responsible Party Or Role: Kodax.

- loom-parallel-return
  - Kind: unresolved-dependency
  - Description: Loom is independently auditing Core source eligibility, authoring/Pack closure and Workspace integrity ownership. Kodax must preserve its exact local source delta so Anchor can fan-in without cross-edit ambiguity.
  - Responsible Party Or Role: Anchor for later reconciliation.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, release, publication or deployment.
  - Responsible Party Or Role: Anchor / release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return exact host repair/ownership Evidence and one Kodax-to-Anchor Handoff, or return blocked at the first shared dependency that cannot be resolved without violating the Core/Docs boundary.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: every nested `.topics` directory is invalid, fixtures cannot exist in the repository, host labels establish identity, or Extension VS Code owns endpoint/material semantics.
- Must Not Be Used To Claim: deleting fixture files is sufficient, a host-selected same-label Role is authoritative, or local VS Code tests alone make the candidate Sigma-ready.
- Authority Limits: VS Code host/controller/presentation and exact host-owned regression only; shared semantics remain Core/Docs-owned and Anchor retains integration/Sigma sequencing.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Value: YQlYnFeSTjmcFkCch0U2il9eZT9mxsE4U9a7NqLMQ_w

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: FP07MsgNIcfG_XKO3AqU5cB9uV4Ia0NOATfhGbVKhKM