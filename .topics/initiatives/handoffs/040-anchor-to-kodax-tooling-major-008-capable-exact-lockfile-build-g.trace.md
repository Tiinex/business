# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-23 13:59:21
  - Trace: [012-tooling-major-008-anchor-exact-frontier-build-gate-reconciliatio.trace.md](../012-tooling-major-008-anchor-exact-frontier-build-gate-reconciliatio.trace.md)
  - Origin:
    - [relative](../012-tooling-major-008-anchor-exact-frontier-build-gate-reconciliatio.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-23 14:01:25
  - Authors: Anchor
  - Why: The prior Kodax run proved only an execution-environment dependency blocker; the exact Core/VS Code frontiers are unchanged and the same bounded technical gate must now run on a capable host.
  - Summary: Resume the unchanged VS Code canonical runtime gate on a capable exact-lockfile host and return deterministic build/test evidence to Anchor.
  - Status: ready/local

---

## Handoff Parties

- Purpose: resume Tooling Major 008 canonical VS Code emitted-runtime parity on a capable exact-lockfile execution host while preserving the already-accepted shared Core/Tooling semantics and keeping Sigma real-host acceptance downstream of deterministic machine gates.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- execute-exact-lockfile-build-on-capable-host
  - Transfer Kind: work-and-responsibility
  - Description: use a host that can acquire the exact VS Code repository lockfile dependencies and run the repository-owned build from the exact carried VS Code frontier. A human operator may provide local filesystem/network/terminal execution capability, but Kodax remains responsible for interpreting the technical receipts and returning bounded technical Evidence.
  - Controlling Artifact: [Anchor Exact-Frontier Build Gate Reconciliation](business::.topics/initiatives/012-tooling-major-008-anchor-exact-frontier-build-gate-reconciliatio.trace.md)
  - Boundary: exact lockfile authority only; do not use TypeScript 5.8.3 or another substitute compiler, hand-author `dist`, weaken package versions, or mutate shared Core/package semantics.

- prove-canonical-emitted-runtime-parity
  - Transfer Kind: work-and-responsibility
  - Description: after exact dependency installation, run the repository-owned build and prove the complete emitted runtime is source-consistent: zero missing expected JS outputs and zero stale JS outputs for the exact accepted TypeScript source frontier, including `dist/core/handoffEndpointSelection.js` and current `dist/core/workspaceChoice.js` behavior. If the canonical build exposes a new source defect, stop and return only that exact blocker.
  - Controlling Artifact: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Boundary: emitted-runtime correction only; no accepted semantic redesign.

- run-deterministic-vscode-and-local-core-gates
  - Transfer Kind: work-and-responsibility
  - Description: require `node test/run.mjs` to pass all 117 bridge cases and `node test/package-integration.mjs` to pass all 4 package scenarios. Also run the repository's disposable exact-local-Core harness (`npm run test:local-core -- --core <exact-carried-core-workspace>`) so the extension is validated against the exact carried Core frontier without durable manifest/lockfile mutation. Preserve the exact command outputs and version receipts needed for Anchor reconciliation.
  - Controlling Artifact: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Boundary: deterministic Node/package/build acceptance only; do not claim Sigma or real Extension Host acceptance.

- return-exact-technical-result-to-anchor
  - Transfer Kind: responsibility
  - Description: return one qualified Kodax-to-Anchor Handoff carrying the exact corrected VS Code Workspace if canonical build output changes durable `dist`, the unchanged exact Core Workspace, and deterministic receipts for dependency versions, build/parity, 117/117, 4/4, and exact-local-Core validation. If any gate fails, return the first exact bounded blocker with the durable frontiers preserved.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: no remote commit, push, release, publication, deployment, or registry mutation.

## Required Context

- anchor-reconciliation
  - Material: exact Anchor Evidence proving the Kodax roundtrip preserved the accepted Core and VS Code frontiers byte-for-byte and that only the capable build environment remains unresolved.
  - Material Reference: [Anchor Exact-Frontier Build Gate Reconciliation](business::.topics/initiatives/012-tooling-major-008-anchor-exact-frontier-build-gate-reconciliatio.trace.md)
  - Purpose: exact transfer baseline and no-semantic-broadening boundary.
  - Availability: available

- prior-environment-blocker
  - Material: exact Kodax evidence for the sandbox npm/DNS blocker and prohibited substitute compiler boundary.
  - Material Reference: [Kodax Canonical Build Environment Blocker Evidence](business::.topics/initiatives/011-tooling-major-008-kodax-canonical-build-environment-blocker-evid.trace.md)
  - Purpose: distinguish environment logistics from product/source defects.
  - Availability: available

- canonical-runtime-task
  - Material: exact emitted-runtime parity Task and its zero-missing/zero-stale, 117/117, and 4/4 done criteria.
  - Material Reference: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Purpose: deterministic technical acceptance contract.
  - Availability: available

- accepted-core
  - Material: exact accepted Core Workspace carried by this package.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: shared semantic/package authority and exact-local-Core validation source.
  - Availability: available

- accepted-vscode
  - Material: exact accepted VS Code Workspace carried by this package.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: canonical build source/runtime frontier.
  - Availability: available

## Reference Context

- shared-headless-package-proof
  - Material: accepted Anchor evidence that Core/Tooling independently manufactures, reads, orients, and grounds the Package V1 semantics that VS Code consumes, including bounded cache and participant/endpoint pointer lineage.
  - Material Reference: [Anchor Headless Package V1 Acceptance Evidence](business::.topics/initiatives/010-tooling-major-008-anchor-headless-package-v1-acceptance-evidence.trace.md)
  - Purpose: preserve machine-proven shared semantics while completing host runtime parity.
  - Availability: available

- current-kodax-return
  - Material: exact preceding Kodax-to-Anchor environment blocker return.
  - Material Reference: [Kodax Canonical Build Environment Blocker Return](business::.topics/initiatives/handoffs/039-kodax-to-anchor-tooling-major-008-canonical-build-environment-bl.trace.md)
  - Purpose: preserve exact return continuity and blocker disposition.
  - Availability: available

## Retained Responsibilities

- anchor-final-fan-in
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: recipient-ground the Kodax return, compare exact source/runtime delta, replay shared Tooling/package acceptance, and manufacture the subsequent Sigma carrier only after deterministic gates are green.
  - Boundary: Kodax technical PASS does not self-promote to Major 008 closure or Sigma acceptance.

- sigma-real-host-acceptance
  - Retained By: Sigma
  - Responsibility: after Anchor deterministic reconciliation, perform the actual human VS Code host journey for Role dropdowns, durable references/reload, participant selection, carried/cache behavior, single/multi Pack, ZIP truth, Outgoing truthfulness, and Transport.
  - Boundary: Sigma is not the technical build/debug authority and must not compensate for an unqualified canonical runtime.

## Exclusions And Dependencies

- capable-networked-build-host
  - Kind: unresolved-dependency
  - Description: exact npm lockfile dependencies must be obtainable on the execution host; this is the bounded environment capability missing from the ChatGPT sandbox.
  - Responsible Party Or Role: host provider for execution capability; Kodax for technical interpretation and return Evidence.

- no-substitute-compiler
  - Kind: excluded-scope
  - Description: TypeScript 5.8.3 or any compiler other than the lockfile TypeScript 5.7.2 may not establish canonical runtime parity.
  - Responsible Party Or Role: Kodax and host operator.

- no-semantic-broadening
  - Kind: excluded-scope
  - Description: do not change Core Handoff/Role/participant/cache/Package V1/pointer semantics or introduce VS Code-private semantic authority to make the build pass.
  - Responsible Party Or Role: explicit future qualified authority only.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, release, publication, deployment, registry write, or other remote mutation is authorized.
  - Responsible Party Or Role: separate explicit authority only.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return one qualified Kodax-to-Anchor Handoff after exact lockfile dependency acquisition, repository-owned TypeScript 5.7.2 build, zero missing/stale emitted outputs, 117/117 bridge, 4/4 package integration, and exact-local-Core validation are all green; otherwise return the first exact bounded blocker without semantic broadening.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Sigma testing has begun, Major 008 is closed, a human host operator becomes technical acceptance authority, or remote mutation is authorized.
- Must Not Be Used To Claim: canonical runtime acceptance without exact lockfile versions and deterministic receipts, or Sigma acceptance from Node/package tests.
- Authority Limits: bounded Kodax implementation/build validation under the exact carried Core/VS Code frontiers and controlling parity Task.
- Transport Limits: one canonical Package V1 carrier carrying current Business continuity plus exact accepted Core and VS Code parent snapshots.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [012-tooling-major-008-anchor-exact-frontier-build-gate-reconciliatio.trace.md](../012-tooling-major-008-anchor-exact-frontier-build-gate-reconciliatio.trace.md)
  - Value: lthkAJvz7Qhgdmm7x2e_SFerzJP8qATAk1kprgCWo58

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: lzWqa8FGDwRQ54gm9nnwAX3keMBIn293VqG7NNo_uME