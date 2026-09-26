# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-26 20:47:14
  - Trace: [008-anchor-to-anchor-core-frozen-vs-code-grounding-bridge-recovery.trace.md](../../../handoffs/008-anchor-to-anchor-core-frozen-vs-code-grounding-bridge-recovery.trace.md)
  - Origin:
    - [relative](../../../handoffs/008-anchor-to-anchor-core-frozen-vs-code-grounding-bridge-recovery.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-26 21:30:56
  - Authors: Anchor
  - Why: Preserve the exact merge candidate, validation boundary, and full recovery state before Sigma real-host acceptance.
  - Summary: Core-frozen VS Code shared-Core human-parity bridge merge/test candidate after local qualification; real VS Code host remains Sigma gate.
  - Status: ready/local

---

# VS Code Re-entry — Shared-Core Human-Parity Bridge Merge Candidate Evidence

## Supported Claim Or Question

- Supported Claim Or Question: is the carried VS Code source now a bounded merge/test candidate for human use of the same frozen Core Tooling semantics already exercised by Tiinex/LLM workflows, without restoring V2/legacy semantics or modifying Core?
- Evidence Role: final local technical qualification and recovery evidence before Sigma performs real VS Code Extension Host/manual UI acceptance and merge disposition.
- Supported Conclusion: yes as a merge/test candidate. Core is byte-identical to the accepted frozen Core carried by the preceding full recovery. VS Code now uses Core-projected exact Handoff endpoint references for explicit Return To authoring, exposes Core-driven Incoming grounding state in the TreeView, migrates the historical Extension Host fixtures through current Core Tooling, and fixes multi-route Pack by consuming Core's exact projected route identity rather than passing a host-private route key as a Core transport selector. The strongest runnable local source/package qualification is green. A real VS Code Extension Host/UI run remains the deliberate Sigma acceptance gate because this sandbox has no VS Code CLI and lacks the normal VS Code/Node development type packages.

## Provenance

- Known Source: exact preceding five-Workspace recovery carrier `business-017-1-1-1-1-1-anchor-to-anchor.handoff-package.zip`; its exact frozen Core, App, Docs and Business Workspaces; the carried VS Code bridge source; current VS Code-only edits; Core-generated Extension Host fixture replacements; disposable exact-local-Core test harness results; routed multi-Handoff package roundtrip; and local VSIX packaging against the exact frozen sibling Core.
- Preservation Basis: Core remains frozen and byte-identical to the preceding accepted recovery package. Carry the complete current Business/Core/VS Code/App/Docs frontier in one successor Package V1 so Sigma can test and merge without reconstructing state from chat.
- Provenance Limits: no remote commit, merge, push, publication, release, published-Core update, or real VS Code Extension Host execution is claimed by this Evidence.

## Evidence Material

- Material: current VS Code source Workspace, frozen Core Workspace, migrated host fixtures, local unit/integration results, routed Package V1 roundtrip, package integration result, and VSIX packaging result.
- Material Kind: local bridge implementation and merge-candidate qualification evidence.
- Core freeze: direct recursive comparison against the Core Workspace embedded in the preceding full recovery package is byte-identical. No Core source change was made during this VS Code completion phase.
- VS Code source delta relative to the carried bridge baseline is bounded to 13 paths: `package.json`; `src/artifactAuthoringPanel.ts`; `src/core/receivedHandoff.ts`; `src/operatorTrees.ts`; `src/packageBuilder.ts`; `src/vscode/extensionHostAcceptance.ts`; `test/extension-host/fixtures/incoming-pointerless.handoff-package.zip`; `test/extension-host/fixtures/manifest.json`; the two fixture Handoffs under `test/extension-host/fixtures/source-workspace/.topics/handoffs/`; `test/extension-host/suite.cjs`; `test/package-integration.mjs`; and `test/run.mjs`.
- Return endpoint parity: Handoff authoring can select `Return To` from the same Core-projected endpoint catalog used for From/To and persists the exact qualified `Return To Reference`; labels are not converted into authority by host inference.
- Incoming grounding parity: the TreeView exposes `Ground Handoff` on qualified Incoming routes, invokes Core grounding against the exact orientation-qualified pointer, and renders Core receipt values for readiness, completion qualification, return transition, and return timing. VS Code does not calculate those semantic states.
- Fixture migration: Extension Host fixtures now use Workspace id `extension-host-acceptance` and exact `extension-host-acceptance::...` references. The two fixture Handoffs were reauthored through frozen Core Tooling with explicit return endpoint references; the pointerless fixture package was regenerated through frozen Core rather than manually resealed.
- Fixture qualification: frozen Core reports the pointerless fixture `ready` with zero audit findings, exactly one `extension-host-acceptance` Workspace and zero Handoff routes. The source fixture projects exactly two `qualified-exact` Handoff leaves (Anchor→Loom and Anchor→Kodax) and exact qualified endpoint candidates Anchor, Kodax, Loom, Pilot and Sigma.
- Multi-route Pack correction: VS Code's UI route key is no longer treated as a Core transport selector. For multi-route carriers, the host first consumes Core's complete carrier projection, matches the already-selected Workspace id plus Handoff path to exactly one qualified Core route, then reuses that exact Core route id for human transport presentation/manufacture. The host never constructs a Core route id. Shared route transport metadata is likewise joined back through Core's carrier projection rather than host route-id string conventions.
- Multi-route roundtrip: the current package builder produced one physical carrier containing both fixture routes, returned two distinct Core transport texts with exact Workspace/path/recipient metadata, and Core re-oriented the physical carrier as `ready` with the expected two routes.
- Disposable exact-local-Core bridge suite: 117/117 Tiinex VS Code bridge cases passed against a physically copied exact frozen Core runtime.
- Package integration: 5/5 scenarios passed, including pointerless Pack, reorientation without invented Handoff authority, the new multi-route Pack regression, idempotent/non-overwriting publication, and extracted VSIX execution of its bundled public Core entrypoint.
- Final local VSIX packaging: `dist/tiinex-vscode-0.1.7.vsix` was built successfully with sibling-source Core binding; 906 entries; bundled Core version `0.1.1`; bundled Core file count 790. Generated `dist`, VSIX bytes, local link state, and `node_modules` remain ignored runtime/build material and are not source authority.
- Typecheck environment boundary: the available TypeScript compiler emits the current source and reports only missing type-library diagnostics for `node` and `vscode`; those normal development packages are absent in this sandbox. No additional TypeScript diagnostic was produced. This is an environment limitation, not represented as a full typecheck PASS.
- Real-host boundary: the sandbox has no `code`, `code-insiders`, or `codium` CLI, so `test:extension-host` cannot execute here. Its acceptance suite has been updated to exercise the real registered TreeView/commands, explicit Return To reference, Incoming grounding, multi-route routed carrier, pointerless carrier, Transport requalification, and restart behavior. Sigma's Windows/VS Code run is the remaining product-level gate.

## Preservation And Fidelity

- Preservation State: Business, Core, VS Code, App, and Docs are all required in the successor recovery. Core is frozen/unchanged; VS Code carries the complete current merge candidate; App and Docs remain exact preserved context; Business adds this qualification Evidence and the Sigma landing/test Handoff.
- Fidelity Notes: no Package V2 compatibility, legacy package parser, host-private lineage allocator, host-private grounding/completion/return semantics, manual fixture resealing, or Core workaround was introduced. Generated `dist`, `.vscode/link`, `node_modules`, test scratch, logs, and local VSIX output are intentionally excluded from semantic source carriage.
- Known Losses: a full normal dependency-backed `tsc --noEmit`, real VS Code Extension Host acceptance, and Sigma's visual/manual TreeView acceptance are not available in this sandbox and remain explicit human/environment gates.

## Interpretation Limits

- Does Not Prove: Sigma acceptance, merge/commit/push, published Core compatibility at the currently declared published dependency line, release readiness, or successful manual UX acceptance on Sigma's machine.
- Not Yet Used As: remote mutation authority, release/publication evidence, or permission to change frozen Core.
- Must Not Be Treated As: permission to restore V2/legacy semantic paths, to make VS Code compensate for a future Core blocker, to infer qualified route/participant/return state from labels or filenames, or to claim Task completion from grounding/transport state.
- Disposition: deliver this exact five-Workspace source candidate to Sigma. Sigma should run the real VS Code Extension Host/manual TreeView workflow with the carried local Core, then either accept/merge the exact candidate or return one concrete blocker. Any newly demonstrated Core blocker must still be discussed with Sigma before Core is reopened.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [008-anchor-to-anchor-core-frozen-vs-code-grounding-bridge-recovery.trace.md](../../../handoffs/008-anchor-to-anchor-core-frozen-vs-code-grounding-bridge-recovery.trace.md)
  - Value: XbC1WcM0uI1tCFrk5K7qjQn2t8Yuhd8vQkO-9FwSErs

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 6IVnDV7tCIuUBt7EBNbAItOFOL7ZLUTcWpxG0Z3dxB8