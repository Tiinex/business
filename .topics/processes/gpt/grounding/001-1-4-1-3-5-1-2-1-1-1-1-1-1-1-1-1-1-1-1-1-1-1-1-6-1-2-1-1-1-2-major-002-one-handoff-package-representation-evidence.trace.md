# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 20:45:58
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 11:36:22
  - Authors: Anchor
  - Why: Lock the real representation defect and the exact numeric lineage/cache invariant before final implementation recovery.
  - Summary: Exact latest carrier/Core evidence shows route-count-dependent Package V1 vs artifact-first Phase 2 drift; Package V1 already provides the required numeric Workspace-cache-Role-Handoff Parent chain.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: What is the exact representation drift that must be removed before Major 002 can close, and what lineage/cache invariants does the already-existing Package V1 implementation prove are available without inventing a second recipient format?
- Evidence Role: Anchor architecture-recovery evidence over the exact latest carrier and carried Core source.
- Supported Conclusion: the latest carrier proves route-count-dependent representation drift. Single-route Package V1 already carries Workspace trace/ZIP, an optional Workspace-scoped cache trace/ZIP, then participant/endpoint/Handoff pointers through one numeric Parent chain. Multi-route manufacture instead switches to artifact-first Phase 2, which introduces route-token/hash filenames plus `e`/`p` pseudo-dimensions. The repair target is therefore convergence onto one Package V1-style recipient surface, not further evolution of Phase 2 as a second standard.

## Provenance

- Known Source: exact latest-known carrier `vscode-001-2-3-1-1-1-sigma-to-anchor.handoff-package.zip` supplied by Sigma and treated as the sole current frontier for this recovery branch.
- Carrier Observation: Start identifies `artifact-first-clean-carrier-phase2`, two qualified routes, route-path/hash Handoff pointer naming, and `e`/`p` Role-pointer dimensions.
- Core Source Basis: exact Core Workspace carried by that package.
- Preservation Basis: bounded read-only inspection of the exact carrier and carried Core source; no source mutation, remote mutation, package rewrite, or semantic schema change was performed to derive this Evidence.
- Provenance Limits: this Evidence identifies current implementation behavior and the target invariant; it does not itself prove the final multi-route numeric branching algorithm until Loom returns the implementation and regression evidence.

## Evidence Material

- Material: exact latest carrier Start surface plus carried Core Package V1 and artifact-first Phase 2 builders.
- Material Kind: recipient-facing package observation and exact implementation-source inspection.

### Existing Package V1 already contains the desired lineage model

- `recipientV2.packageV1.build.js` emits each direct complete Workspace as one `.workspace.md` artifact and one `.workspace.zip` payload sharing the same numeric prefix.
- When detached material is required for that Workspace, Package V1 emits a Workspace dependency cache artifact and cache ZIP at the same next numeric dimension, currently `<workspace-prefix>-1-cache.trace.md` and `<workspace-prefix>-1-cache.zip`.
- The cache artifact declares the Workspace artifact as Parent and becomes the Parent authority for subsequent route-grounding pointers.
- Package V1 starts the pointer lineage at `<cache-dimension>-1` when a cache exists, otherwise directly below the Workspace.
- Participant Role pointers are created first; each pointer becomes the Parent of the next numeric dimension.
- Endpoint requirements are deterministically ordered From then To; each endpoint pointer likewise becomes the Parent of the next numeric dimension.
- The Handoff pointer is emitted at the final next numeric dimension and declares the final Role pointer, or cache/Workspace when Roles are absent, as its Parent.
- This matches the required lineage class: Workspace -> optional cache/material -> participant(s) -> From -> To -> Handoff, using numeric Parent dimensions only.

### Artifact-first Phase 2 is a divergent recipient representation

- The latest carrier Start declares `artifact-first-clean-carrier-phase2` because more than one route is present.
- Phase 2 emits separate route tokens derived from workspace/path data and hash material for sibling routes.
- Phase 2 emits endpoint Role pointers under `e` pseudo-dimensions and participant Role pointers under `p` pseudo-dimensions.
- This makes endpoint/participant classification part of the filename dimension instead of preserving filename dimension as Parent lineage.
- Route cardinality therefore changes the recipient-facing representation even though Handoff semantics do not change.

### Cache/material boundary

- The cache is transport/material carriage only. It must not become recipient semantic authority or a second index/manifest.
- The cache trace and cache ZIP share one numeric lineage dimension exactly as Workspace trace and Workspace ZIP do.
- Cache internals should preserve adapter-resolvable material identity using qualified workspace-relative/permalink-derived paths where available; opaque `.bin` leaves are not acceptable when exact source path/media identity is already known.
- Participant/endpoint/Handoff pointers resolve into the Workspace or cache through normal shared adapter/material-resolution mechanics. They must not invent route-token prefixes, recipient namespaces, or host-private lookup semantics.

## Locked Acceptance Surface

For one route with one participant, the normative structural example is:

`001-5-1` Workspace trace
`001-5-1` Workspace ZIP
`001-5-1-1` cache/material trace
`001-5-1-1` cache/material ZIP
`001-5-1-1-1` participant Role pointer
`001-5-1-1-1-1` From Role pointer
`001-5-1-1-1-1-1` To Role pointer
`001-5-1-1-1-1-1-1` Handoff pointer

If participant material is absent, no empty participant dimension is invented; the chain compresses naturally from cache/Workspace to From -> To -> Handoff.
For multiple participants, each participant advances the same numeric Parent chain.
For multiple Handoff routes, each route must remain a numeric descendant branch of the same qualified Workspace/cache ancestor; route branching may use numeric sibling ordinals only. No letters, hashes, source-path slugs, or alternate recipient format may become filename dimensions.


## Preservation And Fidelity

- Preservation State: the latest carrier, its carried Business/Core/VS Code Workspace bytes, and all observed Sigma media remain unchanged; this Evidence is a read-only architecture finding.
- Fidelity Notes: the numeric lineage example is taken from the already-existing Package V1 construction model and the user-confirmed acceptance invariant; it is not inferred from filename aesthetics alone.
- Known Losses: the final numeric sibling branching scheme for more than one route under the same Workspace/cache remains implementation work for Loom, bounded by the no-letter/no-hash/Parent-consistency invariants above.

## Interpretation Limits

- Does Not Prove: that every current Phase 2 helper must be deleted; JSON-free byte verification, closure, cache materialization, and exact route projection mechanics may be reused behind the single Package V1 recipient surface.
- Not Yet Used As: final implementation acceptance, Sigma acceptance, Major closure, release approval, or remote mutation authority.
- Must Not Be Treated As: permission to preserve Package V1 and Phase 2 as two normal recipient-facing standards.
- Must Not Be Used To Claim: cache or pointer artifacts create Handoff/Role semantics; authoritative semantics remain in the referenced artifacts and Parent lineage.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md)
  - Value: Ebr-Lo3KdDKoEI-6ReFR7bO19XoV_SD1UhqGTKehMZk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: zzBRkzdAmQ4FBGQSIB6OO5KSbZaYi1tW4ydmjEeAnUs