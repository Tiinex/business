# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 19:47:47
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-anchor-to-loom-operator-context-top-level-workspace-boundary-rec.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-anchor-to-loom-operator-context-top-level-workspace-boundary-rec.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-anchor-to-loom-operator-context-top-level-workspace-boundary-rec.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 20:23:05
  - Authors: Loom
  - Why: Return the exact implementation and regression evidence required by the controlling Anchor corrective Task.
  - Summary: Bounded Core repair and integrated regression evidence for operator-context top-level Workspace ownership.
  - Status: ready/local

---

# Operator Context Top-Level Workspace Boundary Recovery — Loom Evidence

## Supported Claim Or Question

- Supported Claim Or Question: does the bounded Core correction prevent an explicit repository root from promoting nested independent fixture/schema Workspaces into that root's live top-level Workspace set while preserving multiple legitimate Workspace artifacts on the root's canonical `.topics/.workspaces` surface?
- Evidence Role: Loom implementation and regression evidence for the exact Anchor corrective Task.
- Supported Conclusion: yes for the qualified carried Core/Extension snapshots and the focused acceptance surface described below. The pre-fix Core reproduces `extension-host-acceptance, extension-vscode, vscode`; the corrected Core returns exactly `extension-vscode, vscode`, preserves legitimate sibling Workspace artifacts, passes focused Core compatibility coverage, and passes the Extension repository's 116-case integrated bridge suite in a disposable installed-Core harness.

## Provenance

- Known Source: exact Business, Core, and Extension VS Code Workspace snapshots qualified from the selected Anchor-to-Loom Handoff carrier `business-002-1-4-1-1-1-1-1-1-1-3-anchor-to-loom.handoff-package.zip` through Tiinex grounding.
- Controlling Task: [Operator Context Top-Level Workspace Boundary Recovery](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-operator-context-top-level-workspace-boundary-recovery.trace.md).
- Integrated Blocker Evidence: [Integrated Fan-In Operator Context Leakage Evidence](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-5-integrated-fan-in-operator-context-leakage-evidence.trace.md).
- Core Baseline: exact received `001-4-core.workspace.zip` source snapshot; pre-fix direct public `project-operator-context` over the exact Extension root returned Workspace ids `extension-host-acceptance`, `extension-vscode`, `vscode` with status `ready` and no error findings.
- Extension Consumer: exact received `001-5-extension-vscode.workspace.zip` source snapshot, treated read-only. The integrated test was executed only in a disposable copy.
- Preservation Basis: Core source was modified only in the carried writable Core workspace; the received Core ZIP remains preserved as the exact baseline, and the Extension source snapshot remains byte-unchanged.
- Provenance Limits: no remote repository state was queried or mutated; the integrated Extension run used a disposable local installed-Core harness as described below, and no real VS Code Extension Host execution is claimed.

## Evidence Material

