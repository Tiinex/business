# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-27 20:50:25
  - Trace: [016-anchor-to-anchor-vscode-final-candidate-conversation-limit-recovery.trace.md](016-anchor-to-anchor-vscode-final-candidate-conversation-limit-recovery.trace.md)
  - Origin:
    - [relative](016-anchor-to-anchor-vscode-final-candidate-conversation-limit-recovery.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-27 23:18:08
  - Authors: Anchor
  - Why: Return the bounded implementation candidate for focused Sigma real-host acceptance without adding host-owned semantic paths or reopening Core.
  - Summary: VS Code-only candidate correcting Transport route selection, Handoff Title/Slug authoring, Outgoing pointer expansion, and native participant QuickPick authority flow; Core remains frozen.
  - Status: ready/local

---

## Handoff Parties

- Purpose: validate the bounded VS Code host-adapter candidate that fixes the concrete real-host blockers discovered from Sigma's latest Windows recordings while preserving Core as the sole semantic authority.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)

## Transfers

- vscode-host-boundary-candidate-016
  - Transfer Kind: work-and-responsibility
  - Description: perform the focused real Windows / VS Code acceptance pass on the exact carried VS Code Workspace. The candidate reuses Core-owned route selectors, Handoff rendering/materialization, endpoint projection and participant qualification; no alternative semantic path is introduced in the host.
  - Controlling Artifact: [preceding Anchor recovery](016-anchor-to-anchor-vscode-final-candidate-conversation-limit-recovery.trace.md)
  - Boundary: acceptance is limited to the concrete host seams listed below. Core remains frozen. Do not broaden discovery unless this exact candidate produces one reproducible blocker.

## Required Context

- vscode-candidate-workspace
  - Material: exact VS Code Workspace containing candidate 016 source, built dist, aligned dist-audit and regression updates.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: exact candidate under acceptance; no loose patch or VSIX derivative is authoritative over this Workspace snapshot.
  - Availability: available

- frozen-core-workspace
  - Material: exact frozen Core Workspace carried from the qualified parent package.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: semantic and Tooling authority. The candidate consumes its existing contracts and does not modify Core.
  - Availability: available

- app-workspace
  - Material: unchanged App Workspace carried from the qualified parent package.
  - Material Reference: [App Workspace](app::.topics/.workspaces/tiinex-app.workspace.md)
  - Purpose: preserve complete shared-consumer context without claiming an App delta.
  - Availability: available

- docs-workspace
  - Material: unchanged Docs Workspace carried from the qualified parent package.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: preserve canonical schema/validator context without claiming a Docs delta.
  - Availability: available

## Reference Context

- preceding-candidate-frontier
  - Material: exact predecessor acceptance frontier and recovery boundary.
  - Material Reference: [Handoff 016](016-anchor-to-anchor-vscode-final-candidate-conversation-limit-recovery.trace.md)
  - Purpose: preserves lineage from the prior qualified candidate while this Handoff narrows the next Sigma pass to the concrete discovered host blockers.
  - Availability: available

## Retained Responsibilities

- bounded-blocker-recovery
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: receive Sigma's disposition on this exact candidate. If accepted, preserve the accepted frontier. If one concrete blocker is returned, reproduce it against this exact carried Workspace and fix only at the demonstrated owner boundary.
  - Boundary: do not reopen Core, invent host-owned semantic authority, or broaden scope from subjective UX preference without a reproducible correctness blocker.

## Candidate Delta

- transport-route-selector
  - Change: Transport qualification now passes the exact Core-oriented Handoff Pointer path as `--route` instead of synthesizing `workspaceId:handoffPath` in VS Code.
  - Expected Effect: both Pack → Transport and Send to Transport → Transport qualify the same carried routes through one shared host seam.
  - Boundary: VS Code does not create route identity; Core orientation remains route authority.

- handoff-title-and-slug
  - Change: Handoff Title is forwarded to Core Handoff rendering so it becomes the durable H1/Summary. A separate optional Slug is only a path-label hint; blank Slug derives a From-to-To label and Core still owns slugification, lineage dimensioning, collision handling and final allocation.
  - Expected Effect: logical tree labels become meaningful through the existing H1 projection, while filenames remain Core-planned.
  - Boundary: no host slugifier or host filename allocator was added.

- outgoing-pointer-expansion
  - Change: Outgoing exact-carrier pointer nodes reuse the same pointer-target resolver already used by Incoming.
  - Expected Effect: expanding a Handoff/Role Pointer in Outgoing reveals the actual carried target just as Incoming does.
  - Boundary: no second pointer-resolution implementation was added.

- participant-quickpick
  - Change: Attach obtains optional 0..n additional participant Role selections from the same Core-projected endpoint catalog used by Handoff From/To, then Core requalifies the explicit selections and remains final participant authority.
  - Expected Effect: native VS Code multi-select UX without restoring Role-inventory-as-participant-authority.
  - Boundary: UI inventory is not semantic participant authority; only the returned Core participant projection is carried.

## Machine Qualification

- bridge-regressions
  - Result: 122/122 VS Code bridge cases passed against the frozen qualified Core source used as a local runtime surrogate because the execution environment could not reach the NPM registry.
  - Boundary: the surrogate was test-only and is excluded from the carried VS Code Workspace; package metadata remains pinned to `@tiinex/core@^0.45.0`.

- package-integration
  - Result: 6/6 package integration scenarios passed, including routed multi-route Pack, physical Handoff/participant pointers, re-orientation, idempotent retry and extracted VSIX/Core entrypoint behavior.
  - Boundary: Windows main-host UX acceptance remains Sigma's responsibility.

- built-javascript-syntax
  - Result: all 54 emitted `dist/**/*.js` files passed `node --check`; `dist-audit` is byte-aligned to the tested `dist` snapshot.
  - Boundary: this is syntax/build-output evidence, not a substitute for the real VS Code host gate.

## Focused Sigma Acceptance

- transport
  - Verify: Pack a routed Outgoing and confirm the finished carrier appears under Transport with the correct recipient/routing text.
  - Verify: use Send to Transport on a carrier and confirm it appears under the same Transport model.
  - Verify: exercise at least one multi-route carrier if available; no `selection-required` or `route-parties-required` error should arise from the old synthesized selector.

- handoff-authoring
  - Verify: enter a human Title and leave Slug blank. The created filename should be Core-allocated from From/To while the artifact H1/Summary and logical tree label use the entered Title.
  - Verify: optionally enter an explicit Slug and confirm it affects the Core-planned path without replacing the H1 Title.

- participants
  - Verify: after Attach, native QuickPick permits zero, one or multiple additional Role selections resolved from the same qualified open-Workspace endpoint source as Handoff From/To.
  - Verify: the resulting Outgoing route/pointers reflect Core's requalified participant projection rather than raw inventory.

- pointer-tree
  - Verify: in Outgoing Files projection, expand physical Handoff and Role Pointers and confirm their actual carried targets appear as children, matching Incoming behavior.

- latency
  - Observe: ordinary author/attach/Pack/Transport latency and report only a concrete reproducible stall. No performance refactor is requested by this Handoff without such evidence.

## Exclusions And Dependencies

- core-frozen
  - Kind: excluded-scope
  - Description: no Core change is part of this candidate. A Core change requires separate owner-level evidence that this exact host candidate cannot satisfy an existing contract.
  - Responsible Party Or Role: Anchor / Sigma

- no-parallel-vscode-semantics
  - Kind: excluded-scope
  - Description: do not add host-owned route IDs, endpoint discovery, participant authority, pointer semantics, slugification, carrier lineage or allocation paths parallel to Core.
  - Responsible Party Or Role: Anchor / Sigma

- no-broad-regression-reopen
  - Kind: excluded-scope
  - Description: Incoming/Replace and Commit/Push remain outside this focused pass unless an actual regression is observed.
  - Responsible Party Or Role: Sigma

## Completion Expectation

- Signal Kind: disposition
- Signal Meaning: Sigma either accepts the exact carried VS Code candidate for the focused host seams above, or returns one concrete reproducible blocker with visual evidence sufficient for bounded owner-level recovery.
- Return To: Anchor
- Return To Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Core was changed, remote merge/push occurred, Windows acceptance is already established, or any loose build derivative supersedes the carried Workspace snapshot.
- Must Not Be Used To Claim: permission to infer semantic authority from VS Code inventory, synthesize route/pointer/participant identity, broaden scope without a concrete blocker, or replace the canonical Handoff Package with loose files.
- Transport Limits: normal completion is this canonical Handoff Package plus the exact routing text projected by Core.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [016-anchor-to-anchor-vscode-final-candidate-conversation-limit-recovery.trace.md](016-anchor-to-anchor-vscode-final-candidate-conversation-limit-recovery.trace.md)
  - Value: CsZSC6DjRno-Y-G1bPgv7n6uymNEj0qErDr-2JLJvu4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: egGCqO5UcPAOgzQhUjxm6Vij1HV5c-guMGWx3Xt2dx4