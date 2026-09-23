# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 19:41:50
  - Trace: [029-kodax-to-anchor-tooling-major-008-final-vs-code-shared-core-conv.trace.md](handoffs/029-kodax-to-anchor-tooling-major-008-final-vs-code-shared-core-conv.trace.md)
  - Origin:
    - [relative](handoffs/029-kodax-to-anchor-tooling-major-008-final-vs-code-shared-core-conv.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 19:53:47
  - Authors: Anchor
  - Why: Preserve exact fan-in evidence and prevent a build-artifact mismatch from being misclassified as another Core or Package V1 design problem.
  - Summary: Anchor isolates the final pre-Sigma blocker to exactly two VS Code emitted-runtime parity defects; source logic passes integrated deterministic acceptance once runtime matches source.
  - Status: ready/local

---

# Tooling Major 008 — Anchor Emitted Runtime Parity Blocker Evidence

## Supported Claim Or Question

- Supported Claim Or Question: Is the returned Major 008 VS Code candidate ready for real-host acceptance as carried, or does its durable emitted runtime differ from the exact accepted source frontier?
- Evidence Role: Anchor integrated fan-in evidence isolating one bounded VS Code build-artifact consistency blocker after the Kodax shared-Core convergence return.

## Provenance

- Known Source: exact qualified `business-001-1-1-1-1-kodax-to-anchor.handoff-package.zip`, compared against exact parent `business-001-1-1-1-anchor-to-kodax.handoff-package.zip` with carried Tiinex Tooling.
- Preservation Basis: exact returned Business/Core/VS Code Workspace bytes materialized only through the qualified Handoff Workspace byte provider after cold orientation and grounding.
- Source Delta Basis: Core is byte-identical to the accepted parent; VS Code changes 17 paths and adds/removes none; Business adds only Kodax Evidence/return artifacts.
- Runtime Audit Basis: disposable compile/transpile output from the exact returned `src/**/*.ts` frontier was compared path-for-path against the carried `dist/**/*.js` runtime surface. Disposable output is diagnostic evidence only and is not promoted as product source.
- Provenance Limits: no real VS Code Extension Host is available in Anchor's machine; real-host acceptance remains separate.

## Evidence Material

- Material Kind: exact source-frontier comparison, source/emitted-runtime parity audit, and disposable integrated execution receipts.
- Material: returned VS Code source/dist bytes, unchanged accepted Core bytes, Node/package integration receipts, and focused Core Major 008 receipts.

### Exact durable source delta

- Core relative to the resumed Anchor-to-Kodax parent: byte-exact, 0 changed paths.
- VS Code relative to the resumed parent: 17 byte-changed paths, 0 additions, 0 removals.
- Business relative to the resumed parent: exactly two added Kodax artifacts (implementation Evidence and return Handoff), 0 byte-changed or removed paths.

### Emitted runtime parity blocker

The durable returned VS Code snapshot is not build-consistent with its exact source frontier in exactly two runtime locations:

1. `src/core/handoffEndpointSelection.ts` is present and is imported by current `src/packageBuilder.ts`; current carried `dist/packageBuilder.js` requires `./core/handoffEndpointSelection`, but `dist/core/handoffEndpointSelection.js` is absent.
2. `src/core/workspaceChoice.ts` contains the accepted direct-canonical-Workspace representative filter that excludes nested fixture/test Workspaces, but carried `dist/core/workspaceChoice.js` is stale and still returns all recursively discovered candidates when root-name matching does not disambiguate.

A full exact-source emitted-JS audit produced 54 expected JS outputs:
- 52 carried `dist` files match their exact source-derived output after source-map comment normalization.
- 1 output is missing: `dist/core/handoffEndpointSelection.js`.
- 1 output is stale: `dist/core/workspaceChoice.js`.
- No other JS parity differences were found.

This is a durable runtime/package consistency blocker, not authority to change Core semantics, Package V1, Role discovery rules, or the accepted Major 008 source implementation.

### Anchor disposable integration probe

Anchor generated source-consistent runtime output only inside a disposable harness, preserving the carried candidate unchanged.

Against exact accepted Core source (probe-only installed package metadata adjusted to the extension lock value solely to exercise the existing offline installed-binding branch):

- `node test/run.mjs`: `117/117 Tiinex VS Code bridge core cases passed`.
- `node test/package-integration.mjs`: `4/4 package integration scenarios passed`.
- Core `test/handoff-major-008-core.test.mjs`: `3/3` pass.
- Core focused `Major 008 explicit participant selection` tests: `2/2` pass, including direct carried-Workspace resolution and discovery-only bounded cache material.

Before disposable emitted-runtime regeneration:
- `node test/run.mjs` first fails because `dist/core/handoffEndpointSelection.js` is absent.
- After supplying only that missing output, the next failure exposes stale `dist/core/workspaceChoice.js` by returning `vscode`, `001-3-acceptance`, and `extension-host-acceptance` where only `vscode` is valid.
- Regenerating source-consistent runtime output removes both blockers and the complete deterministic suite passes.

## Preservation And Fidelity

- Preservation State: returned Business/Core/VS Code Workspace bytes remain unchanged; all runtime regeneration occurred in disposable Anchor harnesses only.
- Fidelity Notes: the probe demonstrates that the accepted source logic is internally consistent once emitted runtime matches source. It does not authorize Anchor to mutate Kodax-owned durable VS Code output.
- Known Losses: dependency-backed TypeScript typecheck and true Local + Published VS Code Extension Host execution remain unavailable in this environment.

## Interpretation Limits

- Does Not Prove: real VS Code Extension Host acceptance, Sigma UX acceptance, registry Published-Core acceptance, or final Major 008 completion.
- Must Not Be Treated As: authority to redesign Package V1, reopen Core authoring/material semantics, alter Workspace discovery semantics, or add new host-private logic.
- Not Yet Used As: Sigma promotion.
- The correct next action is a bounded Kodax emitted-runtime parity correction for the exact accepted source frontier, followed by Anchor re-run of the deterministic integration and then the real-host gate.

## Review Notes

The source implementation itself is accepted provisionally by Anchor's deterministic probe. The only known pre-Sigma blocker is durable emitted runtime parity for the two identified Core-host outputs. Kodax should regenerate/land matching emitted runtime from the exact accepted source without semantic source changes unless its canonical repository build exposes a new exact source defect.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [029-kodax-to-anchor-tooling-major-008-final-vs-code-shared-core-conv.trace.md](handoffs/029-kodax-to-anchor-tooling-major-008-final-vs-code-shared-core-conv.trace.md)
  - Value: jBtqm-TnTmT-cdiZ1pQdkckMai_UDtX0WE-Is1zUun8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: evXhAOARyujwxq1x2x5rIoFxpFtz9maueE54vP6HSDA