# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Viewer](001-3-viewer-project.trace.md)
  - Origin:
    - [relative](001-3-viewer-project.trace.md)
- Current
  - Current Schema: [tiinex.discovery.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/discovery/tiinex.discovery.v1.schema.md)
  - Created At: 2026-08-30 16:12:00
  - Authors: Anchor; Sigma
  - Why: Reconcile the Viewer that actually exists now before turning Atlas or PoC recovery into implementation work, while preserving the product need for several complementary human-readable projections.
  - Summary: Viewer present-state and Atlas readiness discovery separating current source, PoC parity evidence, public qualification, human feedback, and the smallest realistic path toward Feed, Tree, Lineage, and Atlas as complementary views.
  - Status: draft/local

---

# Viewer Present State And Atlas Readiness

## Discovery Intent

- Intent: establish a trustworthy present-state read of Tiinex Viewer before decomposing new Site and Tooling development, and determine where Atlas belongs without treating an intended spatial graph as already implemented or semantically authoritative.
- Starting Question: what is genuinely present, partially recovered, unqualified, or still only product direction in the current Viewer, and what is the smallest development sequence that can recover confidence before Atlas becomes implementation work?

## Discovery Field

- Field: Tiinex Viewer current-state across the Site `refactor` source, its PoC parity ledger and public validation state, the existing Business Viewer outcomes, and current human product feedback.
- In Scope: Feed/discovery projection, Tree/path projection, Lineage/Parent projection, PoC parity status, current Viewer validation/release boundary, typed non-Parent relation support relevant to spatial reading, Atlas as a named intended spatial projection, mobile-first comprehension, and readiness for later technical Task decomposition in the natural implementation repositories.
- Out Of Scope: fixing the current Site pipeline blocker; declaring the whole PoC port complete; implementing Atlas; selecting Leaflet or another rendering library as permanent architecture; introducing coordinate semantics; relation authoring; broad Viewer feature expansion; or creating Site/Tooling implementation Tasks before their current seams and acceptance boundaries are understood.
- Freshness Boundary: current-source observations were checked on 2026-08-30 against Site `refactor` commit `ba59d72c0ad0015170838b4ce906b538da4f78f8` (`tiinex-site` `0.2.289-v470`) and its latest visible `refactor` publish run `33214378230` from 2026-08-28.

## Discovery Method

- Method: read the current Site source and its own parity ledger first; distinguish source presence from qualified behavior; compare those facts with the human-observed PoC baseline and current product feedback; then derive only the minimum development ordering needed to make later Atlas work truthful and testable.
- Evidence Approach: classify observations as **current source**, **current self-declared parity state**, **public qualification state**, **human-observed PoC evidence**, or **human feedback/product direction**. The existence of a test, module, label, or historical interaction is not by itself treated as proof that the current refactor is qualified or product-complete.

## Discovery Boundaries

- Current Truth Boundary: the Site refactor contains substantial Viewer/runtime work, but its latest visible publish run fails during `Validate source` before the broad test, build, and deploy stages. Present source therefore must not be described as currently qualified merely because supporting tests and modules exist.
- PoC Boundary: the earlier PoC remains useful product evidence for Feed/Tree/Lineage separation, progressive disclosure, creation, Time Portal, and human navigation patterns. It is not proof that those behaviors are fully ported or passing at the current refactor commit.
- Atlas Boundary: Atlas means the intended spatial artifact-and-relation projection. Automatic layout, pan/zoom, and user-moved visual positions are presentation state only. Coordinates, proximity, direction, and manual node placement must not become Parent, Relation, provenance, priority, or other semantic authority.
- Rendering Boundary: Leaflet remains a plausible tileless rendering candidate because the intended interaction is spatial pan/zoom rather than geographic truth, but the current Site package has no Leaflet dependency and this Discovery does not make one library part of Tiinex semantics or architecture.
- Relation Boundary: Parent remains direct continuity ancestry. Atlas must keep typed non-Parent relations distinguishable rather than flattening them into Parent or inferring relation meaning from visual position.
- Development Boundary: this Discovery can justify later technical Tasks, but it does not authorize implementation or silently thaw unrelated feature work.
- Human/Tooling Parity Boundary: human-first presentation may be richer, more spatial, or easier to scan, but it must not create privileged semantic access. A Viewer capability fails readiness if a human can inspect, infer, validate, or perform a semantic operation that the qualified Tooling/LLM path cannot inspect, validate, and reproduce from the same authoritative artifacts, or vice versa. Presentation state may differ; semantic inputs, edges, boundaries, and results must remain equivalent.
- Testing Boundary: Viewer capability should not reach the normal product surface merely to make Sigma manually discover basic semantic defects. Machine-verifiable behavior needs corresponding Tooling support and deterministic tests first; human acceptance should primarily test comprehension, usability, real-path fit, and judgments that automation cannot supply.

## Discovery Outcome

