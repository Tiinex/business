# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 20:07:53
  - Trace: [006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md](../006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
  - Origin:
    - [relative](../006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 20:08:22
  - Authors: Kodax
  - Why: The parity-only correction is required to stop and return when canonical rebuild exposes a new exact source defect rather than broadening source semantics.
  - Summary: Return the unchanged accepted VS Code/Core frontier with the exact newly exposed VS Code-local TypeScript build blocker.
  - Status: ready/local

---

# Kodax To Anchor — Tooling Major 008 Emitted Runtime Build Blocker Return

## Handoff Parties

- Purpose: return the exact accepted Tooling Major 008 VS Code/Core frontier unchanged because the bounded emitted-runtime parity correction hit a new exact internal VS Code source-contract blocker before any durable output correction could be safely landed.
- From: Kodax
- From Kind: role
- From Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Transfers

- reconcile-vscode-source-contract-blocker
  - Transfer Kind: work-and-responsibility
  - Description: reconcile the exact accepted VS Code source mismatch where `projectHandoffLeaves` is typed as `HandoffLeavesResult` without `findings`, while `src/packageBuilder.ts` reads `projected.findings` during route projection. The parity-only Kodax tranche intentionally made no semantic source change.
  - Controlling Artifact: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Boundary: determine and authorize the smallest source-contract correction before asking Kodax to regenerate emitted runtime; do not reopen Core semantics or Package V1 from this blocker alone.

- rerun-emitted-runtime-parity-after-source-reconciliation
  - Transfer Kind: work
  - Description: after the exact VS Code source-contract mismatch is reconciled under appropriate authority, rerun the repository-owned build and require zero missing/stale JS outputs, 117/117 bridge cases, 4/4 package integration, then continue to the real Extension Host gate.
  - Controlling Artifact: [Kodax Emitted Runtime Canonical Build Blocker Evidence](business::.topics/initiatives/006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
  - Boundary: no parity PASS or Sigma promotion exists in this return.

## Required Context

- blocker-evidence
  - Material: exact Kodax Evidence for the canonical-build environment gate, internal source-contract mismatch, and byte-preservation receipt.
  - Material Reference: [Kodax Emitted Runtime Canonical Build Blocker Evidence](business::.topics/initiatives/006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
  - Purpose: precise blocker identity and proof that no VS Code/Core source or durable runtime bytes were changed.
  - Availability: available

- controlling-task
  - Material: exact Anchor parity-correction Task and its stop-on-new-source-defect boundary.
  - Material Reference: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Purpose: bounded scope and Done Criteria.
  - Availability: available

- accepted-vscode-source
  - Material: exact unchanged accepted VS Code Workspace containing the original two emitted-runtime parity defects and the newly exposed internal type-contract mismatch.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: unchanged source frontier for Anchor reconciliation and subsequent bounded rebuild.
  - Availability: available

- accepted-core
  - Material: exact unchanged accepted shared Core Workspace.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: read-only shared dependency; no Core change is requested by this return.
  - Availability: available

## Reference Context

- prior-anchor-parity-evidence
  - Material: Anchor fan-in Evidence that isolated the original two emitted-runtime parity defects before this build correction.
  - Material Reference: [Anchor Emitted Runtime Parity Blocker Evidence](business::.topics/initiatives/005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md)
  - Purpose: preserve the exact original parity-defect identity separately from the newly exposed source-contract blocker.
  - Availability: available

- major-contract
  - Material: complete Tooling Major 008 product contract and non-regression invariants.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: preserve accepted Handoff UX, shared-Core ownership and Package V1 boundaries while the build blocker is reconciled.
  - Availability: available

## Retained Responsibilities

- source-authority-reconciliation
  - Retained By: Anchor
  - Responsibility: decide the bounded authority and exact correction for the VS Code-local `HandoffLeavesResult` / `projected.findings` type-contract mismatch before emitted-runtime regeneration resumes.
  - Boundary: this blocker does not establish authority for Kodax to widen the parity-only tranche into source semantics.

- shared-core-semantics
  - Retained By: accepted Core frontier / Loom
  - Responsibility: retain canonical Core Handoff/Package semantics unchanged unless a separately qualified shared-Core defect is established.
  - Boundary: this return presents no such Core defect.

- human-acceptance
  - Retained By: Sigma
  - Responsibility: remain downstream of deterministic build/regression completion and genuine real-host acceptance.
  - Boundary: this blocked return is not Sigma promotion.

## Exclusions And Dependencies

- exact-build-toolchain
  - Kind: unresolved-dependency
  - Description: the current host lacks the repository-lock type packages required for a fully canonical TypeScript build (`@types/node` and `@types/vscode`); registry acquisition is unavailable in this execution environment.
  - Responsible Party Or Role: Anchor / capable build machine.

- internal-vscode-source-contract
  - Kind: unresolved-dependency
  - Description: exact accepted VS Code source has a local TypeScript mismatch between `HandoffLeavesResult` and `packageBuilder.ts` access to `projected.findings`; the controlling Task requires returning this blocker instead of broadening parity scope.
  - Responsible Party Or Role: Anchor for reconciliation / subsequent bounded Kodax source tranche if authorized.

- core-or-package-redesign
  - Kind: excluded-scope
  - Description: no Core source change, Package V1 redesign, endpoint/participant semantic change, cache/pointer redesign, or host-private semantic workaround is authorized by this return.
  - Responsible Party Or Role: explicit future qualified authority only.

- remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release, deployment, registry mutation, or other remote write is performed.
  - Responsible Party Or Role: explicit release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: blocked source-reconciliation return with exact VS Code/Core Workspace bytes unchanged; reconcile the exact VS Code-local type-contract blocker, then rerun the bounded emitted-runtime parity correction and deterministic acceptance before any real-host/Sigma step.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: emitted-runtime parity is complete, the known missing/stale `dist` files are accepted, Core is defective, real-host acceptance ran, or Sigma accepted Major 008.
- Must Not Be Used To Claim: authority to hand-edit generated runtime around the source mismatch, broaden Package V1/shared-Core semantics, or treat a host-only diagnostic type probe as canonical build acceptance.
- Authority Limits: exact bounded Kodax return under the selected Anchor-to-Kodax emitted-runtime parity Handoff only.
- Transport Limits: return through one canonical Tiinex Handoff package carrying Business continuity plus unchanged parent VS Code/Core Workspace snapshots.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md](../006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
  - Value: Xb0mpOfj1U2z7Ph9GrYLoQ22CdV2DPem1cpoauvNuAA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: uANTldUbL4lmEtgE1Jma2Gguu_YPz8HMa4av6kHfaC8