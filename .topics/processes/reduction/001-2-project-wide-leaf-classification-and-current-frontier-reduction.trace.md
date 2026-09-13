# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-12 22:01:30
  - Trace: [001-1-anchor-to-anchor-reduction-major-001-current-frontier-and-histor.trace.md](001-1-anchor-to-anchor-reduction-major-001-current-frontier-and-histor.trace.md)
  - Origin:
    - [relative](001-1-anchor-to-anchor-reduction-major-001-current-frontier-and-histor.trace.md)
- Current
  - Current Schema: tiinex.reduction.v1
  - Created At: 2026-09-12 22:32:44
  - Authors: Anchor
  - Why: Return a bounded project-wide Reduction that makes fresh Anchor recovery readable while preserving unresolved work, protected integrity mismatches, and exact lineage.
  - Summary: Classify the qualified 113 real Handoff leaves plus three fixtures, preserve the eight-item attention frontier, and compact terminal or superseded lineage without deletion.
  - Status: ready/local

---

# Reduction Major 001 — Project-Wide Leaf Classification And Current-Frontier Carry-Forward

## Source Context

- Controlling Task: `business::.topics/processes/reduction/001-reduction-major-001-current-frontier-and-historical-leaf-reducti.trace.md`.
- Received route: `business::.topics/processes/reduction/001-1-anchor-to-anchor-reduction-major-001-current-frontier-and-histor.trace.md`.
- Current Master Recovery basis: `business::.topics/initiatives/refactor/orchestration/handoffs/012-1-anchor-full-recovery-grounding-major-001-integrated.trace.md`, with the immediately prior full-recovery checkpoints used only to preserve explicitly still-open VS Code, Playthings and human-gate obligations.
- Material scope: the exact 16 qualified Workspace snapshots carried by the received Handoff package and materialized through Tiinex `ground --continue/--materialize-workspace`; no native carrier archaeology or remote state was used for classification.
- Leaf projection basis: Tiinex `project-handoff-leaves` over each carried Workspace plus a merged projection cross-check. The per-Workspace projection produced 116 qualified Handoff leaves; 113 are program artifacts under `.topics`, and 3 are fixture/test-only leaves.
- Canonical reduction semantics: `docs::.topics/.schemas/reduction/tiinex.reduction.v1.schema.md` as qualified Required Context.

### Classification Basis Codes

- **B1 — current-route:** the exact selected Reduction Major 001 route is the controlling active handoff.
- **B2 — current-vscode:** the latest Master Recovery explicitly retains VS Code Major 003 as active/unaccepted and identifies the Transport filename/scanability delegation as the next live repair.
- **B3 — current-grounding-blocker:** the latest Master Recovery explicitly retains the independent fresh-successor behavioral replay as an open gate.
- **B4 — current-sigma-gate:** the latest Master Recovery explicitly retains the Site/Playthings real-browser execution as a Sigma host/human gate.
- **B5 — terminal-return:** the leaf is an explicit qualified specialist/completed return whose transfer is not retained as an open action by the latest Master Recovery. This class does not claim project/release closure beyond the returned bounded work.
- **B6 — superseded-frontier:** a later qualified complete Master Recovery/current Workspace frontier carries the operative state and does not retain this leaf as open. This classification is based on the later qualified recovery, not filename age.
- **B7 — unresolved-pilot-disposition:** the Pilot return explicitly leaves Anchor accept/reject disposition open, and no later qualified current-Recovery evidence found in this pass resolves that individual visual candidate.
- **B8 — fixture:** qualified Handoff-shaped material outside `.topics` carried for fixture/test purposes, not program frontier work.

## Carry-Forward State

- **Raw qualified leaf set remains intact:** 116 leaves total; 113 real program leaves and 3 fixture/test-only leaves. Nothing is deleted, hidden, or rewritten by this Reduction.
- **Current attention set:** 8 of 113 real program leaves — 2 active/current, 1 waiting/blocked, 1 human gate, and 4 genuinely unresolved Pilot visual-return dispositions.
- **Terminal/historical set:** 105 of 113 real program leaves — 41 completed/accepted terminal returns and 64 superseded historical leaves.
- **Readability effect:** a fresh Anchor can scan 8 attention-bearing leaves instead of treating all 113 real leaves as potentially actionable, a reduction of 105 attention candidates (92.9%) while preserving navigation to every source leaf.
- **Active/current:**
  - Business Reduction Major 001 route `.topics/processes/reduction/001-1-anchor-to-anchor-reduction-major-001-current-frontier-and-histor.trace.md`.
  - Extension VS Code Transport filename fidelity/scanability repair `.topics/refactor/orchestration/001-3-6-4-1-3-1-1-1-2-1-2-2-1-2-1-2-1-2-1-1-anchor-to-kodax-vs-code-major-003-transport-filename-fidelity-an.trace.md`; live candidate remains unaccepted and the carried Extension VS Code snapshot remains the last accepted baseline.
