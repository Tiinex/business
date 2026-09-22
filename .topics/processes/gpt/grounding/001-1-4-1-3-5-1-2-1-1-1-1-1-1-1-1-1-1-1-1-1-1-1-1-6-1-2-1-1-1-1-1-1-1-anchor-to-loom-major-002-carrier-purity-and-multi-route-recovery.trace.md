# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 21:56:14
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 21:57:02
  - Authors: Anchor
  - Why: Latest Sigma replay leaves bounded Core-owned carrier and route-projection defects.
  - Summary: Repair clean recipient carrier and shared multi-route projection while preserving the working single-route path.
  - Status: ready/local

---

## Handoff Parties

- Purpose: close the remaining Core-owned carrier-purity and multi-route projection defects exposed by the latest Sigma replay while preserving the successful primary path.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Loom
- To Kind: role
- To Reference: [Loom Role](business::.topics/roles/001-3-1-loom-canonical-holder-cutover-role.trace.md)

## Transfers

- clean-carrier-default
  - Transfer Kind: work-and-responsibility
  - Description: make the normal recipient-facing Handoff carrier omit `tiinex-recipient-v2.transport.json`, using the existing artifact-first clean-carrier mechanics or a stricter equivalent so receiver truth is reconstructed only from visible Tiinex artifacts and exact payload bytes.
  - Boundary: do not post-delete the JSON while runtime logic still relies on it; do not recreate an equivalent hidden semantic authority.

- multi-route-projection
  - Transfer Kind: work-and-responsibility
  - Description: reproduce the exact two-route Sigma carrier and repair shared route/carrier projection so each qualified explicit route yields correct route-specific human/transport output. Preserve fail-closed behavior for genuinely invalid routes and single-route compatibility.
  - Boundary: return host invocation defects to Kodax rather than encoding VS Code policy in Core.

- shared-source-lifecycle-audit
  - Transfer Kind: work
  - Description: audit whether Core source-override/workspace qualification contracts require any change for deterministic stale-source requalification. Implement only shared mechanics proven to belong in Core; otherwise return exact host ownership evidence.
  - Boundary: no silent resealing or semantic repair of stale artifacts.

- loom-return
  - Transfer Kind: responsibility
  - Description: return exact Core delta, focused and broad regression receipts, residual risks and one qualified Loom-to-Anchor Handoff.
  - Boundary: candidate for Anchor fan-in only; no Sigma self-promotion.

## Required Context

- controlling-task
  - Material: exact Post-Sigma Carrier Purity And Transport/Lifecycle Recovery Task.
  - Material Reference: [Recovery Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md)
  - Purpose: controlling objective and Done Criteria.
  - Availability: available

- sigma-evidence
  - Material: exact Anchor-preserved latest Sigma replay Evidence.
  - Material Reference: [Sigma Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-major-002-latest-sigma-carrier-purity-and-lifecycle-evidence.trace.md)
  - Purpose: exact observed failures and product-output package reproduction.
  - Availability: available

- core-workspace
  - Material: exact Core Workspace carried by the latest Sigma product package.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: writable shared implementation source.
  - Availability: available

- vscode-workspace
  - Material: exact VS Code Workspace carried by the latest Sigma product package.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: read-only cross-layer caller/reproduction context.
  - Availability: available

## Reference Context

- latest-product-carrier
  - Material: exact `tiinex-vscode-001-sigma-to-anchor.handoff-package.zip` produced during the latest Sigma replay.
  - Purpose: concrete two-route carrier reproduction and recipient-surface evidence; it is observational product output, not current-work authority.
  - Availability: available

## Retained Responsibilities

- host-controller-recovery
  - Retained By: Kodax
  - Retained By Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)
  - Responsibility: Outgoing discovery, stale host state, duplicate Attach, refresh lifecycle and exact host invocation of Core projections.
  - Boundary: Loom returns host-owned findings rather than patching the extension.

- fan-in-and-sigma
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: reconcile parallel returns and decide the next Sigma gate.
  - Boundary: no specialist-local acceptance promotion.

## Exclusions And Dependencies

- no-docs-change
  - Kind: excluded-scope
  - Description: no canonical schema/semantic change unless an exact contradiction is returned to Anchor/Axiom.
  - Responsible Party Or Role: Loom.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, release, publication or deployment.
  - Responsible Party Or Role: Anchor / release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return the bounded Core repair/evidence and one Loom-to-Anchor Handoff, or stop at the first exact ownership/semantic blocker.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: compatibility JSON is semantic authority, route ambiguity may be guessed, or Core owns VS Code controller lifecycle.
- Must Not Be Used To Claim: local Core tests alone establish Major 002 acceptance.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-major-002-post-sigma-carrier-purity-and-transport-lifecycle-reco.trace.md)
  - Value: w33mim_up_Sdg6cT-JYt_OX_4p4ytCepkj1yPyBeE_0

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: a9ql4R0mXOduo0aPfPuW8aBPsE_loX0t02LmRejgswA