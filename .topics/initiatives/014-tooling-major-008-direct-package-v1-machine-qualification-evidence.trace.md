# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-24 00:21:20
  - Trace: [042-anchor-to-anchor-direct-package-v1-implementation-checkpoint.trace.md](handoffs/042-anchor-to-anchor-direct-package-v1-implementation-checkpoint.trace.md)
  - Origin:
    - [relative](handoffs/042-anchor-to-anchor-direct-package-v1-implementation-checkpoint.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-24 02:37:00
  - Authors: Anchor
  - Why: Preserve the exact machine qualification reached after the direct Package V1 implementation was completed beyond the prior checkpoint, including readable adapter-native cache, generic grounding pointers, ZIP-only continuation, hermetic embedded-Tooling execution and anti-drift protection.
  - Summary: Gates 1 through 4 of Task 013 are machine-qualified and the final hermetic package works from an empty host using only its embedded bootstrap; final canonical permalink binding, fresh-LLM behavioral acceptance and Sigma acceptance remain open.
  - Status: ready/local

---

# Tooling Major 008 — Direct Package V1 Machine Qualification Evidence

## Supported Claim Or Question

- Supported Claim Or Question: does the current Core implementation directly manufacture, serialize, inspect, orient, ground and continue Package V1 without Handoff Package V2 machinery, while preserving readable Workspace/cache/pointer semantics and failing closed against the agreed drift classes?
- Evidence Role: Anchor machine qualification for Task 013 Gates 1 through 4 plus the pre-fresh-LLM hermetic host challenge.
- Supported Conclusion: yes for machine qualification. Core validation passes 222/222 repository tests plus portable/bootstrap qualification; the focused Package V1/recovery/anti-drift suite passes 17/17; an active-source scan excluding the anti-regression test itself finds zero recipientV2, recipient-v2, archiveV2, handoff-v2, handoff.material, material.bin or rebuild-required implementation traces; and a physical multi-route/cache Package V1 boots and reaches grounded-to-act from an empty directory using only its carried bootstrap and untouched package bytes.

## Provenance

- Controlling Task: [Task 013](business::.topics/initiatives/013-tooling-major-008-handoff-package-v2-purge-and-native-v1-rebuild.trace.md).
- Prior Checkpoint: [Handoff 042](business::.topics/initiatives/handoffs/042-anchor-to-anchor-direct-package-v1-implementation-checkpoint.trace.md).
- Core Workspace: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md).
- Canonical Docs Workspace: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md).
- Business Workspace: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md).
- Evidence Boundary: exact current local Workspace bytes and machine receipts only. No GitHub mutation, no VS Code implementation and no claim of fresh-LLM or Sigma acceptance.

## Evidence Material

- Core Validation: `npm run validate` passes 222/222 Node tests, portable smoke qualification and embedded bootstrap qualification.
- Focused Package Qualification: direct Package V1, manual/read-only recovery and retired-V2 anti-drift tests pass 17/17.
- Active V2 Sweep: zero active implementation hits for retired Handoff Package V2 identifiers/paths after excluding historical `.topics` provenance and the intentional anti-regression forbidden-string test.
- Direct V1 Path: normalized Core manufacture input -> Package V1 allocation/materialization -> Package V1 inspection -> deterministic physical ZIP. No V2 builder, upgrader, verifier or writer participates.
- Workspace Carriage: Workspace ZIP payloads are repo-root snapshots and exact inner Workspace artifact bytes are rebound during inspection.
- Cache Carriage: bounded cache entries retain readable adapter-native paths such as `github/Tiinex/business/.topics/...`; no generic `material/`, `.bin` indirection or hidden JSON mapping truth is used.
- Grounding Pointers: Process, Policy, endpoint Role, participant Role and Handoff pointer projections use the same exact target resolution machinery while semantic authority remains with the referenced Handoff/context/Role artifacts.
- Participant Reference Preservation: an external participant may preserve an adapter-native GitHub permalink while Workspace id/path remain separate resolution identity; Tooling does not rewrite the permalink into a Package-private pseudo-reference.
- Anti-Drift: pointer digest mutation, cache over-expansion, sibling-route pointer borrowing with recomputed integrity, carried-material cache duplication and retired V2 machinery are rejected by permanent tests.
- Physical ZIP Continuation: a ZIP-only test loads one serialized Package V1, orients it, grounds the selected route to grounded-to-act and materializes its carried Workspace into an empty output directory with runtime-only continuation state.
- Hermetic Host Challenge: a clean directory containing only the multi-route/cache package extracted only its declared bootstrap, ran the embedded Tooling without Core checkout/npm/internet, oriented two routes, grounded the selected route to grounded-to-act with qualified continuity and materialized the selected Work Workspace.

## Acceptance Candidates

- Simple Candidate A: `A-simple-single-route.package-v1.zip`; SHA-256 `7e72414b4657677c49b8945b04b6ac930868cf9cba130930da87ce12b8656c7b`; one route, no cache.
- Hermetic Candidate B: `B-hermetic-multi-route-cache.package-v1.zip`; SHA-256 `683359f5dd5fd133148146279cee7300ae6d5fb558c7a50276efa75b51553be7`; two routes, one bounded cache.
- Candidate B Cache: exactly five readable GitHub-native entries — Process, Policy, Anchor Role, Loom Role and Sigma Role under `github/Tiinex/business/.topics/...`.
- Candidate B Grounding: recipient Sigma Role resolves from cache; Anchor endpoint Role, Loom grounding Role, Process and Policy resolve from cache; Tooling correctly keeps Role grounding separate from semantic participant inference.
- Candidate Status: pre-commit machine candidates only. They are not final canonical acceptance packages because the changed Package V1 bounded-cache schema has not yet been committed to a new exact Docs permalink.

## Preservation And Fidelity

- Preservation State: exact Core direct-V1 implementation, one canonical Docs bounded-cache correction and Business Task/continuity are preserved as the current three-Workspace frontier.
- Fidelity Notes: `sha256-base64url-c14n-v2` remains the trace-integrity method and is explicitly protected by the V2 purge regression test; only Handoff Package V2 machinery is retired.
- Known Losses: none established in direct Package V1 machine behavior. Final immutable Docs schema identity is unavailable until the changed Docs Workspace is committed/pushed.

## Interpretation Limits

- Not Yet Used As: fresh-LLM behavioral acceptance, Sigma Package V1 acceptance, Core freeze, VS Code thaw or release authority.
- Does Not Prove: that a fresh LLM with no prior conversation will follow Start/bootstrap/grounding correctly without improvisation; that Sigma accepts the human-facing ZIPs; or that the old exact Docs commit contains the new bounded-cache contract.
- Must Not Be Treated As: authority to change VS Code during Uppdrag 1, reintroduce Handoff Package V2 compatibility, mutate GitHub from Anchor, or substitute a mutable/non-exact schema reference for the required final permalink.
- Disposition: package and commit/push the exact Core/Docs/Business frontier, observe the new exact Docs commit read-only, bind Core Package V1 schema references to it, rerun the same machine gates, then conduct fresh-LLM acceptance before Sigma review.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [042-anchor-to-anchor-direct-package-v1-implementation-checkpoint.trace.md](handoffs/042-anchor-to-anchor-direct-package-v1-implementation-checkpoint.trace.md)
  - Value: iDm7kL_c17Xb4WH7vyhbceLcnvbLg9-FDPEbxZTksqs

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:MvcHbBtPTE-TJI3JXurnFq9B1FYSWpFcp8PuiAmUqkU