- **Waiting/blocked:**
  - Grounding Major 001 independent fresh-successor behavioral gate `.topics/processes/gpt/grounding/002-2-1-2-2-1-2-anchor-to-anchor-grounding-major-001-independent-replay-return.trace.md`; machine cold-start qualification does not close the independent behavioral replay requirement.
- **Human gate:**
  - Site Major 005 real-browser execution gate `.topics/refactor/orchestration/handoffs/002-1-1-1-anchor-to-sigma-site-major-005-real-browser-execution-gate.trace.md` assigned to Sigma; this is a technical host gate and does not itself constitute Playthings product acceptance.
- **Unresolved visual dispositions:** four Pilot→Anchor Root visual returns remain explicit accept/reject candidates (portrait/gate, tiles, props, inspect/observe verb). They remain visible and must not be silently treated as accepted or stale.
- **Protected non-leaf integrity findings:** Docs lineage resolution reports exactly two `lineage.parent.integrityMismatch` errors. Both remain protected from terminal/stale classification:
  - `docs::.topics/.schemas/tiinex.workspace.v1.schema.md` → declared pinned Root parent.
  - `docs::.topics/.validators/tiinex-reduction-destructive-lineage-eligibility-v1.validator.md` → declared validation-method parent.
- **Other retained current dependencies from the latest Master Recovery:** shared Feedback create-capability gap, exact locked VS Code toolchain availability, deferred integrated Sigma VS Code acceptance, Playthings coherent continuation/human gating, and the Tiinex organization `.github` recovery gap. These are not converted into Handoff-leaf state by this Reduction.

### Workspace Summary

| Workspace | Qualified leaves | Program leaves | Active | Blocked | Human gate | Completed terminal | Superseded | Unresolved | Fixtures |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| business | 28 | 28 | 1 | 1 | 0 | 5 | 21 | 0 | 0 |
| site | 30 | 30 | 0 | 0 | 1 | 16 | 13 | 0 | 0 |
| verse-playthings | 24 | 24 | 0 | 0 | 0 | 3 | 17 | 4 | 0 |
| extension-vscode | 12 | 12 | 1 | 0 | 0 | 1 | 10 | 0 | 0 |
| core | 8 | 8 | 0 | 0 | 0 | 8 | 0 | 0 | 0 |
| docs | 7 | 7 | 0 | 0 | 0 | 6 | 1 | 0 | 0 |
| cli | 3 | 2 | 0 | 0 | 0 | 1 | 1 | 0 | 1 |
| extension-chrome | 1 | 1 | 0 | 0 | 0 | 0 | 1 | 0 | 0 |
| provider-native | 1 | 1 | 0 | 0 | 0 | 1 | 0 | 0 | 0 |
| app | 2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 2 |
| interop-native | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| interop-openai | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| provider-github | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| runtime-native | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| verse-atlas | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| verse-native | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |

### Exact Leaf Inventory

