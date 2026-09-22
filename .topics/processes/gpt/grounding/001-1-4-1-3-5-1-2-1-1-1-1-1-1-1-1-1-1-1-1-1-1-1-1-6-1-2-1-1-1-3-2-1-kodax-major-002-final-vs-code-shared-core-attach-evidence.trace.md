# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 11:43:11
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-2-anchor-to-kodax-major-002-final-vs-code-shared-core-completion.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-2-anchor-to-kodax-major-002-final-vs-code-shared-core-completion.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-2-anchor-to-kodax-major-002-final-vs-code-shared-core-completion.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 12:19:55
  - Authors: Kodax
  - Why: Preserve the exact Kodax-owned final host/Core boundary delta, regression receipts, and first unresolved machine blocker for Anchor fan-in.
  - Summary: Bounded Attach discovery now consumes exact Core-projected Handoff lineage; 117/117 bridge and 4/4 package integration pass, while real-host execution remains blocked by missing VS Code CLI.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: Does the final bounded Kodax VS Code repair remove the remaining host-private Handoff discovery/leaf authority from Attach, keep exact open-Workspace provenance and shared-Core qualification, and preserve the existing single/multi package path without introducing a second semantic engine?
- Evidence Role: Kodax implementation and regression evidence for Anchor fan-in under Major 002.
- Supported Conclusion: Yes at the repository/shared-Core boundary. Attach Handoff browse now consumes shared Core `project-handoff-leaves` for the explicitly selected qualified Workspace root, host-side scoping rejects nested fixture/repository paths outside `.topics/`, Core qualification remains authoritative for exact Attach identity, and Pack/Transport paths are unchanged. The repository-owned bridge suite passes 117/117 and package integration passes 4/4 in a disposable offline installed-binding harness using the exact carried Core code. The real VS Code Extension Host machine gate remains blocked before execution because no VS Code-family CLI exists in this environment.

## Provenance

- Known Source: Tiinex-qualified Anchor-to-Kodax route selected by `001-3-1-1-1-handoff-pointer.trace.md` from the current carrier.
- Preservation Basis: the exact carried VS Code Workspace archive was verified before materialization at SHA-256 `0fc0e2513e8a3f13783c1fcb6bc30859dc0abb25d8f8ff31e504c1506b21fddf`; the exact carried Core Workspace archive was verified at SHA-256 `27f4e50712f4f091b18ff42751cf31a06907a4f71672797364e82e092ad2c471`.
- Mutation Boundary: only the qualified VS Code Workspace and Business continuation were mutated. Core remained read-only and the received outer carrier remained untouched.
- Provenance Limits: the full Node regression run used a disposable copy of the exact carried Core package under `node_modules/@tiinex/core`, changing only that disposable package copy's `version` metadata to the extension lock value `0.35.0` so the existing installed-binding branch could execute offline. That is a harness receipt, not Published Core acceptance.

## Evidence Material

- Material: exact VS Code source/build delta, Core-projected Attach authority change, dependency-free source-scoping regression, 117/117 bridge receipt, 4/4 package-integration receipt, TypeScript/build environment receipt, real Extension Host machine-gate receipt, and byte-preservation receipts.
- Material Kind: bounded host/controller implementation plus repository-owned regression evidence.

### Durable host correction

- Added `src/core/handoffRouteSelection.ts` as a pure host-side source-scoping helper. It accepts only Core-qualified exact Handoff candidates for the explicitly selected Workspace, normalizes relative paths, rejects traversal/absolute paths, rejects candidates outside `.topics/`, preserves Core-projected leaf state, deduplicates by exact Handoff path, and adds no Handoff semantics of its own.
- `src/packageBuilder.ts` now routes exact Handoff candidates through that helper, checks Core findings, preserves Core leaf state in the presentation model, and exposes `loadHandoffRouteChoicesForSource`. That loader first verifies the selected root projects exactly one requested Workspace id, then delegates Handoff lineage/qualification to shared Core `project-handoff-leaves`.
- `src/operatorTrees.ts::attachHandoffFromWorkspace` no longer calls `indexLocalWorkspace` plus `leafArtifactPathSet` to create the live Attach candidate surface. It requests Core-projected Handoff choices for the exact selected Outgoing Workspace root, presents either Core leaves or full Core-qualified lineage, and still calls `qualifyExistingHandoff` for the exact selected identity before Attach.
- Existing duplicate Attach, participant projection, stale Outgoing requalification, one shared Core manufacture path for single/multi Pack, and per-route Core Transport projection were not replaced or weakened.
- `test/run.mjs` adds a dependency-free route-scoping regression proving that same exact source projection rejects nested fixture paths and degraded candidates while preserving exact Core leaf identity. Stale source-string assertions were updated to require the Core-projected Attach path instead of the removed host-private browse path.

### Exact durable delta