- Outcome: completed discovery with a staged readiness result. Viewer work is developed enough to support concrete recovery and qualification Tasks now, but Atlas should enter implementation only after the current Viewer seams are qualified enough that new spatial presentation is not built on uncertain parity.
- Current Source: Feed/discovery has explicit leaf filtering and sorting behavior; Tree has a path-tree projection; Lineage has a loaded-workspace resolver/traversal and a projection over declared Parent edges; view state explicitly carries at least Feed and Tree verse selection. These are real current source surfaces, not only historical PoC concepts.
- Current Self-Declared Parity: the v470 PoC parity ledger still marks many relevant scenarios `partial`, including path-tree material lineage, loaded-lineage resolution, declared-lineage tree, discovery presentation parity, artifact creation contracts, Time Portal, publication/re-ingest, and several persistence/source boundaries. The ledger explicitly requires manual/browser evidence for several of these before parity is claimed. The current PoC inventory is known to be incomplete: a behavior missing from the ledger or this Discovery is not evidence that it has parity, was intentionally removed, or is no longer required.
- Current Public Qualification: the latest visible `refactor` publish run reaches dependency installation and then fails at `Validate source`; later smoke, typecheck, runtime, build, public-output, and deploy steps are skipped. This means the current refactor does not presently provide one green public qualification result for the Viewer surfaces inspected here.
- Current Lineage/Relation Seam: the inspected workspace Lineage projection is centered on resolved Parent/Trace edges and associated missing/mismatch diagnostics. The parity ledger records one bounded old-Reference behavior as a durable typed non-Parent Relation, while broader Reference relation parity remains partial. A generic Viewer graph projection that exposes Parent and typed Relation edges side by side is therefore still a needed seam before Atlas can truthfully visualize both.
- Atlas Present State: Atlas is product direction, not a recovered current surface. No Leaflet dependency is present in the current package and no current Atlas surface was located in the inspected refactor material. It should be planned as a new projection over qualified artifact graph semantics, not described as unfinished PoC parity unless later evidence shows otherwise.
- Human Product Signal: current feedback supplied to Sigma indicates Feed is useful for ongoing Tiinex work but not simple enough as the only introductory view. This is evidence for complementary first-contact projections, not evidence that Feed should be removed or that one spatial view will suit every reader.
- Product Direction: retain Feed, Tree, and Lineage as distinct views and add Atlas as the named spatial overview when ready. Each view should answer a different human question while opening the same artifacts and respecting the same semantic authority.
- Realistic Development Sequence: **(0) Loom iteration-efficiency gate** — treat Tooling development-loop cost as priority 1 and establish focused/restartable validation before broader support work expands the test/checkpoint burden; **(1) bootstrap role understanding** — recover Tooling/LLM-readable role semantics, including shared/base-role inheritance or specialization, without relying on chat memory; **(2) Viewer current/release baseline** — resolve which Site state is intended to be qualified and establish a focused, repeatable path that can actually evaluate the relevant Viewer surfaces; **(3) PoC parity disposition** — progressively classify human-important PoC loops as recovered, partial, intentionally changed, unknown, or still requiring proof without assuming the inventory is complete; **(4) shared graph read model** — expose viewer-neutral nodes plus explicitly distinct Parent and typed Relation edges, preserving unresolved edges without guessing and without coordinates, with equivalent Tooling/LLM inspection and validation; **(5) Atlas read-only slice** — automatic layout, pan/zoom, mobile navigation, clear node type/name, visually distinct Parent versus Relation edges, and open/focus into the same artifact used by the other views; **(6) human + LLM acceptance** — verify semantic parity through Tooling first and then compare whether humans can understand the intended question without deep reading; **(7) authoring later** — only after graph reading is trusted, explore explicit relation creation and maintenance without making drag position semantic.
- Task Readiness: technical subtasks may now be decomposed, but Loom should begin with **Tooling iteration efficiency** before taking on broader Tooling/Viewer support. Bootstrap role understanding and the Viewer current/release baseline are then concrete near-term gaps; PoC parity disposition remains progressive because the inventory is incomplete. The shared graph-read-model seam may be designed in parallel once the Tooling contract can be exercised cheaply enough. Atlas-specific implementation Tasks should wait until corresponding Tooling projection/validation and the relevant current Viewer seams are qualified; Atlas does not need to wait for every unrelated Site feature to be complete.
- Next Artifacts: create Site/Tooling-local development Tasks only when the owning implementation seam is clear; preserve this Business Discovery as the manager-readable reason and acceptance direction rather than duplicating technical implementation detail here.

## References

- Site refactor inspected: https://github.com/Tiinex/site/tree/ba59d72c0ad0015170838b4ce906b538da4f78f8
- Current Site package: https://github.com/Tiinex/site/blob/ba59d72c0ad0015170838b4ce906b538da4f78f8/package.json
- Current PoC parity ledger: https://github.com/Tiinex/site/blob/ba59d72c0ad0015170838b4ce906b538da4f78f8/src/parity/poc.parityLedger.js
- Current workspace Lineage projection: https://github.com/Tiinex/site/blob/ba59d72c0ad0015170838b4ce906b538da4f78f8/src/workspaces/workspace.lineageView.js
- Latest visible refactor publish run: https://github.com/Tiinex/site/actions/runs/33214378230

## Interpretation Limits

- Limits: this Discovery does not prove current Viewer parity, provide a complete inventory of missing PoC behavior, fix or diagnose every cause behind the failing Site validation chain, prove that Leaflet is the correct implementation library, prove that Atlas will solve first-contact comprehension, establish a universal usability consensus, settle the exact canonical representation of role inheritance/specialization, authorize coordinate semantics, or establish relation authoring behavior. It establishes a bounded present-state and development ordering that should be rechecked as Tooling efficiency, bootstrap role resolution, Site refactor, qualification state, and PoC recovery knowledge change.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Viewer](001-3-viewer-project.trace.md)
  - Value: Z9OpOKoRrUw36W8_jOf7E3_-Ec36pqymqyIHKtYWIYc

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: N-kZqyfcah-tSE7SnZaSrSSsVp9lfirqBoXMtfmLUuo