#### business

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `.topics/business-development/003-anchor-to-anchor-foundation-reanchor-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Foundation Conversation Re-anchor — Anchor To Anchor |
| `.topics/initiatives/001-6-1-1-anchor-to-sigma-isolated-business-cold-start-acceptance-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Isolated Business Repository-Only Cold-Start Acceptance — Anchor To Sigma |
| `.topics/business-development/002-1-1-anchor-to-sigma-lineage-projection-correction-retry-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Business Major 002 Lineage Projection Correction — Sigma Retry |
| `.topics/initiatives/001-3-6-1-1-anchor-to-sigma-full-source-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Anchor to Sigma — complete extraction checkpoint |
| `.topics/initiatives/001-3-6-2-1-anchor-to-sigma-full-source-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Anchor to Sigma — complete extraction checkpoint |
| `.topics/initiatives/001-3-6-3-2-anchor-to-sigma-parity-source-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Anchor to Sigma — full source parity and publishing |
| `.topics/initiatives/refactor/extensions/handoffs/001-refactor-anchor-to-vs-code-anchor-current-shared-context-refresh.trace.md` | Anchor → Anchor | superseded historical | B6 | Refactor Anchor → VS Code Anchor: current shared-context refresh |
| `.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-2-1-sigma-pack-fix-full-source.trace.md` | Anchor → Sigma | superseded historical | B6 | Sigma full-source delivery after Pack filename repair |
| `.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-after-glimmer-stream-delegation.trace.md` | Anchor → Anchor | superseded historical | B6 | Anchor full recovery after Glimmer stream delegation |
| `.topics/initiatives/refactor/handoffs/002-anchor-full-recovery-after-stream-orchestration-and-playthings-d.trace.md` | Anchor → Anchor | superseded historical | B6 | Anchor full recovery after stream orchestration and Playthings delegation |
| `.topics/initiatives/refactor/handoffs/003-anchor-full-recovery-after-stream-orchestration-playthings-and-v.trace.md` | Anchor → Anchor | superseded historical | B6 | Anchor full recovery after stream orchestration, Playthings and VS Code delegations |
| `.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-1-loom-to-anchor-carrier-major-002-lineage-safety-hardening-return.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Return qualified Core lineage-safety repairs and bounded Business evidence for Anchor integration. |
| `.topics/initiatives/refactor/orchestration/handoffs/003-anchor-to-kodax-viewer-carrier-major-002-poc-replacement-reconci.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor to Kodax — Viewer Carrier Major 002 PoC Replacement Reconciliation |
| `.topics/initiatives/refactor/orchestration/handoffs/004-anchor-to-prism-verse-playthings-carrier-major-002-browser-reali.trace.md` | Anchor → Prism | superseded historical | B6 | Anchor to Prism — Verse Playthings Carrier Major 002 Browser Reality Qualification |
| `.topics/initiatives/refactor/orchestration/handoffs/005-anchor-to-kodax-extension-vs-code-carrier-major-002-operator-com.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor to Kodax — Extension VS Code Carrier Major 002 Operator Completion Tranche |
| `.topics/initiatives/refactor/orchestration/handoffs/006-anchor-to-glimmer-stream-audience-grounding-refresh.trace.md` | Anchor → Glimmer | superseded historical | B6 | Anchor to Glimmer — Stream Audience Grounding Refresh |
| `.topics/initiatives/refactor/orchestration/handoffs/008-1-kodax-to-anchor-extension-chrome-carrier-major-002-bounded-opera.trace.md` | Kodax → Anchor | completed/accepted terminal | B5 | Kodax to Anchor — Extension Chrome Carrier Major 002 Bounded Operator Automation Return |
| `.topics/initiatives/refactor/orchestration/handoffs/009-1-1-anchor-full-recovery-carrier-major-002-after-loom-lineage-safety.trace.md` | Anchor → Anchor | superseded historical | B6 | Anchor Full Recovery — Carrier Major 002 After Loom Lineage-Safety Merge |
| `.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-site005-return-sigma-browser-gate.trace.md` | Anchor → Anchor | superseded historical | B6 | Anchor Full Recovery — Site 005 Return And Sigma Browser Gate |
| `.topics/processes/gpt/grounding/001-1-2-1-1-2-anchor-to-anchor-standard-successor-grounding-acceptance-return.trace.md` | Anchor → Anchor | completed/accepted terminal | B5 | Return the standard fresh-Anchor probe decisions, qualified Evidence, current Core007/Docs005 frontier, one non-blocking grounding-friction note, and retained acceptance boundaries. |
| `.topics/processes/gpt/grounding/001-1-2-2-1-2-fresh-anchor-to-anchor-perturbed-successor-grounding-acceptance.trace.md` | Anchor → Anchor | superseded historical | B6 | Fresh Anchor To Anchor — Perturbed Successor Grounding Acceptance Return |
| `.topics/processes/gpt/grounding/001-1-2-4-1-2-anchor-to-anchor-coverage-corrected-standard-successor-return.trace.md` | Anchor → Anchor | completed/accepted terminal | B5 | Return the full twelve-category coverage-corrected standard successor decisions, recovered frontier/root/human gates, exact authority references, uncertainties and disclosed isolation caveat. |
| `.topics/processes/gpt/grounding/001-1-2-4-2-2-anchor-to-anchor-coverage-corrected-perturbed-successor-return.trace.md` | Anchor → Anchor | completed/accepted terminal | B5 | Return the completed fresh perturbed successor matrix with all twelve decisions, exact authority, preserved uncertainty and independent-grading boundary. |
| `.topics/processes/gpt/grounding/001-1-2-4-3-2-anchor-to-anchor-clean-standard-successor-replay-return-with-iso.trace.md` | Anchor → Anchor | superseded historical | B6 | Anchor To Anchor — Clean Standard Successor Replay Return With Isolation Caveat |
| `.topics/processes/gpt/grounding/001-1-2-4-5-1-anchor-to-anchor-selector-isolated-standard-successor-replay-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Anchor To Anchor — Selector-Isolated Standard Successor Replay |
| `.topics/initiatives/refactor/orchestration/handoffs/011-anchor-full-recovery-authoring-accepted-grounding-hardening-acti.trace.md` | Anchor → Anchor | superseded historical | B6 | Anchor Full Recovery — Authoring Accepted, Grounding Hardening Active, Transport Repair Ready |
| `.topics/processes/gpt/grounding/002-2-1-2-2-1-2-anchor-to-anchor-grounding-major-001-independent-replay-return.trace.md` | Anchor → Anchor | waiting/blocked | B3 | Anchor To Anchor — Grounding Major 001 Independent Replay Return |
| `.topics/processes/reduction/001-1-anchor-to-anchor-reduction-major-001-current-frontier-and-histor.trace.md` | Anchor → Anchor | active/current | B1 | Anchor To Anchor — Reduction Major 001 Current Frontier And Historical Leaf Reduction |