- Original `src/**/*.ts` tree fingerprint: `0b9fb9932f7184509cee6ac5608dbbbf8875a6d9b74cfde39d155b4f4a299bfc` across 53 files.
- Final `src/**/*.ts` tree fingerprint: `ad6f74cbca615a1caa66db902d4ff16d7ea5e15cd4524c02a424befc69aaba7c` across 54 files.
- Added source: `src/core/handoffRouteSelection.ts` SHA-256 `69d3101889cd7c8300daae864b5840640400fc6bc708b29af6735a514c43fb7e`.
- Changed source: `src/packageBuilder.ts` from `1687017dba8ea8e445e6f8382a1be71191b941450d4f8845b83b6dd88e9a737d` to `69fc5e9b3cc7484cde4933a59a8951f25abbcf8ca3269935141f83bb44de1470`.
- Changed source: `src/operatorTrees.ts` from `89f771010239b7b697a70cae906e4b055988472cc16c5612c7a74fe94f292d6f` to `8407579b748e10f001a02f17d49043f95aae18fcfa2470138992ee789396e208`.
- Changed regression: `test/run.mjs` from `1a8fe9f5f2224ef9426a8d8e28136a56444c92d0fc9c83ccfd5281f4da5e5762` to `7896d45c18499a73519026e4e365353e37c2ced6899b3ed9fe68cf962a0b92ab`.
- Corresponding emitted runtime deltas are limited to `dist/packageBuilder.js(.map)`, `dist/operatorTrees.js(.map)`, and new `dist/core/handoffRouteSelection.js(.map)`.
- Full comparison against the qualified received VS Code snapshot reports 3 added files, 7 changed files, and 0 removed files; all additions beyond source are corresponding ignored `dist` build output.
- No durable `node_modules` or `.vscode/link/dependency-mode.json` exists in the returned VS Code Workspace.

### Execution receipts

- Disposable offline installed-binding run: `node test/run.mjs` completed `117/117 Tiinex VS Code bridge core cases passed`.
- Disposable offline installed-binding run: `node test/package-integration.mjs` completed `4/4 package integration scenarios passed. Windows/VS Code UI acceptance remains separate.`
- The package-integration scenarios cover real package-builder output, exact re-orientation without invented Handoff/lineage, byte-identical idempotent retry versus divergent overwrite rejection, and extracted VSIX execution of its bundled public Core entrypoint.
- Global TypeScript 5.8.3 with `--noEmitOnError false` emits the modified runtime files. The compiler exit remains 2 solely because this sandbox lacks the configured type libraries `node` and `vscode`; the emitted modified JavaScript files each pass `node --check` and are the files used by the green 117/117 disposable regression run.
- Canonical real-host attempt: `node scripts/test-extension-host.mjs --mode both --local-core <exact-carried-core>` exits before build/host execution with exact blocker `tiinex.extension-host.vscode-cli-unavailable` because none of `code`, `code-insiders`, or `codium` is available.

## Preservation And Fidelity

- Preservation State: exact carried Core source is unchanged; the VS Code correction is bounded to Attach/Core projection plus its regression and corresponding emitted runtime; received package bytes are untouched; no fixture deletion/movement, no remote mutation, no commit/push/publication/release/deployment, and no Sigma promotion occurred.
- Fidelity Notes: the host still owns only explicit Workspace-root selection and presentation. Core owns Workspace projection, Handoff qualification/lineage, participants, package manufacture, route projection and transport semantics.
- Known Losses: the machine lacks a real VS Code CLI, so the repository-owned real Extension Host gate could not execute under either Local or Published mode. The sandbox also lacks local `@types/node` and `@types/vscode`, so ordinary typecheck cannot complete here.

## Interpretation Limits

- Not Yet Used As: Sigma acceptance, real VS Code Extension Host acceptance, Published Core acceptance, release approval, or deployment authorization.
- Does Not Prove: that a machine with VS Code installed will pass the real-host suite; that downstream registry/published dependency state is correct; or that unrelated product areas are defect-free.
- Must Not Be Treated As: authority to recreate Core semantics in VS Code, broaden the repair beyond shared-Core Attach provenance, hide discovery defects by moving fixtures, or self-promote the candidate to Sigma.
- Disposition: repository/shared-Core boundary repair complete; downstream machine disposition remains blocked at first exact unresolved gate `tiinex.extension-host.vscode-cli-unavailable` and is returned to Anchor for fan-in/next-capable-machine sequencing.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-2-anchor-to-kodax-major-002-final-vs-code-shared-core-completion.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-2-anchor-to-kodax-major-002-final-vs-code-shared-core-completion.trace.md)
  - Value: N_2yiXqIGB_GEdWflZjAm2bwKeI4w8JmdHOHysT_7Tw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: cuBHimopXvey5JHYi1CVMMqG64rMBi_hIFT3Tcub494