- Material: Core correction in `src/tooling/portable/handoff/operatorContextProjection.js`. For each explicit host root, the existing descendant `rootFiles` set remains available to shared Handoff/Role projections, but Workspace package-source candidates are now taken only from direct files on that root's canonical `.topics/.workspaces` surface. A nested independent `.topics/.workspaces` surface is therefore not silently promoted into the parent root's live top-level Workspace set and instead requires its own explicit host root.
- Minimality: the rule is applied only at operator-context Workspace candidate selection. It does not add VS Code filtering, delete or move fixtures, reinterpret Workspace schema semantics, change endpoint/material closure, or alter nested material when that nested root is explicitly selected on its own.
- Regression: new `test/operator-context-workspace-boundary.test.mjs` constructs two qualified sibling Workspace artifacts on one selected root's top-level `.topics/.workspaces` surface plus one qualified nested fixture Workspace. The unmodified received Core fails the regression by returning all three Workspace ids; the corrected Core passes and returns exactly the two top-level siblings.
- Direct Integrated Reproduction After Correction: the corrected public Core CLI `project-operator-context` over the exact carried Extension root returns status `ready`, Workspace ids exactly `extension-vscode`, `vscode`, and zero error findings.
- Focused Core Compatibility: `node --test test/operator-context-workspace-boundary.test.mjs test/endpoint-role-route-binding.test.mjs test/bounded-handoff-carrier.test.mjs test/minimal-carrier-material-transport-projection.test.mjs test/manufacture-runtime-source-alignment.test.mjs` completed 17/17 PASS, 0 fail. This preserves the latest Loom endpoint Role/material-closure, bounded-carriage, pointerless and runtime/source-alignment regressions exercised by those files.
- Portable Qualification: `npm run test:portable` passed (`portable node surface imports`), and `npm run test:bootstrap` returned `status: embedded-qualified` with 516 runtime files and 5,837,966 runtime bytes.
- Integrated Extension Acceptance: the repository-owned `node test/run.mjs` completed **116/116 Tiinex VS Code bridge core cases passed**, including `installed Core runtime executes real operator-context and staged-only validation projections`, whose assertion requires exactly `extension-vscode, vscode`.
- Integrated Harness Boundary: the received Extension snapshot contains no `node_modules`. To exercise its repository-owned installed-Core binding path without mutating the qualified Extension source, Loom used a disposable Extension copy and copied the corrected Core candidate under `node_modules/@tiinex/core`. Only that disposable Core copy's `package.json` version field was set to the Extension lockfile's expected `0.35.0` so the existing published-binding/version assertion could execute; the corrected operator-context implementation/test bytes came from the candidate Core unchanged, and neither qualified source snapshot was modified by this harness adaptation.
- Exact Core Delta: relative to the received Core snapshot, 1 file is changed and 1 file is added; no files are removed. Changed: `src/tooling/portable/handoff/operatorContextProjection.js` (baseline SHA-256 `12b6ca619dbe3ef8a91698d9e08e3677e3a6bf348f6f0741d899c1fc77f3102f`, corrected SHA-256 `c8fe92bab4a0b61ad650e9ed0886d3afb51c8410f5dfaf1435904b8f170d28ed`). Added: `test/operator-context-workspace-boundary.test.mjs`.
- Material Kind: exact source delta plus deterministic Core and Extension execution receipts.

## Preservation And Fidelity

- Preservation State: received Business/Core/Extension carrier material remains preserved; only the writable Core candidate contains product-source changes, and Business receives only new return Evidence/Handoff artifacts plus runtime-only continuation state.
- Fidelity Notes: the direct pre-fix and post-fix Workspace sets were observed from the same Extension root. The 17/17 Core count and 116/116 Extension count are exact completed test receipts. Portable/bootstrap checks completed successfully after the Core change.
- Known Losses: this evidence does not claim a separate full `node --test test/*.test.mjs` Core wildcard suite run. Acceptance is bounded to the controlling Task's focused Core regressions, portable/bootstrap qualification, the exact direct reproduction, and the full repository-owned Extension bridge suite. Real VS Code Extension Host execution remains outside this evidence, consistent with the controlling integrated blocker evidence.

## Interpretation Limits

- Does Not Prove: that every nested Workspace is invalid in every context; a nested Workspace remains eligible when its own root is explicitly selected and qualified.
- Must Not Be Treated As: authorization to mutate Extension VS Code, Docs semantics, fixtures, remote repositories, releases, deployments, or Sigma state.
- Not Yet Used As: Anchor acceptance, Sigma acceptance, release approval, publication authority, or deployment authority.
- Does Not Mean: operator context now derives semantic Workspace identity from path shape alone; qualification still comes from exact Workspace artifact audit, while the new path rule only bounds which qualified Workspace artifacts belong to one explicit host root's top-level live set.
- Must Not Be Used To Claim: whole-program acceptance, real Extension Host acceptance, or that unrelated Core suites were exhaustively rerun.
- Disposition: return the exact bounded Core candidate and this evidence to Anchor for reconciliation; no self-promotion to Sigma.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-anchor-to-loom-operator-context-top-level-workspace-boundary-rec.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-anchor-to-loom-operator-context-top-level-workspace-boundary-rec.trace.md)
  - Value: E_cAj7D8sjfCxhtEqOyf-aq1GK6vlMoLGKisSRk3I2A

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: B-oT6wPBUAdvZlBBdD7etMHVm0LOiHKvxsmkJLGA2dQ