#### site

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `.topics/tooling/001-2-1-1-1-loom-to-anchor-scoped-export-parent-boundary-impact-return-handoff.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Scoped Export Parent Boundary Impact — Anchor Return Handoff |
| `.topics/tooling/001-1-1-1-1-loom-to-anchor-validation-checkpoint-efficiency-return-handoff.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Validation And Checkpoint Efficiency — Anchor Return Handoff |
| `.topics/tooling/002-1-1-1-1-1-1-1-1-1-1-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-loom-foundation-human-first-cli-carrier-ux-handoff.trace.md` | Anchor → Loom | superseded historical | B6 | Foundation Human-First CLI And Carrier UX — Anchor To Loom |
| `.topics/tooling/005-2-3-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-axiom-pinned-parent-continuity-reconciliation-handoff.trace.md` | Anchor → Axiom | superseded historical | B6 | Pinned Historical Parent Continuity Reconciliation — Anchor To Axiom |
| `.topics/tooling/005-2-3-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-axiom-to-anchor-pinned-parent-continuity-reconciliation-return-handoff.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Pinned Historical Parent Continuity Reconciliation — Axiom Return To Anchor |
| `.topics/tooling/007-3-1-1-1-1-1-1-loom-to-anchor-human-first-common-cli-output-density-correction-return-handoff.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Human-First Common CLI Output Density Correction — Loom To Anchor Final Return |
| `.topics/tooling/007-4-1-1-anchor-to-anchor-human-first-common-cli-major-checkpoint-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Human-First Common CLI Stable Checkpoint — Anchor To Fresh Anchor |
| `.topics/tooling/007-4-1-1-1-anchor-to-anchor-human-first-common-cli-major-checkpoint-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Human-First Common CLI Stable Checkpoint — Anchor To Fresh Anchor |
| `.topics/tooling/007-4-1-1-2-1-anchor-to-loom-schema-invalid-author-repair-common-path-ergonomics-handoff.trace.md` | Anchor → Loom | superseded historical | B6 | Schema-Invalid Author Repair Common-Path Ergonomics — Anchor To Loom |
| `.topics/viewer/004-1-anchor-to-anchor-post-reduction-artifact-action-major-checkpoint-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Post-Reduction Viewer Artifact + Action Major Checkpoint — Anchor To Anchor |
| `.topics/tooling/008-1-1-1-1-anchor-to-anchor-site-reduction-finalization-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Repo-Scale Site Reduction Finalization — Anchor To Anchor |
| `.topics/tooling/010-1-1-1-axiom-to-anchor-reduction-safety-contract-return-handoff.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Reduction Safety Contract — Axiom To Anchor |
| `.topics/tooling/010-2-1-1-loom-to-anchor-reduction-audit-repair-parity-return-handoff.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Loom returns the bounded Site-local parity implementation and validation Evidence to Anchor with the current Reduction Parent-span blocker explicit and fail-closed. |
| `.topics/viewer/005-1-1-1-kodax-to-anchor-node-graph-verse-projection-return-handoff.trace.md` | Kodax → Anchor | completed/accepted terminal | B5 | Node Graph Verse Projection — Kodax To Anchor Return |
| `.topics/tooling/011-1-anchor-to-axiom-schema-slice-factory-semantics-handoff.trace.md` | Anchor → Axiom | superseded historical | B6 | Schema Slice Factory Semantics — Anchor To Axiom |
| `.topics/tooling/011-3-anchor-to-axiom-schema-factory-canonical-repair-handoff.trace.md` | Anchor → Axiom | superseded historical | B6 | Schema Factory Canonical Repair — Anchor To Axiom |
| `.topics/tooling/011-2-1-1-loom-to-anchor-schema-slice-factory-mechanics-return-handoff.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Loom returns the shared schema-factory mechanics and conformance evidence to Anchor with Decision and Evidence semantic blockers explicit for Axiom reconciliation. |
| `.topics/tooling/011-3-2-axiom-to-anchor-schema-factory-canonical-repair-return-handoff.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Schema Factory Canonical Repair — Axiom To Anchor Return |
| `.topics/tooling/011-4-1-1-loom-to-anchor-schema-factory-reverification-transport-closure-handoff.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Schema Factory Re-verification + Transport Closure — Loom To Anchor |
| `.topics/tooling/011-6-1-1-loom-to-anchor-generic-cross-workspace-endpoint-role-carriage-repair-return-handoff.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Generic Cross-Workspace Endpoint Role Carriage Repair — Loom To Anchor |
| `.topics/tooling/011-5-1-2-1-kodax-to-anchor-schema-factory-viewer-proof-handoff.trace.md` | Kodax → Anchor | completed/accepted terminal | B5 | Kodax → Anchor Schema Factory Viewer Proof Return Handoff |
| `.topics/tooling/011-6-1-anchor-to-axiom-evidence-parent-lineage-validator-semantic-adjudication-handoff.trace.md` | Anchor → Axiom | superseded historical | B6 | Anchor → Axiom Evidence Parent-Lineage Validator Semantic Adjudication Handoff |
| `.topics/tooling/011-6-3-axiom-to-anchor-evidence-parent-lineage-validator-disposition-return-handoff.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Axiom To Anchor — Evidence Parent-Lineage Validator Disposition Return |
| `.topics/tooling/016-2-anchor-to-loom-common-author-continuation-repair-handoff.trace.md` | Anchor → Loom | superseded historical | B6 | Common Author Continuation Schema Authority Repair — Anchor To Loom |
| `.topics/tooling/017-anchor-to-anchor-context-reset-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Cold-transfer current Major 008 coordination to a fresh Anchor with task 016 as the immediate blocker and established transport discipline preserved. |
| `.topics/tooling/020-1-1-1-1-axiom-to-anchor-work-provenance-grounding-semantics-return-handoff.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Axiom → Anchor Work-Provenance Grounding Semantics Return |
| `.topics/tooling/023-3-1-1-1-axiom-to-anchor-major-012-pointerless-carrier-semantics-return-handoff.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Axiom To Anchor Major 012 Pointerless Carrier Semantics Return Handoff |
| `.topics/tooling/023-3-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-major-012-watcher-session-operator-interaction-repair-loom-to-anchor-return.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Return the technically qualified Tiinex VS Code 0.1.4 watcher-session and packaged Operator-interaction repair with focused regressions and deterministic VSIX. |
| `.topics/tooling/024-3-1-anchor-to-sigma-major-013-vscode-0-1-7-dogfood-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Major 013 VS Code 0.1.7 — Anchor To Sigma Dogfood |
| `.topics/refactor/orchestration/handoffs/002-1-1-1-anchor-to-sigma-site-major-005-real-browser-execution-gate.trace.md` | Anchor → Sigma | human gate | B4 | Anchor To Sigma — Site Major 005 Real Browser Execution Gate |

