# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 14:57:34
  - Trace: [001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md](../001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Origin:
    - [relative](../001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 14:59:50
  - Authors: Anchor
  - Why: Conversation continuity is at risk and the remaining Handoff authoring/participant/cache/pointer work must not be reinterpreted or solved by degrading the restored Package V1/shared-Core invariants.
  - Summary: Carry the self-contained Tooling Major 008 acceptance contract and exact current Business/Core/VS Code frontier into the next Anchor without returning to the long Major 002 lineage.
  - Status: ready/local

---

# Anchor To Anchor — Tooling Major 008 Recovery

## Handoff Parties

- Purpose: continue Tooling Major 008 from the exact current Business/Core/VS Code frontier without reconstructing intent from chat history or reopening the retired Major 002 package-design path.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Transfers

- tooling-major-008
  - Transfer Kind: work-and-responsibility
  - Description: own the full implementation/reconciliation path for Tooling Major 008 until deterministic Core/VS Code qualification and Sigma real-host acceptance. Preserve the Major exactly as written; do not narrow it to a single pointer symptom or reopen package-format design.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: the controlling Task's acceptance criteria and MUST NOT invariants are normative for this work turn. Any proposed implementation that makes a criterion easier by weakening an invariant is out of scope.

- specialist-orchestration
  - Transfer Kind: responsibility
  - Description: delegate shared authoring/material/pointer semantics to Loom/Core and thin host UX/integration to Kodax/VS Code in parallel where source ownership is disjoint; reconcile exact returned bytes before Sigma.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: Kodax must not repair Core gaps with host-private semantic logic; Loom must not redesign VS Code UX or replace Package V1.

## Required Context

- controlling-major
  - Material: self-contained Tooling Major 008 acceptance contract, including endpoint discovery, durable References, Attach participant multi-select, cache rules, numeric lineage, single/multi Package V1 parity, machine gates, and Sigma gate.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: authoritative current-work objective and non-regression boundary.
  - Availability: available

- anchor-role
  - Material: canonical Anchor Role.
  - Material Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Purpose: orchestration and reconciliation boundary.
  - Availability: available

- tooling-project
  - Material: Tiinex Tooling Project.
  - Material Reference: [Tiinex Tooling](business::.topics/initiatives/001-2-tooling-project.trace.md)
  - Purpose: organizational parent and shared-Core-first implementation boundary.
  - Availability: available

- core-workspace
  - Material: exact carried current Core Workspace.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: shared implementation owner for authoring, qualification, cache/material closure, adapters, pointer lineage, and Package V1.
  - Availability: available

- vscode-workspace
  - Material: exact carried current VS Code Workspace.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: thin operator host for discovery UX, endpoint selectors, Attach participant multi-select, Outgoing presentation, Pack/Transport invocation.
  - Availability: available

## Reference Context

- previous-major-boundary
  - Material: Major 002 history remains evidence of repaired Package V1/Transport defects but is not the current work lineage.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: prevent the next Anchor from continuing the long historical grounding lineage or interpreting its local fixes as current scope.
  - Availability: available

## Retained Responsibilities

- human-acceptance
  - Retained By: Sigma
  - Responsibility: final real VS Code operator acceptance after deterministic integrated qualification.
  - Boundary: Sigma is not the routine machine test runner or implementation debugger.

- semantic-escalation
  - Retained By: semantic owner / Axiom when genuinely required
  - Responsibility: resolve only an actual canonical semantic contradiction found by implementation.
  - Boundary: absence of implementation support is not itself authority to redesign schemas or Handoff semantics.

- remote-mutation
  - Retained By: explicit release/repository authority
  - Responsibility: commit, push, publication, release, deployment, and other remote mutation.
  - Boundary: this recovery Handoff does not authorize remote mutation.

## Exclusions And Dependencies

- alternate-package-representation
  - Kind: excluded-scope
  - Description: do not introduce or reactivate a second recipient-facing Handoff package representation, recipient/meta JSON sidecar, alphabetic pointer dimensions, or source-path/hash filename lineage.
  - Responsible Party Or Role: Anchor, Loom, Kodax.

- host-private-semantic-layer
  - Kind: excluded-scope
  - Description: VS Code may keep UX/cache state but must not own semantic correctness for endpoint/participant authority, material closure, pointer lineage, or Package V1.
  - Responsible Party Or Role: Kodax.

- broad-schema-redesign
  - Kind: excluded-scope
  - Description: do not alter canonical Docs semantics unless a concrete contradiction is preserved and escalated.
  - Responsible Party Or Role: Anchor / semantic owner.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return either the first exact unresolved blocker that prevents Tooling Major 008 acceptance, or an integrated Core + VS Code candidate with deterministic machine evidence ready for Sigma real-host acceptance; after Sigma, reconcile to accepted closure or the next bounded blocker.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: the previous Major 002 is reopened, Package V1 may be redesigned, passing unit tests equals human acceptance, or carried Roles imply participant authority.
- Must Not Be Used To Claim: endpoint labels are qualified references, participant presence is inferred from carried material, full participant Workspaces must be silently added to Outgoing, or cache creates semantic authority.
- Authority Limits: implementation orchestration and reconciliation only within the exact Tooling Major 008 acceptance contract.
- Transport Limits: use canonical Tiinex Handoff packages and shared Core manufacture; no invented intermediate transport format.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md](../001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Value: pGG1b6GOIfihv1TvR8xXuymohSGoimS0jzPdVMD1-dI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: DRGvjt6Rn0hBQdTVWWIET3yuw7Js2U2YC5YIwnu2sZ8