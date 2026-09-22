# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 21:57:02
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-2-anchor-to-kodax-major-002-vs-code-transport-and-lifecycle-recove.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-2-anchor-to-kodax-major-002-vs-code-transport-and-lifecycle-recove.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-2-anchor-to-kodax-major-002-vs-code-transport-and-lifecycle-recove.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 22:46:25
  - Authors: Kodax
  - Why: Return exact Kodax implementation and fail-closed acceptance evidence for Anchor Major 002 fan-in.
  - Summary: Bounded VS Code discovery/lifecycle repair completed; real Extension Host gate remains environment-blocked and shared route projection remains with Loom.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: Did Kodax close the VS Code-owned Major 002 discovery/lifecycle defects without moving shared carrier or route semantics into the host, and what remains blocked before Anchor fan-in?
- Evidence Role: Kodax implementation and acceptance evidence for Anchor reconciliation.
- Supported Conclusion: The bounded VS Code host repair is implemented for explicit operator-root Workspace discovery, stale Outgoing source requalification/invalidation, exact duplicate Attach idempotence, and toast-independent refresh. The carried host already invoked Core transport projection once per exact qualified route, so no host-private multi-route semantic patch was added. The required real VS Code Extension Host gate remains blocked because no VS Code CLI exists in this environment, and the shared multi-route projection defect observed by Sigma remains owned by Loom/Core rather than masked in VS Code.

## Provenance

- Known Source: Tiinex-qualified Anchor-to-Kodax Major 002 route from the received `business-001-2-anchor-to-loom-and-kodax.handoff-package.zip` carrier.
- Preservation Basis: the received carrier SHA-256 was `917fda2e25c31db15dee9293cd4eab0cf3e2adb56ca94762f479d81d85da7d42`; the exact carried VS Code archive SHA-256 was `24764a593b4f1b44863b490fbc77fba1036a11e4f1363e3a7359dbe9f52bc133`; the exact carried Core archive SHA-256 was `d9a9c5349aa30f5e8c0dcf0c31028ced908fdc8e17819291faa401475a52d11e`.
- Mutation Boundary: only the qualified VS Code workspace and Business continuation were mutated. The carried Core workspace remained read-only.
- Provenance Limits: the exact Sigma product-output parent carrier named `tiinex-vscode-001-sigma-to-anchor.handoff-package.zip` is represented by the received carrier lineage and Sigma Evidence but is not separately available as a local file in this execution environment, so no new direct byte-level replay of that historical package is claimed here.

## Evidence Material

- Material: exact modified VS Code source/test workspace, generated JavaScript emitted from the carried source, dependency-free syntax/test receipts, Local Core partial test receipt, real-host blocker receipt, and host/shared ownership findings.
- Material Kind: bounded host implementation plus fail-closed local acceptance evidence.

### Explicit operator-root Workspace discovery

- `src/core/workspaceChoice.ts` now treats one direct canonical `.topics/.workspaces/*.workspace.md` artifact under an explicitly open VS Code root as the representative live source and excludes recursively discovered nested fixture/acceptance Workspaces from that root.
- Legacy root-name matching remains only as a fallback. If several direct canonical Workspace artifacts are equally plausible, the host fails closed instead of surfacing the recursive candidate set.
- `test/run.mjs` adds the Sigma-shaped renamed-checkout/nested-fixture regression and an ambiguity fail-closed case.
- `test/extension-host/suite.cjs` adds a production-controller `workspaceCatalog` gate that writes a nested valid Workspace fixture under the live root and requires the selector to remain exactly one direct canonical source.

### Stale Outgoing source lifecycle

- Outgoing local source identity now carries the exact root plus Workspace target path in its host source key and records a visible `qualified` / `invalid` source-qualification state.
- `refreshOutgoing` requalifies selected local sources before refreshing the tree. A source that no longer resolves to the exact selected Workspace id/root/target becomes visibly invalid and clears the previous built-carrier state.
- Pack repeats the same requalification before payload planning/manufacture and stops early with an explicit invalidated-source message instead of allowing a late `workspace-source-override-unqualified` surprise.
- The real-host suite mutates the exact Workspace artifact to an unqualified body, requires Refresh to mark it invalid, restores the exact bytes, and requires Refresh to recover it as qualified before Pack.

### Exact duplicate Attach and refresh independence

- Attached Handoff host identity now includes Workspace source key, normalized Handoff path, and SHA-256 of the exact qualified Handoff Markdown.
- Re-attaching the same exact Handoff is idempotent: no second semantic route is created and the host records `attach-idempotent-exact` for acceptance evidence.
- If the same path carries different qualified Handoff bytes, normal requalification/update behavior remains available rather than conflating display path with exact identity.
- The no-additional-participants informational toast is now fire-and-forget; Outgoing refresh/update is no longer gated on dismissing that notification.
- The real-host suite exercises duplicate exact Attach and asserts one route plus stable artifact SHA-256.