#### verse-playthings

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `.topics/viewer/playthings/graphics/root/001-1-anchor-to-pilot-root-verb-generation-handoff.trace.md` | Anchor → Pilot | superseded historical | B6 | Root Verb — Anchor To Pilot |
| `.topics/viewer/playthings/graphics/root/001-2-2-pilot-to-anchor-root-portrait-generation-return-handoff.trace.md` | Pilot → Anchor | genuinely orphaned/unresolved | B7 | Root Portrait / Root Gate — Pilot To Anchor Return |
| `.topics/viewer/playthings/graphics/root/001-3-2-pilot-to-anchor-root-tiles-return-handoff.trace.md` | Pilot → Anchor | genuinely orphaned/unresolved | B7 | Root Tiles — Pilot To Anchor Return |
| `.topics/viewer/playthings/graphics/root/001-6-pilot-to-anchor-root-verb-generation-return-handoff.trace.md` | Pilot → Anchor | genuinely orphaned/unresolved | B7 | Root Verb Inspect/Observe Result — Pilot To Anchor Return |
| `.topics/viewer/playthings/graphics/root/001-4-2-pilot-to-anchor-root-props-generation-return-handoff.trace.md` | Pilot → Anchor | genuinely orphaned/unresolved | B7 | Root Props — Pilot To Anchor Return |
| `.topics/viewer/playthings/development/001-3-1-anchor-to-anchor-playthings-corrected-source-transport-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Playthings Corrected Source Transport — Anchor To Anchor |
| `.topics/viewer/playthings/development/design/semantics/001-1-anchor-to-anchor-designer-review-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Playthings Semantic Designer Review — Anchor To Anchor |
| `.topics/viewer/playthings/development/runtime/001-2-anchor-to-anchor-playthings-runtime-planning-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Playthings Runtime Planning — Anchor To Anchor |
| `.topics/viewer/playthings/development/runtime/001-3-anchor-to-anchor-playthings-lineage-convention-correction-handoff.trace.md` | Anchor → Anchor | superseded historical | B6 | Playthings Lineage Convention Correction — Anchor To Anchor |
| `.topics/viewer/playthings/development/runtime/001-5-anchor-to-sigma-host-neutral-foundations-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Host-Neutral Foundations — Anchor To Sigma |
| `.topics/viewer/playthings/development/runtime/001-6-anchor-to-sigma-package-companion-scene-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Package Companion Scene — Anchor To Sigma |
| `.topics/viewer/playthings/development/runtime/001-7-anchor-to-sigma-npm-release-readiness-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | npm Release Readiness — Anchor To Sigma |
| `.topics/viewer/playthings/development/runtime/001-8-1-anchor-to-anchor-playthings-continuation.trace.md` | Anchor → Anchor | superseded historical | B6 | Playthings Anchor successor — public App integration |
| `.topics/viewer/playthings/development/runtime/001-8-3-anchor-to-anchor-root-renderer-continuation.trace.md` | Anchor → Anchor | superseded historical | B6 | Playthings Anchor successor — Root renderer scaffold to spatial assembly |
| `.topics/viewer/playthings/development/runtime/001-8-2-2-2-anchor-to-sigma-spatial-world-candidate-checkpoint-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Spatial-world candidate checkpoint — Anchor to Sigma |
| `.topics/viewer/playthings/development/runtime/architecture/001-2-2-2-anchor-to-sigma-windows-npm-subprocess-portability-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Playthings Windows publication-path hotfix return |
| `.topics/viewer/playthings/development/runtime/001-8-2-2-3-2-anchor-to-sigma-multi-surface-renderer-checkpoint-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Multi-surface renderer checkpoint — Anchor to Sigma |
| `.topics/viewer/playthings/development/runtime/001-8-2-2-3-3-2-anchor-to-sigma-immersive-test-checkpoint-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Immersive Playthings experience checkpoint — Anchor to Sigma |
| `.topics/viewer/playthings/development/runtime/001-8-2-2-3-3-3-2-anchor-to-sigma-experience-candidate-handoff.trace.md` | Anchor → Sigma | superseded historical | B6 | Playthings Experience Candidate 1 — Anchor to Sigma, hold for Turn 2 |
| `.topics/refactor/handoffs/001-refactor-anchor-to-playthings-anchor-turn-2-integration.trace.md` | Refactor Anchor → Playthings Anchor | superseded historical | B6 | Refactor Anchor to Playthings Anchor — Turn 2 integration |
| `.topics/refactor/qualification/001-2-playthings-to-anchor-carrier-major-001-qualification-return.trace.md` | Playthings → Anchor | completed/accepted terminal | B5 | Playthings to Anchor — Carrier Major 001 Qualification Return |
| `.topics/refactor/qualification/001-4-prism-to-anchor-verse-playthings-carrier-major-002-browser-reali.trace.md` | Prism → Anchor | completed/accepted terminal | B5 | Prism to Anchor — Verse Playthings Carrier Major 002 Browser Reality Return |
| `.topics/refactor/orchestration/001-1-1-anchor-to-prism-playthings-major-003-real-browser-sigma-test-readiness-handoff.trace.md` | Anchor → Prism | superseded historical | B6 | Anchor To Prism — Playthings Major 003 Real Browser Sigma Test Readiness |
| `.topics/refactor/qualification/003-prism-to-anchor-playthings-major-003-real-browser-readiness-retu.trace.md` | Prism → Anchor | completed/accepted terminal | B5 | Prism To Anchor — Playthings Major 003 Real Browser Readiness Return |

