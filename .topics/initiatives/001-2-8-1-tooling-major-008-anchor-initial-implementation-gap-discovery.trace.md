# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 14:57:34
  - Trace: [001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md](001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Origin:
    - [relative](001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 15:22:27
  - Authors: Anchor
  - Why: Give Loom and Kodax exact pre-implementation evidence so Major 008 converges on the remaining seams without reopening package representation work.
  - Summary: Anchor isolates the current durable endpoint authoring, participant-selection and truthful-preview gaps while confirming existing Package V1 cache/pointer mechanics are reusable.
  - Status: ready/local

---

# Tooling Major 008 — Anchor Initial Implementation Gap Discovery

## Supported Claim Or Question

- Supported Claim Or Question: Which exact remaining implementation seams prevent the current accepted Package V1/Core/VS Code frontier from satisfying Tooling Major 008 without another package-format redesign?
- Evidence Role: Anchor pre-implementation discovery that narrows Loom/Core and Kodax/VS Code work to existing authoring, selection, material-closure and preview seams.

## Provenance

- Known Source: exact Business/Core/VS Code Workspaces carried by the qualified Tooling Major 008 Anchor-to-Anchor recovery package and materialized through carried Tiinex Tooling.
- Preservation Basis: the carried Workspaces remain unchanged; findings below are source observations and executable contract queries against those exact bytes.
- Provenance Limits: no specialist implementation return has yet been reconciled under Major 008; these findings identify gaps and existing reusable mechanics but do not prove the eventual repair.

## Evidence Material

- Material Kind: exact current source inspection plus Core creation-contract projection.
- Material: current Handoff creation runtime/renderer, Handoff endpoint/participant projection, Package V1 builder, VS Code authoring panel/controller, Outgoing participant/endpoint flow and prospective tree projection.

### Core durable endpoint authoring gap

- Canonical Handoff validation already recognizes optional `From Reference` and `To Reference` fields in `Handoff Parties`.
- The current Core creation contract for `tiinex.handoff.v1` exposes required `Purpose`, `From`, `From Kind`, `To`, `To Kind`, transfers/contexts and other required sections, but its creation `optionalInputs` is empty and its creation bindings omit `From Reference` and `To Reference`.
- The generic creation renderer currently treats every bound ordinary field as required at rendering time unless the contract surface is extended to represent optional ordinary bindings correctly.
- Therefore the missing durable endpoint References are currently a Core authoring-capability gap, not evidence that canonical Handoff semantics require redesign.

### Existing Core endpoint projection is already appropriately bounded

- Core `projectQualifiedHandoffEndpoints` projects exact qualified Role/Party artifacts from one explicitly bounded qualified Workspace at a time.
- It excludes nested fixture Workspaces, repository-wide scanning, cache inventory, chronology and display labels as authority.
- VS Code already has a host utility that can call this projection for explicit `(workspaceId, root)` sources and deterministically merge the exact candidates.
- The remaining authoring-discovery gap is that current VS Code endpoint catalog uses selected Outgoing Workspaces when an Outgoing exists, otherwise only the authoring Workspace, rather than all explicit operator-open Workspace roots.

### Current VS Code endpoint selection is transient

- The authoring panel can present endpoint suggestions and records exact endpoint selections when candidates exist.
- The authoring submission sends only ordinary field values into Core draft creation and does not persist exact selected endpoint References in the authored Handoff.
- Immediate create-and-attach converts endpoint selections into transient Outgoing endpoint-role bindings.
- Attaching an existing Handoff does not carry those transient endpoint bindings, so restart/re-attach cannot recover exact endpoint Role material unless the Handoff itself contains canonical References.
- This confirms that host session state currently participates in correctness and must be removed from that role.

### Current participant UI is confirmation, not Major 008 explicit selection

- Current VS Code participant flow asks the operator to confirm the exact participant set that Core already semantically projected.
- Weakening or changing that set is rejected; if Core projects no semantic participants, VS Code reports no additional participants.
- Tooling Major 008 instead requires an Attach-time multi-select for zero, one or multiple explicit extra participant Roles from all open qualified Workspaces.
- Presence in open/carried material must not create participation; explicit operator selection is the additional input authority.

### Package V1 pointer/cache mechanics are already reusable

- The current Package V1 builder already places Workspace trace+ZIP at one dimension, optional cache trace+ZIP below it, then builds participant pointers, endpoint pointers and finally the Handoff pointer as a numeric Parent chain.
- Cache material records already preserve exact source/target Workspace/path/reference and byte identity needed for adapter-based material resolution.
- The normal single/multi representation is already Package V1.
- Therefore Major 008 should feed durable endpoint References and explicit qualified participant selections into existing shared closure/manufacture mechanics rather than redesigning Package V1.

### Current Outgoing preview can still overclaim future pointers

- VS Code currently constructs prospective participant/endpoint pointer rows locally.
- In particular, From/To prospective pointer rows can be created from Handoff endpoint labels even when exact Role material is not qualified.
- This allows Outgoing to imply that a Role pointer will be packed although final Core manufacture has no authority to create it.
- Major 008 requires this preview to come from Core-qualified prospective package truth or to show an explicit unresolved state.

## Preservation And Fidelity

- Preservation State: no carried source byte was changed by this discovery.
- Fidelity Notes: no disposable code patch is promoted by this Evidence; specialist owners remain responsible for implementation and deterministic regression evidence.
- Known Losses: this environment does not provide Sigma real-host acceptance and this Evidence does not test the eventual end-to-end repaired flow.

## Interpretation Limits

- Does Not Prove: the exact implementation shape Loom/Kodax should choose, final cache fallback behavior, real-host usability, or Major 008 completion.
- Must Not Be Treated As: permission to reintroduce a second recipient representation, recipient/meta JSON, host-owned semantic authority, recursive repository discovery, mandatory endpoint References, or package-format redesign.
- Not Yet Used As: machine or human acceptance of Major 008.

## Review Notes

The shortest current path is a convergence path, not a representation rewrite: extend Core native authoring to preserve optional exact endpoint References, qualify explicit Attach participant selections against open Workspace candidate identities, feed both through existing material closure/Package V1 mechanics, and make VS Code a thin presentation/submission layer over those shared Core projections.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md](001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Value: pGG1b6GOIfihv1TvR8xXuymohSGoimS0jzPdVMD1-dI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: iObL5NfC6A_-PTyDCgvc44HZPKQdXMz_OX8xyumcTP4