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
  - Created At: 2026-09-22 20:17:16
  - Authors: Anchor
  - Why: Kodax correctly stopped on a VS Code-local type-contract mismatch; Anchor has now resolved its authority and exact bounded correction without changing semantics.
  - Summary: Apply the exact authorized HandoffLeavesResult findings type reconciliation and resume canonical emitted-runtime parity under the existing Major 008 Task.
  - Status: ready/local

---

# Anchor To Kodax — Tooling Major 008 Emitted Runtime Parity Resume

## Handoff Parties

- Purpose: apply the exact authorized VS Code-local `HandoffLeavesResult.findings` type-surface reconciliation, then resume the existing emitted-runtime parity correction and deterministic acceptance without changing Major 008 semantics.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- apply-bounded-vscode-type-contract-correction
  - Transfer Kind: work-and-responsibility
  - Description: in `src/tiinex/bootstrap.ts`, add the optional `findings?: Array<{ severity: string; code: string; message: string }>;` property to `HandoffLeavesResult` exactly as authorized by the controlling Decision. Do not change runtime projection behavior or packageBuilder error handling.
  - Controlling Artifact: [Handoff Leaves Result Findings Contract Reconciliation](business::.topics/initiatives/006-1-tooling-major-008-handoff-leaves-result-findings-contract-decision.trace.md)
  - Boundary: one VS Code-local TypeScript contract reconciliation only; no Core, Package V1, endpoint/participant/cache/pointer semantic change.

- resume-emitted-runtime-parity-correction
  - Transfer Kind: work
  - Description: after the exact source correction, rerun the repository-owned build for the current accepted VS Code source frontier, restore zero missing/stale emitted JS outputs, then run the original 117/117 bridge and 4/4 package integration gates against the exact accepted Core frontier.
  - Controlling Artifact: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Boundary: generated output must come from the repository-owned build path; do not hand-author `dist` files around unavailable dependencies or compile blockers.

## Required Context

- contract-decision
  - Material: exact Anchor Decision resolving the internal `HandoffLeavesResult` / `projected.findings` mismatch.
  - Material Reference: [Handoff Leaves Result Findings Contract Reconciliation](business::.topics/initiatives/006-1-tooling-major-008-handoff-leaves-result-findings-contract-decision.trace.md)
  - Purpose: exact source-change authority and non-semantic boundary.
  - Availability: available

- kodax-blocker-evidence
  - Material: exact prior build blocker Evidence proving unchanged VS Code/Core bytes and identifying the missing external type packages plus internal type mismatch.
  - Material Reference: [Kodax Emitted Runtime Canonical Build Blocker Evidence](business::.topics/initiatives/006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
  - Purpose: preserve the blocker basis and prove this resume does not rewrite history.
  - Availability: available

- controlling-task
  - Material: original emitted-runtime parity Task, including zero missing/stale output, 117/117 bridge, 4/4 package integration and no-semantic-broadening criteria.
  - Material Reference: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Purpose: completion gate after source reconciliation.
  - Availability: available

- major-contract
  - Material: Tooling Major 008 product contract and all MUST/MUST NOT acceptance criteria.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: keep all work in the same active Major and prevent package/semantic drift.
  - Availability: available

- accepted-core
  - Material: exact accepted Core Workspace carried unchanged in this return/resume frontier.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: read-only shared dependency for integration tests.
  - Availability: available

- accepted-vscode
  - Material: exact unchanged VS Code Workspace returned by Kodax before this source-contract Decision.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: source frontier to correct and canonically rebuild.
  - Availability: available

## Reference Context

- prior-anchor-parity-evidence
  - Material: Anchor Evidence that isolated the original missing/stale emitted-runtime files before the source-contract blocker was exposed.
  - Material Reference: [Anchor Emitted Runtime Parity Blocker Evidence](business::.topics/initiatives/005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md)
  - Purpose: preserve the original parity target separately from this source-contract reconciliation.
  - Availability: available

## Retained Responsibilities

- final-integrated-core-package-acceptance
  - Retained By: Anchor
  - Responsibility: after Kodax return, independently verify emitted-runtime parity and directly test shared Core Handoff/package behavior before any Sigma carrier is manufactured.
  - Boundary: Kodax regression receipts do not replace Anchor Core/package acceptance.

- real-host-sigma-acceptance
  - Retained By: Anchor / Sigma
  - Responsibility: real Extension Host and human acceptance remain downstream of deterministic source/build/package gates.
  - Boundary: this Handoff cannot close Major 008.

## Exclusions And Dependencies

- core-or-package-redesign
  - Kind: excluded-scope
  - Description: do not modify Core, Package V1 representation, pointer lineage, Role/participant semantics, cache/material semantics, recipient representation, or transport semantics.
  - Responsible Party Or Role: Kodax.

- host-private-authority
  - Kind: excluded-scope
  - Description: do not restore transient endpoint/participant semantic authority or duplicate Core qualification logic in VS Code.
  - Responsible Party Or Role: Kodax.

- external-build-dependencies
  - Kind: unresolved-dependency
  - Description: canonical build requires exact repository-lock TypeScript 5.7.2, `@types/node` 22.10.2 and `@types/vscode` 1.95.0. Acquire them only as ordinary local build dependencies if the execution environment permits; do not mutate registries or claim canonical build success using substitutes.
  - Responsible Party Or Role: Kodax / execution host.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, release, publication, deployment or registry mutation is authorized.
  - Responsible Party Or Role: explicit release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return one qualified Kodax-to-Anchor Handoff with the exact authorized source contract correction, canonical emitted runtime parity restored, unchanged Core, full parity audit, 117/117 bridge and 4/4 package integration green; otherwise return only the next exact bounded blocker without semantic broadening.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Major 008 is complete, Core/package acceptance is delegated to Kodax, Sigma acceptance has occurred, or a new package representation is permitted.
- Must Not Be Used To Claim: a type declaration change creates semantic authority; the authority comes from the existing Core operation contract and the controlling Major 008 artifacts.
- Authority Limits: exact VS Code-local source-contract reconciliation plus continuation of the already-authorized emitted-runtime parity Task.
- Transport Limits: one canonical Package V1 carrier with current Business and exact accepted Core/VS Code snapshots.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md](../005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Value: 7SQfn4iWGkM48eceRMLm2SCwgWTTN4DTIS879JQrKfw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: O2aBPnKKEJtMajT2h1A5sL9RzIh8FVWSQMERetEmN_s