#### extension-vscode

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `.topics/refactor/handoffs/001-refactor-anchor-to-vs-code-anchor-turn-2-integration.trace.md` | Refactor Anchor → VS Code Anchor | superseded historical | B6 | Refactor Anchor to VS Code Anchor — Turn 2 integration |
| `.topics/refactor/operator/handoffs/009-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-vs-code-pack-name-verification-and-authoring-dogfood-delegation.trace.md` | Anchor → Kodax | superseded historical | B6 | VS Code Pack-name verification and authoring dogfood continuation |
| `.topics/refactor/operator/handoffs/010-kodax-to-anchor-extension-vs-code-repo-owned-recovery-checkpoint.trace.md` | Kodax → Anchor | completed/accepted terminal | B5 | Preserve the current repo-owned extension-vscode checkpoint and escalate exact shared blockers. |
| `.topics/refactor/orchestration/001-1-1-anchor-to-kodax-vs-code-major-003-schema-scalable-artifact-authoring-handoff.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor To Kodax — VS Code Major 003 Schema-Scalable Artifact Authoring |
| `.topics/refactor/orchestration/001-1-2-1-anchor-to-kodax-vs-code-major-003-operator-completion-revision-handoff.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor To Kodax — VS Code Major 003 Operator Completion Revision |
| `.topics/refactor/orchestration/001-3-6-4-1-1-anchor-to-kodax-vs-code-major-003-artifact-continuity-preview-navigation-revision-handoff.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor To Kodax — VS Code Major 003 Artifact Continuity Preview And Navigation Revision |
| `.topics/refactor/orchestration/001-3-6-4-1-3-1-1-1-1-anchor-to-kodax-vs-code-major-003-final-generic-authoring-local-core-acceptance-handoff.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor To Kodax — VS Code Major 003 Final Generic Authoring And Local-Core Acceptance |
| `.topics/refactor/orchestration/001-3-6-4-1-3-1-1-1-2-1-2-1-anchor-to-kodax-vs-code-major-003-sigma-git-automation-scm-ergonomics-repair-handoff.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor To Kodax — VS Code Major 003 Git Automation And SCM Ergonomics Repair |
| `.topics/refactor/orchestration/001-3-6-4-1-3-1-1-1-2-1-2-2-1-1-anchor-to-kodax-vs-code-major-003-transport-queue-qualified-delivery-ux-handoff.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor To Kodax — VS Code Major 003 Transport Queue And Qualified Delivery UX |
| `.topics/refactor/orchestration/001-3-6-4-1-3-1-1-1-2-1-2-2-1-2-1-1-anchor-to-kodax-vs-code-major-003-incoming-merge-conflict-materialization-handoff.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor To Kodax — VS Code Major 003 Incoming Merge Conflict Materialization |
| `.topics/refactor/orchestration/001-3-6-4-1-3-1-1-1-2-1-2-2-1-2-1-2-1-1-anchor-to-kodax-vs-code-major-003-first-class-artifact-authoring.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor To Kodax — VS Code Major 003 First-Class Artifact Authoring Discoverability |
| `.topics/refactor/orchestration/001-3-6-4-1-3-1-1-1-2-1-2-2-1-2-1-2-1-2-1-1-anchor-to-kodax-vs-code-major-003-transport-filename-fidelity-an.trace.md` | Anchor → Kodax | active/current | B2 | Anchor To Kodax — VS Code Major 003 Transport Filename Fidelity And Scanability Repair |

