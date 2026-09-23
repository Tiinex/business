# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-23 13:02:51
  - Trace: [010-tooling-major-008-anchor-headless-package-v1-acceptance-evidence.trace.md](../010-tooling-major-008-anchor-headless-package-v1-acceptance-evidence.trace.md)
  - Origin:
    - [relative](../010-tooling-major-008-anchor-headless-package-v1-acceptance-evidence.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-23 13:03:57
  - Authors: Anchor
  - Why: Shared Tooling now passes a real headless package roundtrip; the next bounded layer is VS Code as a thin consumer, not a second semantic implementation.
  - Summary: Consume the proven shared Package V1 semantics in VS Code, restore exact-lockfile emitted-runtime parity, and return deterministic evidence before Sigma.
  - Status: ready/local

---

## Handoff Parties

- Purpose: move Tooling Major 008 from the now-proven headless shared Package V1 semantics into the VS Code thin-consumer layer, restore canonical repository-owned emitted-runtime parity, and return deterministic machine evidence to Anchor before Sigma real-host testing.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- consume-proven-shared-tooling-as-thin-vscode-host
  - Transfer Kind: work-and-responsibility
  - Description: align the VS Code host with the already-proven shared Core/Tooling operations for qualified Role endpoint discovery, durable From/To References, explicit 0..N participants, carried/bounded-cache material resolution, truthful package projection, numeric participant -> From -> To -> Handoff pointer lineage, and single/multi Package V1 manufacture. VS Code must project and invoke shared semantics rather than reimplement them.
  - Controlling Artifact: [Anchor Headless Package V1 Acceptance Evidence](business::.topics/initiatives/010-tooling-major-008-anchor-headless-package-v1-acceptance-evidence.trace.md)
  - Boundary: no second recipient representation, sibling pointer grouping, VS Code-private Role/package truth, cache identity layer, or semantic duplication.

- restore-canonical-vscode-emitted-runtime-parity
  - Transfer Kind: work-and-responsibility
  - Description: use the exact repository lockfile toolchain, including TypeScript 5.7.2 and pinned type dependencies, to run the repository-owned build from the accepted VS Code source frontier; require zero missing and zero stale emitted JS, then run the full 117/117 bridge and 4/4 package integration suites against the exact accepted Core frontier.
  - Controlling Artifact: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Boundary: do not hand-author dist, substitute a host compiler as product authority, weaken lockfile versions, or change shared Core/package semantics to satisfy the host.

- return-deterministic-kodax-evidence-to-anchor
  - Transfer Kind: responsibility
  - Description: return one qualified Kodax-to-Anchor Handoff carrying the exact VS Code source/runtime delta and deterministic acceptance receipts; if any gate cannot be satisfied, return only the next exact bounded blocker without semantic broadening.
  - Controlling Artifact: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Boundary: Sigma real-host testing is downstream of Anchor replay and is not part of this transfer.

## Required Context

- headless-package-proof
  - Material: Anchor Evidence that shared Core/Tooling independently manufactured, inspected, bootstrapped, oriented, and cold-grounded a real Package V1 carrier with bounded external Role cache and numeric participant/endpoint/Handoff pointer lineage.
  - Material Reference: [Anchor Headless Package V1 Acceptance Evidence](business::.topics/initiatives/010-tooling-major-008-anchor-headless-package-v1-acceptance-evidence.trace.md)
  - Purpose: prove the semantics VS Code must consume already work without VS Code.
  - Availability: available

- controlling-major
  - Material: complete Tooling Major 008 acceptance contract and MUST/MUST NOT invariants.
  - Material Reference: [Tooling Major 008](business::.topics/initiatives/001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
  - Purpose: sole product/closure authority.
  - Availability: available

- canonical-runtime-task
  - Material: exact canonical emitted-runtime parity Task, including repository-owned build, zero missing/stale outputs, 117/117 bridge, and 4/4 package integration criteria.
  - Material Reference: [VS Code Emitted Runtime Parity Correction](business::.topics/initiatives/005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md)
  - Purpose: bounded build/runtime acceptance gate.
  - Availability: available

- anchor-continuation
  - Material: current Anchor Major 008 continuation preserving accepted Loom Core, pre-Sigma ordering, and machine-first acceptance boundary.
  - Material Reference: [Anchor Continuation](business::.topics/initiatives/handoffs/037-anchor-to-anchor-tooling-major-008-canonical-runtime-and-sigma-continuation.trace.md)
  - Purpose: exact controlling continuation state.
  - Availability: available

- accepted-core
  - Material: exact accepted Core Workspace carried by this package.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: shared semantic/package authority and integration-test dependency.
  - Availability: available

- accepted-vscode
  - Material: exact current VS Code Workspace carried by this package.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: thin-host implementation and canonical build source frontier.
  - Availability: available

## Reference Context

- prior-kodax-parity-route
  - Material: earlier Anchor-to-Kodax emitted-runtime resume Handoff retained only as historical context for the parity gate; it is not the current route because later Major 008 descendants superseded its lineage position.
  - Material Reference: [Prior Anchor To Kodax Resume](business::.topics/initiatives/handoffs/032-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-resume.trace.md)
  - Purpose: preserve the earlier bounded build-contract context without reusing its obsolete route position.
  - Availability: available

## Retained Responsibilities

- anchor-final-deterministic-replay
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: after Kodax return, independently replay canonical emitted-runtime parity and shared Tooling/package acceptance before manufacturing any Sigma carrier.
  - Boundary: Kodax receipts do not replace Anchor fan-in acceptance.

- sigma-real-host-acceptance
  - Retained By: Sigma
  - Responsibility: after deterministic gates, verify actual VS Code Role dropdowns, durable save/reload/re-attach, participant multi-select, carried/cache behavior, single/multi Pack, ZIP truth, Outgoing truthfulness, and Transport.
  - Boundary: Sigma must not be the first observer of shared-Core/package or canonical-build defects.

## Exclusions And Dependencies

- no-core-or-package-redesign
  - Kind: excluded-scope
  - Description: do not modify Core Package V1 representation, pointer lineage rules, Role/participant semantics, bounded cache semantics, recipient representation, or transport semantics unless an exact new shared-Core blocker is proven and returned to Anchor.

- no-host-private-semantic-authority
  - Kind: excluded-scope
  - Description: do not create VS Code-private Role discovery, endpoint/participant truth, package semantics, cache identity, or hidden mutable authority needed to make the flow work.

- exact-build-dependencies
  - Kind: unresolved-dependency
  - Description: canonical build requires the exact repository-lock TypeScript 5.7.2 and pinned type dependencies. Acquire them only as ordinary build dependencies if the execution environment permits; do not claim parity using substitutes.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, release, publication, deployment, registry mutation, or other remote write is authorized by this Handoff.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return one qualified Kodax-to-Anchor Handoff only after the VS Code host consumes the shared Tooling semantics without duplication, the exact repository-owned build produces zero missing/stale emitted outputs, and 117/117 bridge plus 4/4 package integration gates are green; otherwise return the next exact bounded blocker.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Major 008 is closed, Sigma testing has started, VS Code may redefine shared semantics, or canonical runtime parity is already accepted.
- Must Not Be Used To Claim: host implementation convenience overrides shared Core/Tooling authority or that passing UI behavior can substitute for canonical build/package acceptance.
- Authority Limits: bounded VS Code thin-consumer implementation, canonical emitted-runtime parity, and deterministic return evidence only.
- Transport Limits: one canonical Package V1 carrier using the exact current Business lineage and accepted Core/VS Code snapshots.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [010-tooling-major-008-anchor-headless-package-v1-acceptance-evidence.trace.md](../010-tooling-major-008-anchor-headless-package-v1-acceptance-evidence.trace.md)
  - Value: PvDIdxah1-5ahhx293K2P-vrOUx5wVadHEf7X-FfsrA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: B2EU3tjvSbspOb35xFyyRyO_v0mRHQRQo1HdEpJbZo0