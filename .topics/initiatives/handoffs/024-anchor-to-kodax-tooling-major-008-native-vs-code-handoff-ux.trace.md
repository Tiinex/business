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
  - Created At: 2026-09-22 15:11:59
  - Authors: Anchor
  - Why: Major 008 requires the operator-friendly VS Code flow to consume shared Core authority rather than replacing it with free text or transient host-private semantic state.
  - Summary: Restore Core-backed endpoint selectors, Attach participant multi-select across open Workspaces, durable edit/reload UX, and truthful Outgoing projection without duplicated host semantics.
  - Status: ready/local

---

# Anchor To Kodax — Tooling Major 008 Native VS Code Handoff UX

## Handoff Parties

- Purpose: implement the thin VS Code half of Tooling Major 008 so endpoint/participant selection is easy for operators but all Role/Identity authority, durable Handoff References, material closure, pointer lineage, and Package V1 truth remain Core-owned.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- endpoint-authoring-ux
  - Transfer Kind: work
  - Description: restore clear From/To endpoint selectors for Handoff create/edit using Core-projected qualified Role/Identity candidates from all explicit open Workspace roots. Normal qualified selection should not require the operator to type `From Kind`/`To Kind`; manual/identity-less authoring must remain an explicit supported option. Selected qualified endpoints must be passed to Core authoring so the resulting Handoff artifact contains durable canonical References and edit/reload can reconstruct the UI selection from those References.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: VS Code presents and submits qualified Core selections; it must not synthesize qualified references from labels or implement its own Role authority rules.

- attach-participant-multiselect
  - Transfer Kind: work
  - Description: when attaching a Handoff to Outgoing, present a multi-select for zero, one, or multiple extra participant Roles using Core-projected candidates from the same explicit multi-Workspace operator context. Preserve exact selected Workspace/artifact identity when invoking Core. A selected participant whose authoritative Workspace is not included in Outgoing must remain selectable; Core decides the bounded cache/material closure rather than VS Code silently adding that Workspace.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: presence in an open/carried Workspace does not imply participation. Only explicit operator selections are submitted as participant input; VS Code must not copy Role bytes or construct cache contents itself.

- open-workspace-discovery
  - Transfer Kind: work
  - Description: build endpoint/participant discovery context from exactly `vscode.workspace.workspaceFolders` / explicit operator-open qualified Workspace roots, call shared Core projection, and present deterministic deduplicated candidates with enough Workspace/provenance context to distinguish same-label Roles. No Outgoing context may be required merely to discover authoring endpoints.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: no recursive repository scanning, no nested fixture discovery, no host-private Role index.

- truthful-outgoing-preview
  - Transfer Kind: work
  - Description: render Outgoing participant/endpoint pointer expectations from Core-qualified prospective package projection rather than optimistic labels. If Core cannot materialize a Role pointer, display the unresolved state explicitly instead of showing a false `pending Pack` pointer. Pack single/multi through the shared Core path only.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: VS Code does not own pointer filenames, Parent allocation, cache closure, material dependency rules, or package representation.

## Required Context

- controlling-major
  - Material: complete Tooling Major 008 acceptance contract and MUST NOT invariants.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: normative user flow, machine acceptance, and non-regression boundary.
  - Availability: available

- current-vscode
  - Material: exact carried current VS Code Workspace.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: implementation surface for operator UX and host integration.
  - Availability: available

- current-core
  - Material: exact carried current Core Workspace; Loom is concurrently extending shared authoring/material/pointer capabilities under the same Major.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: shared interface authority; Kodax may expose a precise missing Core capability as a blocker but must not permanently reimplement it in host code.
  - Availability: available

## Reference Context

- prior-vscode-boundary
  - Material: previous Major 002 work repaired Attach, Workspace-root scoping, Package V1 convergence, and Transport mechanics but left Handoff endpoint authoring and durable pointer closure incomplete.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: historical non-regression context only; do not reopen old package-format work.
  - Availability: available

## Retained Responsibilities

- shared-core-semantics
  - Retained By: Loom
  - Responsibility: reusable endpoint authoring, Role/Identity qualification, participant/material closure, adapters, prospective package projection, pointer lineage, and Package V1 mechanics.
  - Boundary: Kodax must not hide a Core gap with a permanent VS Code-private semantic layer.

- architecture-reconciliation
  - Retained By: Anchor
  - Responsibility: reconcile Loom/Kodax exact bytes, resolve interface seams, run integrated machine acceptance, and prepare Sigma gate.

- human-acceptance
  - Retained By: Sigma
  - Responsibility: final real VS Code usability/behavior acceptance after integrated deterministic qualification.

## Exclusions And Dependencies

- duplicated-role-authority
  - Kind: excluded-scope
  - Description: do not create a VS Code-maintained Role/Identity authority index, qualified-reference builder, pointer naming rule, cache materializer, or Package V1 semantic implementation.
  - Responsible Party Or Role: Kodax.

- recursive-discovery
  - Kind: excluded-scope
  - Description: do not discover endpoints/participants by recursively scanning repository trees or nested test fixtures. Discovery is scoped to explicit open Workspace roots and Core qualification.
  - Responsible Party Or Role: Kodax.

- optimistic-pointer-preview
  - Kind: excluded-scope
  - Description: do not show prospective Role/participant pointers based only on labels or transient selections when Core has not qualified actual materialization.
  - Responsible Party Or Role: Kodax.

- package-redesign
  - Kind: excluded-scope
  - Description: do not change Package V1, reintroduce recipient/meta JSON, alphabetic pseudo-dimensions, or alternate multi-route representation.
  - Responsible Party Or Role: Kodax/Loom.

- remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release, deployment, or other remote mutation.
  - Responsible Party Or Role: Anchor / explicit release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return either the first exact missing shared-Core capability/interface blocker, or a VS Code candidate with deterministic Evidence proving: endpoint dropdowns from all explicit open Workspace roots without an Outgoing prerequisite; manual identity-less option; qualified selection submitted to Core and durable Reference displayed after reload/edit; existing Handoff can Attach after restart without hidden endpoint state; Attach offers multi-select for multiple extra participant Roles across open Workspaces; a participant remains selectable when its Workspace is excluded from Outgoing; VS Code delegates that material closure to Core; Outgoing preview is Core-truthful; and bridge/package/extension-host regressions preserve current Attach/Pack/Transport behavior without duplicated semantic logic.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: selecting a Role in UI alone creates semantic authority, open Workspaces imply participants, or host state may replace durable Handoff References.
- Must Not Be Used To Claim: unit tests replace Sigma real-host acceptance or VS Code may compensate for an unresolved Core semantic capability by copying Core logic.
- Authority Limits: VS Code operator UX/integration under Tooling Major 008 only.
- Transport Limits: return through one canonical Tiinex Handoff package; no invented intermediate bundles.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md](../001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Value: pGG1b6GOIfihv1TvR8xXuymohSGoimS0jzPdVMD1-dI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: o0B2RcPmwHIyyW57U1AY-5Di5pHIwolCGET20kTyQ2s