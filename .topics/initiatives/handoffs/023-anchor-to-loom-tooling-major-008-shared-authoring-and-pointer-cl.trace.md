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
  - Created At: 2026-09-22 15:10:46
  - Authors: Anchor
  - Why: Major 008 requires Core-owned durable Handoff identity and pointer/material closure so VS Code can remain a thin operator host without semantic side channels.
  - Summary: Implement durable endpoint References, multi-root Role projection, participant/cache material closure, truthful Package V1 projection, and numeric pointer lineage in shared Core.
  - Status: ready/local

---

# Anchor To Loom — Tooling Major 008 Shared Authoring And Pointer Closure

## Handoff Parties

- Purpose: implement the shared Core half of Tooling Major 008 so qualified endpoint/participant selections become durable Tiinex Handoff/material inputs and Package V1 can materialize truthful numeric pointer lineage from carried Workspace or bounded cache without any VS Code-private semantic side-channel.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Loom
- To Kind: role
- To Reference: [Loom Role](business::.topics/roles/001-3-1-loom-canonical-holder-cutover-role.trace.md)

## Transfers

- durable-endpoint-authoring
  - Transfer Kind: work
  - Description: extend shared Core native Handoff authoring so an exact qualified endpoint selection can be written durably as canonical `From`/`From Kind`/`From Reference` and `To`/`To Kind`/`To Reference`, while preserving deliberately identity-less endpoints as valid. Reparse/reload of the authored Handoff must recover the exact qualified endpoint binding without host session state.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: do not make References mandatory; do not move authoring semantics into VS Code; do not change canonical Docs/schema meaning unless an actual contradiction is preserved and escalated.

- shared-multi-workspace-role-projection
  - Transfer Kind: work
  - Description: provide/reuse Core projection needed by hosts to discover exactly qualified Role/Identity endpoint and participant candidates from an explicit set of operator-open Workspace roots, with stable Workspace/artifact references and deterministic deduplication. Nested/non-open fixture Workspaces must not become candidates.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: explicit open roots are input authority for discovery scope only; carriage does not imply participation and display labels do not become references.

- participant-and-external-material-closure
  - Transfer Kind: work
  - Description: accept exact qualified extra participant Role selections made at Attach and resolve their Role material generically. If the Role's authoritative Workspace is already included in Outgoing, resolve from the carried Workspace. If that Workspace is open for discovery but excluded from Outgoing, carry only the bounded required Role/material through the normal cache/material ZIP and preserve exact source identity for adapter resolution. Apply the same generic rule to external Required Context such as Process/material artifacts.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: do not silently add the participant's whole Workspace to Outgoing; cache is transported material only and must not create participant/endpoint authority.

- truthful-package-projection-and-pointer-lineage
  - Transfer Kind: work
  - Description: make Core's prospective Package V1 projection and manufacture derive participant/endpoint pointer materialization from the durable Handoff plus exact qualified Attach participant selections/material closure, so host preview and final Pack agree. Required numeric Parent lineage is Workspace trace+ZIP -> optional cache trace+ZIP -> participant pointer(s) -> From pointer -> To pointer -> Handoff pointer, with natural compression when optional nodes are absent.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: Package V1 is the only normal representation. No `e`/`p` dimensions, route-path/hash filename dimensions, recipient/meta JSON, cache index JSON, or second recipient representation.

## Required Context

- controlling-major
  - Material: complete acceptance contract and non-regression invariants for Tooling Major 008.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: normative Done Criteria and MUST NOT boundaries.
  - Availability: available

- current-core
  - Material: exact carried current Core Workspace, including restored Package V1 single/multi manufacture and numeric lineage mechanics.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: implementation surface; preserve accepted Package V1 convergence.
  - Availability: available

- current-vscode
  - Material: exact carried current VS Code Workspace for interface-contract awareness only.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: ensure shared Core operations are consumable by the thin host without implementing host UI.
  - Availability: available

## Reference Context

- prior-package-convergence
  - Material: prior Major 002 recovery established Package V1 as the single normal recipient-facing representation and restored numeric Workspace/cache/pointer lineage.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: historical non-regression context only; Major 008 is the current work authority and the long Major 002 lineage is not reopened.
  - Availability: available

## Retained Responsibilities

- vscode-operator-ux
  - Retained By: Kodax
  - Responsibility: endpoint dropdowns, participant multi-select, open-root host context, edit/reload UI, truthful Outgoing presentation, and thin invocation of Core operations.
  - Boundary: Loom must not implement VS Code-private behavior or make Core depend on VS Code types/state.

- architecture-reconciliation
  - Retained By: Anchor
  - Responsibility: protect Major 008 invariants, reconcile Loom/Kodax bytes, run integrated acceptance, and prepare Sigma gate.

- human-acceptance
  - Retained By: Sigma
  - Responsibility: real VS Code operator acceptance only after deterministic integrated machine qualification.

## Exclusions And Dependencies

- alternate-recipient-representation
  - Kind: excluded-scope
  - Description: do not revive artifact-first Phase 2 or any other normal recipient package path. Route count must not select a package standard.
  - Responsible Party Or Role: Loom.

- host-private-authority
  - Kind: excluded-scope
  - Description: do not design a solution that requires `endpointSelections`, `OutgoingDraft.endpointRoles`, or similar host-only state for semantic correctness after Handoff authoring/reload.
  - Responsible Party Or Role: Loom/Kodax.

- schema-redesign
  - Kind: excluded-scope
  - Description: existing canonical References and Handoff semantics are presumed sufficient. If a true contradiction exists, return it exactly rather than widening schemas locally.
  - Responsible Party Or Role: Loom/Anchor.

- remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release, deployment, or other remote mutation.
  - Responsible Party Or Role: Anchor / explicit release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return either the first exact Core blocker/semantic contradiction, or a bounded Core candidate with deterministic Evidence proving: qualified endpoint selection authors durable canonical References; identity-less authoring remains valid; reload/reparse recovers References; existing Handoff can drive endpoint materialization without host side-channel state; multiple explicit participant selections resolve across carried/open Workspaces with cache fallback; generic external Required Context cache resolution works; prospective projection matches final Package V1; numeric cache/participant/from/to/handoff Parent lineage is exact; single and multi use the same normal Package V1 builder; and no recipient/meta JSON or pseudo-dimension representation is introduced.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Roles present in carried material are automatic participants, labels are qualified references, cache creates authority, or Loom may redesign Package V1.
- Must Not Be Used To Claim: unit-only success equals VS Code usability or Sigma acceptance.
- Authority Limits: shared Core implementation and qualification under Tooling Major 008 only.
- Transport Limits: return through one canonical Tiinex Handoff package; no invented intermediate bundles.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md](../001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Value: pGG1b6GOIfihv1TvR8xXuymohSGoimS0jzPdVMD1-dI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: mZgWa0GeX_BTNTZ3KrFkCl-xTLKM2fmtP4aGlBRblIo