#### core

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `.topics/refactor/tooling/handoffs/001-1-loom-to-anchor-minimal-context-tooling-return.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Bounded Core Tooling result for selective package-parent Workspace carriage and VS Code consumer audit. |
| `.topics/refactor/security/handoffs/001-1-core-secure-transport-v1-implementation-anchor.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Qualified host-neutral Core Secure Transport V1 mechanics, exact security/roundtrip/backward-compatibility evidence, and bounded concrete-profile/schema-target Docs review findings returned to Anchor. |
| `.topics/refactor/security/handoffs/002-1-core-secure-transport-v1-conformance-corrections-anchor.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Core Secure Transport V1 conformance corrections → Anchor |
| `.topics/refactor/tooling/handoffs/002-1-source-frontier-comparison-tooling-to-anchor.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Source frontier comparison Tooling → Anchor |
| `.topics/refactor/orchestration/handoffs/001-1-2-loom-to-anchor-historical-parent-schema-authority-recovery-return.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Loom to Anchor — Historical Parent schema-authority recovery return |
| `.topics/refactor/orchestration/handoffs/001-2-2-loom-to-anchor-core-major-003-manufacture-runtime-source-hygiene-alignment-return.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Loom to Anchor — Core Major 003 Manufacture Runtime And Source Hygiene Alignment Return |
| `.topics/refactor/orchestration/handoffs/002-1-1-1-1-loom-to-anchor-core-major-007-per-field-schema-reference-authori.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Loom To Anchor — Core Major 007 Per-Field Schema Reference Authority Enforcement Return |
| `.topics/refactor/orchestration/handoffs/003-1-1-1-1-1-loom-to-anchor-core-major-009-minimal-carrier-material-represent.trace.md` | Loom → Anchor | completed/accepted terminal | B5 | Loom To Anchor — Core Major 009 Minimal Carrier, Material Representation, And Transport Projection Return |

#### docs

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `.topics/recovery/002-1-1-1-1-1-axiom-to-anchor-bounded-workspace-representation-return-handoff.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Bounded Workspace Representation — Axiom Return To Anchor |
| `.topics/role-authority/001-1-1-1-1-1-1-1-axiom-to-anchor-human-first-domain-neutral-canonical-clarification-return-handoff.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Human-First And Domain-Neutral Canonical Clarification — Axiom Return |
| `.topics/refactor/security/001-2-refactor-anchor-to-docs-lane-secure-transport-v1-semantic-contra.trace.md` | Anchor → Anchor | superseded historical | B6 | Refactor Anchor → Docs lane: Secure Transport V1 semantic contract completion |
| `.topics/refactor/security/001-4-secure-transport-v1-docs-contract-anchor-return.trace.md` | Anchor → Anchor | completed/accepted terminal | B5 | Secure Transport V1 Docs contract → Anchor return |
| `.topics/refactor/security/001-5-1-2-axiom-to-anchor-secure-transport-v1-concrete-profile-review-retu.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Axiom → Anchor: Secure Transport V1 concrete profile review return |
| `.topics/role-lineage/001-1-2-axiom-to-anchor-role-continuity-and-repository-ownership-disposi.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Axiom to Anchor — Role Continuity And Repository Ownership Disposition |
| `.topics/handoff-package/handoffs/001-1-1-1-1-1-axiom-to-anchor-docs-major-007-minimal-carrier-material-recipient-semantics-return.trace.md` | Axiom → Anchor | completed/accepted terminal | B5 | Axiom To Anchor — Docs Major 007 Minimal Carrier And Recipient Semantics Return |

#### cli

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `test/fixtures/secure-transport-handoff.trace.md` | Anchor → Kodax | fixture/test-only | B8 | CLI secure transport fixture handoff |
| `.topics/refactor/security/handoffs/001-refactor-anchor-to-kodax-secure-transport-v1-cli-headless-proof.trace.md` | Anchor → Kodax | superseded historical | B6 | Refactor Anchor → Kodax: Secure Transport V1 CLI headless proof |
| `.topics/refactor/security/handoffs/002-secure-transport-v1-cli-headless-proof-kodax-return.trace.md` | Kodax → Anchor | completed/accepted terminal | B5 | Secure Transport V1 CLI headless proof — Kodax return |

#### extension-chrome

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `.topics/refactor/orchestration/experimental/001-1-1-1-anchor-to-kodax-chrome-experimental-dom-and-accessibility-reconnaissance-handoff.trace.md` | Anchor → Kodax | superseded historical | B6 | Anchor to Kodax — Chrome experimental DOM and accessibility reconnaissance |

#### provider-native

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `.topics/refactor/handoffs/001-anchor-to-anchor-provider-family-return.trace.md` | Anchor → Anchor | completed/accepted terminal | B5 | Return completed provider-native and provider-github source, exact technical qualification and a bounded Core/App reconciliation proposal to Anchor. |

#### app

| Path | From → To | Category | Basis | Title |
|---|---|---|---|---|
| `src/tooling/portable/fixtures/legacy-artifacts/handoff/tooling/001-v480-tooling-workflow-schema-enablement-handoff.trace.fixture.txt` | Architect → Tooling | fixture/test-only | B8 | v480 Tooling workflow schema enablement handoff |
| `src/tooling/portable/fixtures/legacy-artifacts/handoff/tooling/002-v481-tooling-recipient-relative-handoff-material-closure-planner-foundation-handoff.trace.fixture.txt` | Architect → Tooling | fixture/test-only | B8 | v481 Tooling recipient-relative Handoff material-closure planner foundation handoff |

#### interop-native

_No qualified Handoff leaves._

#### interop-openai

_No qualified Handoff leaves._

#### provider-github

_No qualified Handoff leaves._

#### runtime-native

_No qualified Handoff leaves._

#### verse-atlas

_No qualified Handoff leaves._

#### verse-native

_No qualified Handoff leaves._

## Loss And Uncertainty

- This is a current-frontier reduction, not a lifecycle rewrite. A leaf classified `superseded historical` remains a valid historical artifact and may still carry evidence, rationale, or source pointers.
- `completed/accepted terminal` means the bounded returned handoff is terminal for current navigation under the latest qualified Recovery; it does not manufacture release readiness, human acceptance, semantic closure, or destructive eligibility.
- The four Pilot visual returns are intentionally left unresolved because their own handoffs preserve accept/reject disposition and this pass found no qualified later current-Recovery evidence that resolves each individual candidate.
- The two Docs integrity mismatches are outside this leaf classification and remain unresolved/protected. No repair, semantic reinterpretation, or destructive candidate set is proposed here.
- Remote repository currentness was not checked. The carried complete Workspace snapshots and received Master Recovery are the bounded source of truth for this reduction event.
- No physical deletion, source-code implementation change, commit, push, release, publication, or remote mutation is claimed or authorized.

## Validation

- Tiinex orientation and grounding qualified the selected route, Required Context, 16 carried Workspace snapshots, declared Parent continuity to the semantic root, and the current Reduction Task.
- Holder Role binding was explicitly supplied as `Anchor`; grounding reached `grounded-to-act` before materialization or authoring.
- Each Workspace was materialized through Tiinex qualified workspace-byte providers; the received carrier remained untouched.
- Tiinex `project-handoff-leaves` per Workspace reproduced the Task baseline exactly: 113 `.topics` Handoff leaves. App contributed 2 fixture leaves and CLI 1 fixture leaf, producing 116 qualified Handoff-shaped leaves in the merged check.
- High-density real-leaf counts reproduced: Site 30, Business 28, Verse Playthings 24, Extension VS Code 12, Core 8, Docs 7; remaining real leaves are CLI 2, Extension Chrome 1, Provider Native 1.
- Tiinex `resolve-lineage` over Docs returned exactly two error-severity `lineage.parent.integrityMismatch` findings at the protected paths listed above; no attempt was made to hand-wave or repair them inside this Reduction.
- Classification is conservative: explicit latest-Recovery active/gate signals outrank older leaf wording; unresolved accept/reject evidence remains unresolved; filename chronology alone is never used as authority.
- Destructive-lineage eligibility was not invoked because no destructive candidate set is proposed. Ordinary Reduction and destructive eligibility remain separate contracts.

## Owner-Routed Follow-Ups

- **Anchor / Kodax / Sigma:** continue the active Extension VS Code Transport repair; preserve exact locked-toolchain and integrated Sigma acceptance gates.
- **Anchor / Sigma / Playthings specialist:** execute or disposition the current Site/Playthings browser/human gate, then explicitly accept/reject or supersede the four unresolved Pilot visual returns if they still matter to the current product surface.
- **Axiom (semantic) / Loom (mechanical only after semantic disposition):** inspect the two exact Docs parent-integrity mismatches before any terminal/stale or destructive interpretation of affected material.
- **Anchor:** preserve the independent fresh-successor grounding replay gate and the organization `.github` recovery gap until separately qualified.

## Navigation

- For fuller source, use the exact Workspace/path rows above against the carried complete Workspace snapshots from the received Handoff package.
- The received Handoff route and current Task remain the immediate control surface for this reduction pass; the latest Master Recovery remains the compact whole-program source of currentness.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-anchor-to-anchor-reduction-major-001-current-frontier-and-histor.trace.md](001-1-anchor-to-anchor-reduction-major-001-current-frontier-and-histor.trace.md)
  - Value: nVjmE55CK_2cn_k0TyUwgdY751A7GloblKHlt-UG1as

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: CHxFDBeBQo3AnBf_Ug9P2sxvTt0GHsqHWhqLQbAlYJY