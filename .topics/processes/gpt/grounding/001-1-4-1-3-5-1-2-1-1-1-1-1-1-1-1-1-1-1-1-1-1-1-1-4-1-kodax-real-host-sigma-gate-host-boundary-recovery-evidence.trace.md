# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 18:38:24
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-4-anchor-to-kodax-real-host-sigma-gate-host-boundary-recovery-package-correction.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-4-anchor-to-kodax-real-host-sigma-gate-host-boundary-recovery-package-correction.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-4-anchor-to-kodax-real-host-sigma-gate-host-boundary-recovery-package-correction.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 19:18:40
  - Authors: Kodax
  - Why: Anchor requires exact Kodax host delta, ownership findings, regression receipts, and fail-closed acceptance status before parallel reconciliation.
  - Summary: Repair live endpoint authority leakage in Extension VS Code, preserve exact same-label choices, trace Workspace ownership, and return the real-host machine blocker.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: Did the bounded Kodax recovery remove the VS Code host authority leak exposed by Sigma, preserve exact same-label endpoint candidates, avoid host-side Workspace byte repair, and complete the required real-host acceptance?
- Evidence Role: Kodax implementation, ownership-trace, and machine-gate evidence for Anchor reconciliation.
- Supported Conclusion: the VS Code host defect was reproduced and repaired at the host-owned source/presentation boundary. Live endpoint authoring no longer aggregates repository-wide artifacts or collapses candidates by human Role label; exact endpoint candidates are projected independently from the explicitly selected Outgoing Workspace root and same-label candidates remain distinct. The carried top-level Workspace artifacts qualify under the accepted Core before host mutation, so no host resealing/normalization repair was justified. Repository-owned regression coverage was strengthened around the real production controller path, but the required real VS Code Extension Host run remains blocked at `tiinex.extension-host.vscode-cli-unavailable`; therefore this return is blocked and not Sigma-ready.

## Provenance

- Known Source: Tiinex-qualified Business, Extension VS Code, and accepted Core workspaces carried by the selected Anchor-to-Kodax real-host Sigma gate host-boundary recovery Handoff.
- Preservation Basis: the received package SHA-256 is `9a96ca1a644bff873d43a9078b0cc26b26cd37bd7515cb65aec890aeae0fa669`; the carried Extension VS Code baseline archive SHA-256 is `dd4f59d8ae121d75d3f4f88064c69ecb5edc292b3afbd82c58d724c6f18b2490`; the accepted Core archive SHA-256 is `2ff12a1af5b9254604f8ccedd5c742f9db84ef9c75ed5f47bbd8f4c856a1b8c7`. Both nested workspace archives were verified against carrier bindings before materialization.
- Mutation Boundary: only the qualified Extension VS Code workspace and the Business continuation were mutated. The accepted Core remained read-only. No remote repository, release, publication, deployment, or canonical Docs source was mutated.
- Provenance Limits: this environment has no compatible VS Code-family CLI/Extension Host runtime and cannot restore the missing npm dependency tree from the network; real-host acceptance therefore cannot be claimed here.

## Evidence Material

- Material: exact modified Extension VS Code Workspace, exact current accepted Core Workspace, source-delta hashes, deterministic source/test receipts, Core ownership probes, and the explicit real-host blocker receipt.
- Material Kind: bounded host/controller implementation plus repository-owned regression coverage and fail-closed machine-gate evidence.

### Reproduced authority leak and bounded host repair

- Core projection against the broad Extension repository root sees multiple qualified Workspace surfaces, including nested acceptance-fixture Workspaces. This demonstrates why repository-wide discovery is not a valid live authoring authority surface by itself.
- The prior `endpointCatalog()` path combined host-indexed artifacts with broad shared projection and collapsed candidates by `${kind}:${label}`. A fixture Role with the same human label could therefore shadow another exact Role candidate in live presentation.
- Added `src/core/handoffEndpointSelection.ts` as a host-source-scoping controller only. It accepts Core-projected exact endpoint candidates for one explicitly selected Workspace id/root, retains only exact `.topics/**` candidates for that Workspace, deduplicates by exact identity, and deliberately never keys by human label.
- `src/packageBuilder.ts` now exposes `loadHandoffEndpointChoicesForSources()`. Each explicitly selected source is projected independently through shared Core `projectHandoffEndpoints`; blocked/unqualified source projections fail closed. The compatibility surface resolves visible VS Code Workspaces independently rather than treating the extension repository root as one semantic endpoint pool.
- `src/operatorTrees.ts` now builds Handoff authoring endpoint presentation from the selected Outgoing Workspace authoring root. Presentation includes Workspace id and artifact path, so exact same-label choices remain visibly distinct. No label-recency or repository-proximity rule selects semantic authority.
- `src/artifactAuthoringPanel.ts` now renders the precise VS Code-owned reason when Attach-to-Outgoing is unavailable, avoiding the stale claim that no Outgoing context exists when the actual state is a Workspace-selection mismatch.

### Host state and Workspace-byte ownership trace

- All three carried top-level Workspace artifacts tested in the accepted candidate qualify under the accepted Core before host handling. That evidence does not support host-side normalization, resealing, or semantic-byte mutation as a repair.
- The accepted Core can project the broad Extension root as several qualified Workspace candidates, including nested acceptance material; this is source-discovery evidence, not permission for the host to treat every nested Workspace as a live endpoint source.
- No fixture files were deleted or moved to hide the symptom. The production discovery boundary was corrected while the repository-owned fixtures remain in place.
- Existing Outgoing state is now reflected accurately in generic Artifact Authoring: Attach can be disabled because the artifact Workspace is not selected in Outgoing without presenting that as absence of an Outgoing context.

