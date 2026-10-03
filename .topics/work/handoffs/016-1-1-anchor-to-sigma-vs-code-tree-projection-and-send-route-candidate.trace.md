# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-27 23:18:08
  - Trace: [016-1-anchor-to-sigma-vs-code-host-boundary-fix-candidate-016.trace.md](016-1-anchor-to-sigma-vs-code-host-boundary-fix-candidate-016.trace.md)
  - Origin:
    - [relative](016-1-anchor-to-sigma-vs-code-host-boundary-fix-candidate-016.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-28 10:42:25
  - Authors: Anchor
  - Why: Return the bounded Candidate 017 follow-up for focused Sigma real-host acceptance without creating host-owned semantic alternatives or reopening Core.
  - Summary: Candidate 017 preserves the accepted Candidate 016 correctness frontier while closing the remaining logical-tree, row-level Send to Transport, zero-participant expansion and repo-hygiene seams.
  - Status: ready/local

---

## Handoff Parties

- Purpose: validate the bounded Candidate 017 VS Code presentation/host-orchestration delta after Candidate 016 passed its primary correctness seams on Sigma's real Windows host.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)

## Transfers

- vscode-presentation-and-send-route-candidate-017
  - Transfer Kind: work-and-responsibility
  - Description: perform one focused real Windows / VS Code acceptance pass on the exact carried VS Code Workspace. Candidate 017 preserves the Candidate 016 Title/Slug, participant, Pack and Transport correctness frontier while closing the remaining logical-tree presentation asymmetry, the row-level Send to Transport selector seam, and the zero-participant Outgoing expansion edge case.
  - Controlling Artifact: [Candidate 016](016-1-anchor-to-sigma-vs-code-host-boundary-fix-candidate-016.trace.md)
  - Boundary: Core remains frozen. VS Code projects Core-owned route/pointer/participant evidence and explicit operator intent only; no parallel resolver, route identity, pointer identity, slugification, participant authority or manufacture path is introduced.

## Required Context

- vscode-candidate-workspace
  - Material: exact VS Code Workspace containing Candidate 017 source, built dist, synchronized audit build, focused regressions and repository-hygiene update.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: exact candidate under acceptance; no loose patch or derived VSIX supersedes this Workspace snapshot.
  - Availability: available

- frozen-core-workspace
  - Material: exact frozen Core Workspace inherited from the qualified Candidate 016 parent carrier.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: semantic and Tooling authority. Candidate 017 consumes existing Core projections and does not modify Core.
  - Availability: available

- app-workspace
  - Material: unchanged App Workspace inherited from the qualified Candidate 016 parent carrier.
  - Material Reference: [App Workspace](app::.topics/.workspaces/tiinex-app.workspace.md)
  - Purpose: preserve complete shared-consumer context without claiming an App delta.
  - Availability: available

- docs-workspace
  - Material: unchanged Docs Workspace inherited from the qualified Candidate 016 parent carrier.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: preserve canonical schema/validator context without claiming a Docs delta.
  - Availability: available

## Reference Context

- candidate-016-acceptance-frontier
  - Material: exact preceding Candidate 016 acceptance Handoff and the real-Windows video disposition that established Title/Slug, participant qualification, Pack to Transport and Transport route correctness.
  - Material Reference: [Candidate 016](016-1-anchor-to-sigma-vs-code-host-boundary-fix-candidate-016.trace.md)
  - Purpose: preserve the accepted correctness frontier while narrowing this successor to the remaining presentation and row-level acceptance seams.
  - Availability: available

## Retained Responsibilities

- bounded-follow-up-recovery
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: receive Sigma's disposition on this exact Candidate 017. If one concrete blocker remains, reproduce it against this exact carried Workspace and correct only at the demonstrated owner boundary.
  - Boundary: do not reopen Core or the Candidate 016 correctness seams without new reproducible evidence.

## Candidate Delta

- logical-handoff-pointer-projection
  - Change: Incoming logical Handoff expansion now projects the exact physical Handoff Pointer plus the exact participant Role Pointer coordinates already carried by Core orientation. Outgoing logical Handoff expansion presents the corresponding pending Handoff/participant pointer intent from the already Core-qualified authoring projection.
  - Expected Effect: Incoming and Outgoing logical views expose the same operator concept while truthfully distinguishing pre-Pack pending material from post-Pack physical carrier material.
  - Boundary: Incoming pointer coordinates come only from Core orientation; Outgoing pre-Pack rows never synthesize final pointer paths. Physical target resolution still uses the existing shared pointer resolver.

- outgoing-zero-participant-expansion
  - Change: every written included Outgoing Handoff remains expandable even when there are zero additional participants, because the Core-owned Handoff Pointer projection is still a valid child row.
  - Expected Effect: zero-participant routes do not hide their Handoff-pointer provenance solely because participant count is zero.
  - Boundary: this is TreeView presentation state only; no participant or pointer semantics change.

- row-send-to-transport-selector
  - Change: Send to Transport from a resolved Handoff row now forwards the exact Core-oriented Handoff Pointer path to the existing shared Transport qualification seam. Persisted route selection matches route id or exact pointer path; the old host-synthesized `workspaceId:handoffPath` selector is removed.
  - Expected Effect: row-level Send to Transport selects exactly the intended Core-qualified route and uses the same qualification path already proven by Candidate 016 Pack to Transport.
  - Boundary: no second Transport queue or selector grammar is introduced in VS Code.

- orientation-pointer-ancestry-preservation
  - Change: the VS Code received-Handoff adapter preserves Core's endpoint/participant/grounding pointer arrays instead of discarding them at the host boundary.
  - Expected Effect: presentation can consume exact Core-projected pointer ancestry without reparsing or rediscovering semantic relationships.
  - Boundary: adapter preservation grants no new authority and performs no inference.

- repository-hygiene
  - Change: `dist-audit/` is ignored by Git and the local audit snapshot used for qualification is synchronized to the tested Candidate 017 `dist` output.
  - Expected Effect: generated audit output cannot be accidentally committed while local byte-comparison remains available during this qualification pass.
  - Boundary: no runtime or semantic behavior changes.

## Machine Qualification

- offline-typescript-barrier
  - Result: strict TypeScript source qualification passed in the constrained execution environment using the available compiler and the local VS Code compatibility type surface used for offline checking.
  - Boundary: the exact repository devDependency install remains a Windows/local clean-build gate; this result is not represented as a substitute for Sigma's real host build.

- bridge-regressions
  - Result: 122/122 VS Code bridge cases passed after rebuilding `dist` from the Candidate 017 source.
  - Boundary: focused source/bridge regression evidence; real Extension Host behavior remains a separate gate.

- package-integration
  - Result: 6/6 package integration scenarios passed against the frozen Core dependency, including multi-route manufacture and physical route/participant pointer ancestry.
  - Boundary: package integration does not substitute for native TreeView interaction.

- built-javascript-syntax
  - Result: changed emitted JavaScript passed `node --check`; the synchronized `dist-audit` snapshot is byte-identical to the tested `dist` file set excluding the generated VSIX carrier.
  - Boundary: syntax/output evidence only.

- extension-host-regression-added
  - Result: Candidate 017 adds a real Extension Host scenario that independently closes the package-wide Transport item, invokes row-level Send to Transport, verifies exact route-id/pointer selection, and restores the whole-package queue before restart checks.
  - Boundary: the current execution environment has no VS Code CLI, so Sigma's Windows run is the executable host gate for this added scenario.

## Focused Sigma Acceptance

- outgoing-files
  - Verify: with only valid included routes, open Outgoing Files projection before Pack and expand a physical Handoff Pointer and participant Role Pointer. Their actual carried targets should appear through the existing pointer resolver.
  - Verify: repeat with a Handoff that has zero extra participants; the Handoff row remains expandable and exposes Handoff-pointer provenance.

- logical-tree
  - Verify: in compact logical projection, expand an Outgoing Handoff and an Incoming Handoff. Both should expose pointer-oriented provenance; Outgoing truthfully says pending Pack while Incoming exposes physical carrier pointers. Incoming participant pointers should come from the qualified carrier rather than reconstructed Role inventory.

- send-to-transport
  - Verify: invoke Send to Transport from one resolved Handoff row and confirm one prepared carrier appears under Transport with only that exact Core-qualified route selected.
  - Verify: package-root Send to Transport still queues the whole qualified route set and survives the ordinary reload/restart path.

- regression-preservation
  - Verify: Title/Slug/H1 authoring, native 0..n participant QuickPick, Core-qualified participant projection and ordinary Pack to Transport remain as observed in the Candidate 016 pass.

- latency
  - Observe: report only a concrete reproducible stall. Candidate 017 does not introduce a performance refactor or duplicate manufacture path to improve tree presentation.

## Exclusions And Dependencies

- core-frozen
  - Kind: excluded-scope
  - Description: no Core change is part of Candidate 017. Core is reopened only with separate owner-level evidence that the exact carried host candidate cannot satisfy an existing contract.
  - Responsible Party Or Role: Anchor / Sigma

- no-parallel-vscode-semantics
  - Kind: excluded-scope
  - Description: do not add host-owned route IDs, endpoint discovery, participant authority, pointer relationship inference, slugification, carrier lineage/allocation or alternate manufacture/Transport paths.
  - Responsible Party Or Role: Anchor / Sigma

- no-grounding-ux-expansion
  - Kind: excluded-scope
  - Description: `grounded-to-act`, `discuss` and related Core readiness vocabulary remain internal host/Core state in this candidate; no additional operator-facing Ground Handoff UX is introduced unless it enables a concrete required human action.
  - Responsible Party Or Role: Anchor / Sigma

## Completion Expectation

- Signal Kind: disposition
- Signal Meaning: Sigma either accepts the exact carried Candidate 017 for the focused real-host seams above, or returns one concrete reproducible blocker with visual evidence sufficient for bounded owner-level recovery.
- Return To: Anchor
- Return To Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Core was changed, Windows acceptance is already established, generated audit/VSIX output is source authority, or presentation rows grant semantic authority.
- Must Not Be Used To Claim: permission to infer semantic relationships from VS Code inventory, synthesize route/pointer/participant identity, broaden scope without a concrete blocker, or replace the canonical Handoff Package with loose files.
- Transport Limits: normal completion is one canonical Handoff Package plus the exact routing text projected by Core.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [016-1-anchor-to-sigma-vs-code-host-boundary-fix-candidate-016.trace.md](016-1-anchor-to-sigma-vs-code-host-boundary-fix-candidate-016.trace.md)
  - Value: egGCqO5UcPAOgzQhUjxm6Vij1HV5c-guMGWx3Xt2dx4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: VmEf-szZY7DsCAsGlfoEIPlYMszj5xg_REv59VMcUKk