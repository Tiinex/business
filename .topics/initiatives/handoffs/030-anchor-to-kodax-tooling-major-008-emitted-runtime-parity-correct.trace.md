# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 19:54:25
  - Trace: [005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md](../005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Origin:
    - [relative](../005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 19:55:09
  - Authors: Anchor
  - Why: The source implementation is provisionally green, but the carried runtime has one missing and one stale generated module that block real-host acceptance.
  - Summary: Restore durable VS Code emitted-runtime parity for the exact accepted Major 008 source frontier without semantic broadening.
  - Status: ready/local

---

# Anchor To Kodax — Tooling Major 008 Emitted Runtime Parity Correction

## Handoff Parties

- Purpose: correct the final durable VS Code emitted-runtime parity blocker on the already accepted Tooling Major 008 source frontier, without reopening Core semantics, Package V1, Role/participant behavior, or host authority boundaries.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- emitted-runtime-parity-correction
  - Transfer Kind: work-and-responsibility
  - Description: use the repository-owned VS Code build path to make the durable emitted runtime match the exact accepted Major 008 source frontier. The known blocker is exactly one missing emitted module (`dist/core/handoffEndpointSelection.js`) and one stale emitted module (`dist/core/workspaceChoice.js`) before canonical rebuild; do not broaden source semantics unless the canonical build exposes a new exact source defect.
  - Controlling Artifact: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Boundary: build/output parity only; shared Core, Package V1, endpoint/participant semantics, cache/material closure and source authority remain unchanged.

## Required Context

- controlling-task
  - Material: exact bounded correction Task and its acceptance/exclusion criteria.
  - Material Reference: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Purpose: exact work scope and Done Criteria.
  - Availability: available

- anchor-blocker-evidence
  - Material: Anchor fan-in Evidence proving the exact source/dist mismatch and disposable integrated green result once emitted runtime matches source.
  - Material Reference: [Anchor Emitted Runtime Parity Blocker Evidence](business::.topics/initiatives/005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md)
  - Purpose: precise defect identity, parity audit and integration receipts.
  - Availability: available

- major-contract
  - Material: complete Tooling Major 008 product contract and non-regression invariants.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: preserve the accepted end-to-end Handoff UX and Package V1 boundaries.
  - Availability: available

- accepted-core
  - Material: exact accepted shared Core Workspace, byte-identical through the Kodax return.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: read-only dependency for deterministic regressions.
  - Availability: available

- accepted-vscode-source
  - Material: exact current VS Code Workspace containing the accepted Major 008 source implementation and inconsistent emitted runtime.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: canonical source frontier whose emitted output must be repaired.
  - Availability: available

## Reference Context

- kodax-final-convergence
  - Material: prior Kodax implementation Evidence/return whose source behavior is provisionally accepted and whose real-host gate remains pending.
  - Material Reference: [Kodax Final VS Code Shared-Core Convergence Evidence](business::.topics/initiatives/004-tooling-major-008-kodax-final-vs-code-shared-core-convergence-ev.trace.md)
  - Purpose: implementation provenance and original regression claims.
  - Availability: available

## Retained Responsibilities

- integrated-reconciliation
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: re-run source/dist parity, 117/117 bridge, 4/4 package integration and focused Core Major 008 regressions on the exact return; manufacture the real-host/Sigma carrier only after deterministic acceptance.
  - Boundary: Kodax does not claim integrated or human acceptance.

- shared-core-semantics
  - Retained By: Loom / accepted Core frontier
  - Responsibility: canonical authoring, Role/participant/material closure, cache semantics, pointer lineage and Package V1 manufacture remain unchanged.
  - Boundary: no Core source change is requested.

- real-host-human-acceptance
  - Retained By: Anchor / Sigma
  - Responsibility: real VS Code Extension Host machine gate and later Sigma usability acceptance remain after deterministic parity correction.
  - Boundary: deterministic tests are not real-host acceptance.

## Exclusions And Dependencies

- no-semantic-broadening
  - Kind: excluded-scope
  - Description: do not change accepted endpoint/participant discovery, durable Reference semantics, cache/material closure, Package V1, pointer lineage or host authority merely to obtain runtime parity.
  - Responsible Party Or Role: Kodax.

- no-core-mutation
  - Kind: excluded-scope
  - Description: Core is read-only for this correction.
  - Responsible Party Or Role: Kodax.

- no-recipient-meta-layer
  - Kind: excluded-scope
  - Description: no alternate recipient representation, recipient/meta JSON, cache index or host-private semantic layer may be introduced.
  - Responsible Party Or Role: Kodax.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, release, publication, deployment or registry mutation is authorized.
  - Responsible Party Or Role: explicit release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return one qualified Kodax-to-Anchor Handoff carrying the exact accepted source frontier with durable emitted runtime parity restored, unchanged Core, complete parity audit and deterministic regressions green; if canonical build exposes any new source defect, stop and return that exact blocker instead of broadening scope.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Major 008 is complete, real Extension Host execution passed, Sigma accepted the UX, or Published Core is registry-accepted.
- Must Not Be Used To Claim: build parity grants semantic authority or permits package redesign.
- Authority Limits: exact VS Code emitted-runtime parity correction under the selected Major 008 Task only.
- Transport Limits: return through one canonical Package V1 Tiinex Handoff carrier with current Business, unchanged Core and corrected VS Code Workspace.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md](../005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Value: 7SQfn4iWGkM48eceRMLm2SCwgWTTN4DTIS879JQrKfw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 9Srle8q2Xm9EFa-r9a590aWCOBbjVCqqN5PjIrFDDVE