### Exact source delta

- `src/artifactAuthoringPanel.ts` SHA-256 `e5455657706f408a8ed168be51c1e0a818f779a9428a764a4fa0229e0acf4c4e`.
- `src/core/handoffEndpointSelection.ts` SHA-256 `1a2a378817953a53412ffb3849e2a4c26eef2418ffcbff2fbebf293d48ca3331`.
- `src/operatorTrees.ts` SHA-256 `cb6335392173ee69a3745b963832c55572745f623eda72bbaaefe0aa9f590c17`.
- `src/packageBuilder.ts` SHA-256 `1687017dba8ea8e445e6f8382a1be71191b941450d4f8845b83b6dd88e9a737d`.
- `test/extension-host/suite.cjs` SHA-256 `3f3ccce616b119ac1a07bcbcc61bf272a9f476abc5c3ba23f17705f1f24ec3f3`.
- `test/run.mjs` SHA-256 `b332c34dc2f61cd0158c171c9d113254a1df569c8b4c5168ca781b9e6267c40d`.
- Source stat versus the exact carried baseline: 4 source files changed, including one new bounded controller; 241 insertions and 64 deletions. Test stat: 2 files changed; 80 insertions and 18 deletions. Generated `dist` differs only as emitted build material and is not used as a substitute for clean dependency-backed validation.

### Repository-owned regression and acceptance coverage

- Added deterministic unit coverage that exact same-label endpoint candidates remain distinct and nested fixture paths are excluded when projecting an explicit Workspace source.
- The real-host suite now requires the production acceptance seams `tiinex.acceptance.endpointCatalog` and `tiinex.acceptance.authorHandoff` to be registered before execution.
- The suite drives the registered production controller path through pointerless Incoming, Replace, Outgoing continuation, endpoint catalog observation, exact participant confirmation including a positive multi-participant set, production Handoff authoring/Attach, Pack, Transport, restart/requalification, and Workspace-only Pack.
- The negative live-endpoint assertion rejects nested fixture/schema-example Role paths from a normal production Workspace without deleting those fixtures.
- The acceptance-only Handoff-authoring seam uses an exact qualified fixture Task parent rather than inventing a root Handoff, so any remaining authoring failure lands on the shared Core contract rather than a synthetic harness shape.

### Validation receipts

- Dependency-free TypeScript transpile over all 53 `src/**/*.ts` files: `errorDiagnostics: 0`.
- `node test/run.mjs` against emitted JavaScript: 56 tests pass before execution reaches the unavailable installed `@tiinex/core`; the new endpoint-source regression and existing participant-boundary tests pass before that environment stop.
- Extension Host suite syntax check passes.
- Normal dependency-backed typecheck remains blocked because type definition packages `node` and `vscode` are absent (`TS2688`).
- Canonical real-host invocation stops first with `tiinex.extension-host.vscode-cli-unavailable`. No `code`, `code-insiders`, or `codium` runtime is available on this machine.

### Shared Core / parallel-lane ownership findings

- The current accepted Core `project-handoff-endpoints` probes for the carried Business and Extension Workspace roots return `status: ready` with zero endpoint candidates. Kodax did not recreate missing endpoint semantics locally.
- A direct supported Core Handoff-creation probe with the exact qualified fixture Task parent can still block with `portable.draft-create.exact-result.unqualified` (`reason: exact-renderer-empty-or-unqualified`). This remains shared Core/Loom/Anchor reconciliation evidence, not a VS Code host workaround target.
- Because the carried top-level Workspace artifacts qualify before host mutation, the observed Workspace-only Pack integrity/conformance failure is not repaired speculatively in VS Code. Exact shared ownership remains for Loom/Anchor reconciliation.

## Preservation And Fidelity

- Preservation State: accepted Core source remained byte-preserved/read-only. The outer received Handoff carrier was not rewritten. The Extension VS Code change is bounded to host/controller/presentation and regression surfaces described above.
- Fidelity Notes: static/transpile/direct-test progress is reported only at its actual strength. Environment blockers are not reclassified as product failures, and missing real-host execution is not reclassified as a PASS.
- Known Losses: no Local-mode real VS Code Extension Host receipt, no Published-mode real VS Code Extension Host receipt, no clean npm typecheck/test receipt, and no integrated Loom+Kodax reconciled source receipt exist in this environment.

## Interpretation Limits

- Not Yet Used As: Sigma acceptance, Anchor integration acceptance, release approval, publication approval, deployment approval, or proof that the full cross-layer Recovery Task is closed.
- Does Not Prove: that shared Core endpoint/Handoff authoring mechanics are repaired, that the Workspace-only Pack blocker is resolved, that Local and Published Core real-host modes pass, or that parallel Loom changes reconcile cleanly with this host delta.
- Must Not Be Treated As: authority to add host-private Role/Handoff/material semantics, delete fixtures to hide discovery leakage, normalize semantic bytes in VS Code, or promote the candidate to Sigma without the missing machine and integration receipts.
- Disposition: blocked. The Kodax host-owned repair is complete at source/test level, but the first exact unresolved machine gate is `tiinex.extension-host.vscode-cli-unavailable`; shared Core findings return to Anchor/Loom for reconciliation.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-4-anchor-to-kodax-real-host-sigma-gate-host-boundary-recovery-package-correction.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-4-anchor-to-kodax-real-host-sigma-gate-host-boundary-recovery-package-correction.trace.md)
  - Value: jx4bFPPMdS3fZnB3OVxs9A0pgu8Y8ug0CechXDR1tjo

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 5zkye-59HxL6q7NOx6Lq0GN-VJ45Zx0ofSnJ_dN_W60