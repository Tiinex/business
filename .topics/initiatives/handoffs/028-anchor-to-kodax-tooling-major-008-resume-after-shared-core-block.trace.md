# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 19:02:41
  - Trace: [001-2-8-2-tooling-major-008-anchor-shared-core-blocker-reconciliation-evid.trace.md](../001-2-8-2-tooling-major-008-anchor-shared-core-blocker-reconciliation-evid.trace.md)
  - Origin:
    - [relative](../001-2-8-2-tooling-major-008-anchor-shared-core-blocker-reconciliation-evid.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 19:03:06
  - Authors: Anchor
  - Why: Kodax correctly stopped on a shared-Core capability gap; Anchor has now reconciled and focused-verified Loom's bounded Core resolution.
  - Summary: Resume the remaining Major 008 VS Code UX against the accepted Core candidate that now supplies durable endpoint References and explicit participant material closure.
  - Status: ready/local

---

# Anchor To Kodax — Tooling Major 008 Resume After Shared Core Blocker Resolution

## Handoff Parties

- Purpose: resume the remaining thin VS Code half of Tooling Major 008 against the newly reconciled Core candidate that now supplies durable optional endpoint References and explicit participant/material closure, without duplicating Core semantics in the host.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- resume-endpoint-authoring-ux
  - Transfer Kind: work
  - Description: complete Handoff create/edit UX using Core-projected endpoint candidates from all explicit open Workspace roots. Qualified From/To selections must be submitted through the new Core authoring capability so the authored Handoff durably contains canonical optional References; manual/identity-less authoring remains an explicit supported choice. Reload/edit must reconstruct qualified selections from the durable Handoff References rather than transient host state.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: VS Code presents and submits exact Core-qualified identities; it does not synthesize qualified references from labels or implement a private Handoff renderer.

- resume-attach-participant-multiselect
  - Transfer Kind: work
  - Description: implement Attach-time multi-select for zero, one, or multiple extra participant Roles using Core-projected candidates from all explicit open qualified Workspaces. Preserve exact selected Workspace/artifact identity in the Core request. If a selected participant's Workspace is already in Outgoing, Core must reuse the carried Role; if its Workspace is open for discovery but excluded from Outgoing, the Role remains selectable and Core must carry only the bounded required Role material through the normal cache path.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: VS Code must not silently add the participant Workspace to Outgoing, infer participation from visibility, copy Role bytes, or construct cache material.

- resume-truthful-outgoing-preview
  - Transfer Kind: work
  - Description: make Outgoing participant/endpoint pointer expectations reflect Core-qualified prospective package truth. A Role pointer may be shown as pending only when Core has qualified the materialization; otherwise show a visible unresolved state. Single and multi-Handoff Pack must continue through the shared Package V1 Core path.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: VS Code does not own pointer filenames, Parent allocation, cache closure, material dependency rules or recipient representation.

- host-regression-evidence
  - Transfer Kind: work
  - Description: return deterministic evidence proving the complete host-side Major 008 requirements against the exact carried reconciled Core bytes: multi-root endpoint discovery without Outgoing prerequisite; identity-less option; durable endpoint Reference create/edit/reload; existing-Handoff Attach after restart without hidden endpoint state; participant multi-select including a Role from a Workspace excluded from Outgoing; Core-owned cache fallback; truthful preview; and bridge/package/host regressions preserving current Attach/Pack/Transport behavior.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: stop on the first exact missing Core/interface capability rather than recreating it in VS Code.

## Required Context

- controlling-major
  - Material: complete Tooling Major 008 acceptance contract and MUST NOT invariants.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: normative product behavior, machine acceptance and non-regression boundary.
  - Availability: available

- anchor-core-reconciliation
  - Material: Anchor evidence that the shared Core blocker reported by Kodax is resolved by the exact carried Core candidate and independently focused-tested.
  - Material Reference: [Anchor Shared Core Blocker Reconciliation Evidence](business::.topics/initiatives/001-2-8-2-tooling-major-008-anchor-shared-core-blocker-reconciliation-evid.trace.md)
  - Purpose: establish why Kodax may resume instead of building a host workaround.
  - Availability: available

- kodax-blocker
  - Material: Kodax's exact first-blocker evidence proving why the previous host implementation correctly stopped before source mutation.
  - Material Reference: [Kodax Shared Core Endpoint Authoring Blocker](business::.topics/initiatives/003-tooling-major-008-kodax-shared-core-endpoint-authoring-blocker.trace.md)
  - Purpose: retain the original boundary that host code must not replace shared Core authoring semantics.
  - Availability: available

- current-core
  - Material: exact reconciled Loom Core Workspace carried in this package.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: shared Core authoring, participant projection, material closure, pointer lineage and Package V1 capability to consume.
  - Availability: available

- current-vscode
  - Material: exact unchanged VS Code Workspace from the common parent.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: Kodax-owned implementation surface.
  - Availability: available

## Reference Context

- original-kodax-assignment
  - Material: original full Major 008 VS Code assignment; this resume Handoff narrows only the dependency state, not its acceptance criteria.
  - Material Reference: [Original Kodax Major 008 Assignment](business::.topics/initiatives/handoffs/026-anchor-to-kodax-tooling-major-008-native-vs-code-handoff-ux.trace.md)
  - Purpose: preserve the complete intended host work and exclusions.
  - Availability: available

## Retained Responsibilities

- shared-core-semantics
  - Retained By: Loom / accepted Core frontier
  - Responsibility: canonical Handoff authoring, Role/Identity qualification, explicit participant/material closure, adapters, Package V1 lineage and manufacture semantics.
  - Boundary: Kodax consumes these capabilities and returns a blocker if another exact shared gap remains.

- architecture-reconciliation
  - Retained By: Anchor
  - Responsibility: reconcile the next Kodax return against this accepted Core frontier, run integrated acceptance and prepare Sigma only after machine criteria are green.

- human-acceptance
  - Retained By: Sigma
  - Responsibility: final real VS Code usability and behavior acceptance after integrated deterministic qualification.

## Exclusions And Dependencies

- duplicated-role-authority
  - Kind: excluded-scope
  - Description: no VS Code-maintained Role/Identity authority index, qualified-reference builder, pointer naming rule, cache materializer, or Package V1 semantic implementation.
  - Responsible Party Or Role: Kodax.

- recursive-discovery
  - Kind: excluded-scope
  - Description: no recursive repository scanning or nested fixture discovery; use explicit open Workspace roots plus Core projection.
  - Responsible Party Or Role: Kodax.

- transient-correctness
  - Kind: excluded-scope
  - Description: transient endpoint/participant host state may support UI interaction but must not be required for correctness after the durable Handoff/Attach state is established.
  - Responsible Party Or Role: Kodax.

- package-redesign
  - Kind: excluded-scope
  - Description: do not change Package V1, reintroduce recipient/meta JSON, alphabetic pseudo-dimensions, hash/source-path dimensions, or an alternate multi-route representation.
  - Responsible Party Or Role: Kodax.

- remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release, deployment or other remote mutation.
  - Responsible Party Or Role: Anchor / explicit release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return either the first exact new shared-Core/interface blocker with no host workaround, or a VS Code candidate plus deterministic Evidence satisfying the original Major 008 Kodax acceptance contract against the exact carried reconciled Core bytes.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Core machine PASS equals VS Code completion or Sigma acceptance.
- Must Not Be Used To Claim: open Workspace visibility creates participants, labels create Role authority, transient host selections replace durable Handoff References, or host tests authorize Package V1 redesign.
- Authority Limits: thin VS Code operator UX/integration work under Tooling Major 008 only.
- Transport Limits: return through one canonical Tiinex Handoff package; no invented intermediate bundles.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-8-2-tooling-major-008-anchor-shared-core-blocker-reconciliation-evid.trace.md](../001-2-8-2-tooling-major-008-anchor-shared-core-blocker-reconciliation-evid.trace.md)
  - Value: mH6uoeLkEYSoaCFLNrhW6vVJqP3z1KWo1PC1Q0SkgEA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: tUrYzPHKQHN7LkrN1ReqsZZ3BLyD95IPlOWUFbmmTh8