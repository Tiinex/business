# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-04 21:36:02
  - Trace: [007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md](007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md)
  - Origin:
    - [relative](007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-10-04 21:37:07
  - Authors: Anchor; Sigma
  - Why: Finish the remaining user-visible edges without reopening accepted lineage, Workspace, or Package V1 semantics.
  - Summary: Transfer the last bounded transport/presentation checks to Sigma before creating the real stable Major.
  - Status: ready/local

---

# Anchor To Sigma Final Transport Polish Acceptance Handoff

## Handoff Parties

- Purpose: transfer the final bounded real VS Code acceptance of continuation naming, transport-text hygiene, Handoff preview, and byte-identical embedded source preference before creating the real stable Major
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)
- Notes: this is the last narrow acceptance before the stable Major; Sigma remains an ordinary Tiinex recipient and is not expected to debug implementation

## Transfers

- final-transport-polish-acceptance
  - Transfer Kind: work-and-responsibility
  - Description: confirm the four remaining user-visible edges in the normal Windows/VS Code workflow and, only if all pass, perform the real explicit Major package action for the stable checkpoint
  - Controlling Artifact: [Finish Handoff Transport And VS Code Presentation Polish](007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md)
  - Boundary: observation/acceptance only until the explicit final Major action; implementation repair remains with Anchor

## Required Context

- controlling-task
  - Material: current final transport/presentation polish Task
  - Material Reference: [Finish Handoff Transport And VS Code Presentation Polish](007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md)
  - Purpose: exact regressions, candidate behavior, machine evidence, and acceptance boundaries
  - Availability: available

- grounding-applicability
  - Material: exact applicability Relation for this bounded Task
  - Material Reference: [Final Transport Polish Acceptance Guidance Applicability](007-1-final-transport-polish-acceptance-guidance-applicability-relation.trace.md)
  - Purpose: explicit grounding/recipient guidance selection
  - Availability: available

- current-core-workspace
  - Material: exact current Core Workspace carried by this package
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: continuation transport naming fix, transport-text CLI hygiene, and removal of leaked `true`
  - Availability: available

- current-vscode-workspace
  - Material: exact current VS Code Workspace carried by this package
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: built-in Handoff Markdown Preview and byte-identical embedded source preference
  - Availability: available

- portable-grounding-process
  - Material: Portable Session Grounding And Continuity
  - Material Reference: [Portable grounding process](native::.topics/.processes/session-grounding-and-continuity/001-session-grounding-and-continuity-process.trace.md)
  - Purpose: recipient transfer and recovery discipline
  - Availability: available

- tiinex-grounding-profile
  - Material: Tiinex Session Grounding And Continuity Profile
  - Material Reference: [Tiinex grounding profile](../processes/session-grounding-and-continuity/001-session-grounding-and-continuity-process.trace.md)
  - Purpose: Anchor/Sigma acceptance boundary
  - Availability: available

## Reference Context

- prior-major-allocation-repair
  - Material: previous carrier Major allocation repair
  - Material Reference: [Align Handoff Package Carrier Major Allocation](006-align-handoff-package-carrier-major-allocation-task.trace.md)
  - Purpose: establish that Major allocation is not reopened by this Task
  - Availability: available

## Retained Responsibilities

- anchor-debug-and-repair
  - Retained By: Anchor
  - Responsibility: diagnose and repair any implementation issue returned by Sigma
  - Boundary: Sigma returns the observed result and does not become the debugger

## Sigma Acceptance Surface

After manually merging only the minimum changed Workspaces identified next to this carrier:

1. Run `Tiinex: Switch all to Local`.
2. Run the existing `Tiinex: Build linked extension` task and restart/reload normally.
3. Open this Incoming carrier / create the next Outgoing continuation without a Major bump. Expected filename shape: the new `-1` extends the carrier dimension before `-anchor-to-sigma`, never after the slug.
4. Confirm no literal `true` file is created in Core while packing; the carried Core candidate itself must no longer contain `true`.
5. Click the Handoff artifact in the Tiinex tree. Expected: built-in VS Code Markdown Preview opens by default; source remains reachable through VS Code's normal Markdown preview/source controls.
6. Where Local and embedded Incoming Workspace bytes are exact, embedded wins the Outgoing source choice deterministically. In the observed case this should apply to byte-identical Core; changed/non-identical local material must remain Local.
7. If these checks pass, perform the real explicit Major package action. Existing same-prefix Major allocation remains highest-observed + 1 (for example, if `021` is the highest observed Major, the stable Major becomes `022`).
8. If any check fails, stop and return video/screenshot plus the observed filename/source state. Do not debug.

Previously repaired Discovery, Replace, Initialize, and Major allocation do not need broad retesting unless a visible regression appears.

## Exclusions And Dependencies

- semantic-lineage-change
  - Kind: excluded-scope
  - Description: artifact lineage, artifact filename conventions, semantic Parent ancestry, Workspace identity, and Handoff semantic authority are unchanged
  - Responsible Party Or Role: none in this Task

- package-topology-change
  - Kind: excluded-scope
  - Description: Package V1 internal archive topology, Workspace materialization topology, carrier Parent semantics, and Handoff route topology are unchanged
  - Responsible Party Or Role: none in this Task

- implementation-debugging
  - Kind: excluded-scope
  - Description: source isolation, TypeScript repair, CLI parser debugging, or package-manufacture debugging are not Sigma responsibilities
  - Responsible Party Or Role: Anchor if acceptance returns a blocker

- remote-mutation
  - Kind: excluded-scope
  - Description: commit, push, publication, release, deployment, and other remote writes are not authorized by this Handoff
  - Responsible Party Or Role: separately authorized operator after acceptance

## Completion Expectation

- Signal Kind: disposition
- Signal Meaning: report whether the four final polish checks pass and, if they do, whether the real explicit Major action succeeds with the expected next same-prefix Major
- Return To: Anchor
- Return To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- Notes: a short pass/fail plus video/screenshots is sufficient; Sigma should not debug implementation

## Interpretation Limits

- Does Not Mean: transport filename progression changes semantic lineage, embedded byte preference changes Workspace authority, Markdown Preview becomes durable authority, or this progression carrier is itself the stable Major
- Must Not Be Used To Claim: remote-write authority, publication readiness, release readiness, or Task closure before Sigma returns disposition and the explicit stable Major succeeds
- Authority Limits: Core owns carrier/Tooling qualification; Workspace and artifact authority remain unchanged; VS Code only projects the qualified behavior described above
- Transport Limits: this one Handoff Package plus exact Tooling routing is the recipient/recovery surface; prior chat is not required context

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md](007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md)
  - Value: NPCAHRoAI1kXK9R9tmKMBnHvI2MnknEtszfSuZZlrd4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: gtXQii5qeUe7QU0OHxRctUlQTFNcIpczM_AIIky4kuI