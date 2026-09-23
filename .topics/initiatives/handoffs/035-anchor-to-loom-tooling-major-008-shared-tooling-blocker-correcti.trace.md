# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 21:56:04
  - Trace: [009-1-tooling-major-008-real-role-projection-and-clean-cache-path-corr.trace.md](../009-1-tooling-major-008-real-role-projection-and-clean-cache-path-corr.trace.md)
  - Origin:
    - [relative](../009-1-tooling-major-008-real-role-projection-and-clean-cache-path-corr.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 21:56:40
  - Authors: Anchor
  - Why: Anchor direct Tooling acceptance found two shared Core defects that must be fixed before canonical VS Code parity and Sigma.
  - Summary: Correct real canonical Role projection and clean endpoint cache path identity in shared Core while preserving Package V1 and all Major 008 invariants.
  - Status: ready/local

---

# Anchor To Loom — Tooling Major 008 Shared Tooling Blocker Correction

## Handoff Parties

- Purpose: correct the two exact shared Core/Tooling defects found by Anchor before Sigma: real canonical Role projection is empty because runtime schema-lineage source authority is unqualified, and endpoint cache entries leak execution-host absolute paths.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Loom
- To Kind: role
- To Reference: [Loom Role](business::.topics/roles/001-3-1-loom-canonical-holder-cutover-role.trace.md)

## Transfers

- correct-real-role-projection
  - Transfer Kind: work-and-responsibility
  - Description: make shared Core/Tooling qualify and project the actual current canonical Role artifacts from explicitly supplied Workspace roots, resolving the observed Role->Party schema-lineage source-authority contradiction without weakening qualification or moving discovery semantics into VS Code.
  - Controlling Artifact: [Real Role Projection And Clean Cache Path Correction](business::.topics/initiatives/009-1-tooling-major-008-real-role-projection-and-clean-cache-path-corr.trace.md)
  - Boundary: if same-snapshot relative Parent versus historic browse/git origin authority cannot be resolved from existing canonical semantics, stop with a precise Axiom blocker rather than guessing or editing Docs.

- correct-clean-cache-path-identity
  - Transfer Kind: work-and-responsibility
  - Description: ensure all recipient cache entry paths, including From/To endpoint Roles supplied by material bindings, derive from qualified Workspace/provenance/artifact identity and never from the absolute execution-time sourcePath.
  - Controlling Artifact: [Real Role Projection And Clean Cache Path Correction](business::.topics/initiatives/009-1-tooling-major-008-real-role-projection-and-clean-cache-path-corr.trace.md)
  - Boundary: preserve the existing Package V1 structure and numeric Workspace -> cache -> participant -> From -> To -> Handoff Parent lineage.

## Required Context

- direct-tooling-evidence
  - Material: Anchor direct Tooling acceptance proving durable Handoff References, explicit participant bounded cache and exact desired numeric pointer lineage while reproducing both current blockers.
  - Material Reference: [Anchor Direct Tooling Acceptance And Two Core Blockers](business::.topics/initiatives/009-tooling-major-008-anchor-direct-tooling-acceptance-and-two-core.trace.md)
  - Purpose: exact reproduction evidence, observed source-authority contradiction and bad/good cache path examples.
  - Availability: available

- major-contract
  - Material: complete Major 008 acceptance criteria and non-regression invariants.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: architectural boundary and final acceptance authority.
  - Availability: available

- accepted-core
  - Material: exact current carried Core Workspace whose shared Tooling was used for the direct acceptance run.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: implementation source and test authority.
  - Availability: available

- real-role-material
  - Material: exact current Business Workspace containing the canonical Sigma, Anchor and Loom Role artifacts that reproduce the projection problem.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: realistic Role projection and cache-path regression material.
  - Availability: available

## Reference Context

- open-vscode-parity-task
  - Material: canonical VS Code emitted-runtime parity remains open and is not replaced by this Core correction.
  - Material Reference: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Purpose: preserve current acceptance ordering after Core returns.
  - Availability: available

## Retained Responsibilities

- shared-tooling-reacceptance
  - Retained By: Anchor
  - Responsibility: after Loom returns, rerun the same direct Tooling operator flow and inspect real Role projection plus actual mixed endpoint/participant cache tree before accepting the Core correction.
  - Boundary: Loom tests do not substitute Anchor reconciliation.

- vscode-parity-and-sigma
  - Retained By: Anchor
  - Responsibility: only after shared Tooling is clean, finish canonical VS Code emitted-runtime parity and then manufacture Sigma acceptance carrier.
  - Boundary: Sigma must not be first observer of shared Core/package defects.

## Exclusions And Dependencies

- package-redesign
  - Kind: excluded-scope
  - Description: no second recipient representation, recipient/meta JSON, cache index, e/p/hash pseudo-dimensions or Package V1 lineage redesign.
  - Responsible Party Or Role: none under this Handoff.

- qualification-weakening
  - Kind: excluded-scope
  - Description: do not bypass or relax Role qualification just to populate dropdown candidates; correct the exact authority-resolution defect or return an Axiom blocker.
  - Responsible Party Or Role: none under this Handoff.

- vscode-source
  - Kind: excluded-scope
  - Description: do not modify VS Code source/dist as part of this Core correction.
  - Responsible Party Or Role: Kodax/Anchor after Core acceptance.

## Completion Expectation

- Signal Kind: custom
- Signal Meaning: return when both shared Core blockers are corrected with focused realistic regression evidence, or return a precise semantic/Axiom blocker if canonical schema authority cannot be resolved without changing semantics.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Major 008 is complete, canonical VS Code build parity is complete, or Sigma acceptance may begin without Anchor Tooling reacceptance.
- Must Not Be Used To Claim: authority for package redesign, host-private semantics, generalized schema weakening, or Docs mutation.
- Authority Limits: exact Core work defined by the controlling Major 008 microtask only.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [009-1-tooling-major-008-real-role-projection-and-clean-cache-path-corr.trace.md](../009-1-tooling-major-008-real-role-projection-and-clean-cache-path-corr.trace.md)
  - Value: XzQTGVPOvWPyZh_O9dR4wtmPh_pnwbCaIktjpLvheqI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: iTxOCD7O-6ULjE-vBv8AipzfK8hCGh2rPwVKScVKQO4