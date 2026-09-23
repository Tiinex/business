# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 19:55:09
  - Trace: [030-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-correct.trace.md](handoffs/030-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-correct.trace.md)
  - Origin:
    - [relative](handoffs/030-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-correct.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 20:07:53
  - Authors: Kodax
  - Why: Preserve the exact bounded blocker and byte-preservation receipt without widening the parity-only Kodax tranche.
  - Summary: Canonical build parity correction is blocked by a new exact VS Code-local TypeScript contract mismatch; VS Code and Core bytes remain unchanged.
  - Status: ready/local

---

# Tooling Major 008 — Kodax Emitted Runtime Canonical Build Blocker Evidence

## Supported Claim Or Question

- Supported Claim Or Question: Can the exact accepted VS Code source frontier be canonically rebuilt into a durable emitted runtime without changing semantic source, or does the repository build surface a new exact blocker outside the bounded parity-only correction?
- Evidence Role: exact Kodax build/output-parity blocker evidence for the Anchor-requested emitted-runtime correction, preserving the accepted VS Code/Core bytes when the build frontier exposes a new source-contract defect.

## Provenance

- Known Source: exact qualified `business`, `core`, and `vscode` Workspace snapshots carried by the selected Anchor-to-Kodax Handoff package after Start-only cold read, verified portable Tooling bootstrap, Tiinex orientation, exact route grounding, and qualified Workspace materialization.
- VS Code Archive Identity: carried `001-5-vscode.workspace.zip`, SHA-256 `883ed4a0bfede2b86efa09c077ac96727ab43410da3f4f4f70447ada7b26e04b`.
- Core Archive Identity: carried `001-4-core.workspace.zip`, SHA-256 `50a8f620aa0f2cf657370d95302c53db97126009a373a3a4c69a5ecb1673d15e`.
- Preservation Basis: the received VS Code Workspace was copied byte-for-byte before build execution; all temporary build-environment material was removed and the durable VS Code tree was verified identical to that pre-build snapshot after rollback. Core was never mutated.
- Provenance Limits: the exact lockfile TypeScript 5.7.2 and `@types/vscode` 1.95.0 packages are not locally available and registry acquisition is unavailable in this execution environment.

## Evidence Material

- Material Kind: repository-owned canonical build attempt, focused host-only type diagnostic, exact source/type contract inspection, and byte-preservation audit.
- Material: `npm run build` receipt, exact local `HandoffLeavesResult` declaration, exact `packageBuilder.ts` property access, and full before/after Workspace byte comparison.

### Canonical repository build attempt

- Repository build command: `npm run build` from the exact carried VS Code root.
- Repository build path: `npm run clean && tsc -p tsconfig.json`.
- Result: exit code `2` before emitted runtime generation because the host lacks the configured type libraries `node` and `vscode`.
- Exact diagnostics: `TS2688 Cannot find type definition file for 'node'` and `TS2688 Cannot find type definition file for 'vscode'`.
- The build clean step ran first, so the original `dist` tree was restored exactly from the byte-preserved pre-build snapshot before any return material was authored.

### New exact source-contract blocker

A host-only diagnostic compile was used only to continue structural checking after the missing external type-library gate. It did not mutate durable source and is not claimed as canonical type acceptance.

The diagnostic exposed an exact local TypeScript contract mismatch independent of VS Code API typing:

- `src/tiinex/bootstrap.ts` declares `HandoffLeavesResult` with `status`, optional `candidates`, `leaves`, and `pointerless`; it does not declare a `findings` property.
- `src/packageBuilder.ts` reads `projected.findings` twice in `handoffRouteChoicesForSources` when handling the result of `projectHandoffLeaves`.
- TypeScript reports `TS2339: Property 'findings' does not exist on type 'HandoffLeavesResult'` at those accesses.
- This mismatch is internal to the exact accepted VS Code source frontier and does not depend on the missing VS Code external type definitions.

The controlling correction Task explicitly says that if canonical rebuild exposes a new exact source defect that cannot be corrected as emitted-output parity, Kodax must stop and return the blocker instead of broadening source semantics. No source edit was made.

### Preservation receipt

After removing all temporary build material and restoring `dist` from the pre-build snapshot:

- VS Code before/current file count: `391` / `391`.
- Added paths: none.
- Removed paths: none.
- Byte-changed paths: none.
- Durable `node_modules`: absent.
- Core source: unchanged; Core manifest receipt SHA-256 `8f420d03271b7d112f44fc982b084972d8e3a39385d76b42c55db0633e6830ff` over the materialized exact tree.
- The known original parity defects therefore remain intentionally unresolved in the returned VS Code snapshot: missing `dist/core/handoffEndpointSelection.js` and stale `dist/core/workspaceChoice.js`.

## Preservation And Fidelity

- Preservation State: exact accepted VS Code and Core Workspaces are returned unchanged because the bounded parity-only tranche was stopped before any durable output mutation.
- Fidelity Notes: the host-only type diagnostic used temporary local type material solely to expose source-structural diagnostics after the canonical build was blocked on unavailable external typings. It is not a substitute for the exact locked toolchain or for real Extension Host execution.
- Known Losses: no durable emitted-runtime correction was produced; deterministic 117/117 and 4/4 regressions were not rerun against a modified runtime because no modified runtime was allowed to survive the newly exposed source blocker.

## Interpretation Limits

- Does Not Prove: that the accepted VS Code source semantics are wrong at runtime, that Core must change, that Package V1 must change, or that real-host/Sigma acceptance failed.
- Must Not Be Treated As: permission to widen this emitted-output correction into a semantic source refactor, to edit Core, or to manufacture parity files by hand around the source type mismatch.
- Not Yet Used As: emitted-runtime parity acceptance, real Extension Host acceptance, or Sigma promotion.

## Review Notes

Anchor should reconcile the exact internal `HandoffLeavesResult` / `projected.findings` source-contract mismatch and decide the next bounded source-authority step. Once that exact source blocker is resolved under appropriate authority, rerun the repository-owned canonical build, full source/dist parity audit, 117/117 bridge suite, 4/4 package integration, and only then continue to the real-host gate.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [030-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-correct.trace.md](handoffs/030-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-correct.trace.md)
  - Value: 9Srle8q2Xm9EFa-r9a590aWCOBbjVCqqN5PjIrFDDVE

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Xb0mpOfj1U2z7Ph9GrYLoQ22CdV2DPem1cpoauvNuAA