### Multi-route Transport host seam

- The carried host implementation already reopens immutable carrier bytes, reads Core-qualified orientation routes, and calls `projectPackageTransport(runtime, package, workspaceId:handoffPath)` separately for every exact route.
- It does not use an ambiguous package-wide Handoff projection as a prerequisite for a multi-route package and does not reconstruct recipient or route semantics locally.
- Existing dependency-free regression assertions preserve that exact per-route invocation shape.
- Therefore no new VS Code semantic workaround was introduced for Sigma's shared route-projection failure. If the same exact qualified selector remains blocked in Core, that finding belongs to Loom/Core and must remain visible to Anchor.

### Real-host regression expansion

- `test/extension-host/suite.cjs` now covers explicit operator-root Workspace discovery with a live nested fixture, stale source invalidation/recovery, duplicate exact Attach idempotence, the existing participant exact-set gate, multi-route Pack/Transport and restart requalification.
- The suite drives registered production commands/controllers; acceptance-only commands expose snapshots/catalogs but do not substitute semantic projection.
- The required VS Code CLI is still absent, so this suite could not execute in a true Extension Host here.

### Exact local receipts

- Dependency-free TypeScript parse/transpile over all 53 `src/**/*.ts` files: zero syntax diagnostics.
- `tsc -p tsconfig.json --noEmit`: blocked only at unavailable type definition packages `node` and `vscode` in this source-only environment.
- Emitted-JavaScript `node test/run.mjs` with no installed Core: 56 tests passed before `tiinex.core-package.unavailable` at `@tiinex/core/package.json`.
- Temporary Local Core binding to the exact carried Core workspace plus a temporary package symlink: 67 tests passed before a test that explicitly expects an installed `node_modules/@tiinex/core` root observed the intentionally selected Local Core root `/mnt/data/kodax-core-major2`. This is a harness-mode expectation mismatch and is not treated as product acceptance or failure. All temporary binding/symlink state was removed after the run.
- `node --check test/extension-host/suite.cjs`: passed.
- Canonical `node scripts/test-extension-host.mjs`: stops first at exact blocker `tiinex.extension-host.vscode-cli-unavailable`.

### Exact semantic source delta

- `src/core/workspaceChoice.ts` SHA-256 `c2316baeef3770bf2e27f686d42fbd04958b21dee349b3142edbf2b88988b93b`.
- `src/operatorTrees.ts` SHA-256 `89f771010239b7b697a70cae906e4b055988472cc16c5612c7a74fe94f292d6f`.
- `src/vscode/outgoingParticipantController.ts` SHA-256 `f8549f1e6b3b487d2754148f1269bc2a8c9affdfbac5f5918f071635010ff3cc`.
- `test/extension-host/suite.cjs` SHA-256 `af543db316f45d0fd62178463dcbfdb79b028093300bf3bfd5825375a13a5332`.
- `test/run.mjs` SHA-256 `eb59f913649d3efdc261d942e559e7d971d7308e2f57207a66ecf3a1c8b6fd5d`.
- The blocked TypeScript build emitted `dist/**` from the carried source tree; those generated JavaScript files are carried as build output, but the five files above are the intentional semantic source/test delta for this tranche.

## Preservation And Fidelity

- Preservation State: Core source and the received outer carrier were not modified; fixtures remain present; no fixture was removed or moved to hide discovery leakage; no remote mutation, commit, push, release, publication, or deployment occurred.
- Fidelity Notes: environment limitations are reported as blockers, not product failures and not PASSes. The Local Core partial run is reported only at the strength actually observed.
- Known Losses: no true VS Code Extension Host execution, no dependency-backed clean typecheck, and no direct local copy of the historical Sigma product-output parent carrier for a fresh byte replay.

## Interpretation Limits

- Not Yet Used As: Major 002 acceptance, Sigma acceptance, release approval, publication approval, or proof that Loom's shared carrier/route work is complete.
- Does Not Prove: that shared Core multi-route projection is repaired, that recipient-side carrier purity is repaired, or that the real Extension Host scenarios pass in Local and Published modes.
- Must Not Be Treated As: authority for VS Code to filter or reconstruct a Core route failure into false green, or authority to promote the candidate to Sigma.
- Disposition: bounded Kodax VS Code repair ready for Anchor fan-in; machine acceptance remains blocked at `tiinex.extension-host.vscode-cli-unavailable`, and shared carrier/route findings remain pending Loom reconciliation.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-2-anchor-to-kodax-major-002-vs-code-transport-and-lifecycle-recove.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-2-anchor-to-kodax-major-002-vs-code-transport-and-lifecycle-recove.trace.md)
  - Value: g314MyDyXpKrh0ozvF_GAKR-5RcQepOJmjHPAmlVhGY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: CcYwzCuDiZj58iHwlyz1xitK0sOPBO1aBhyenF42igc