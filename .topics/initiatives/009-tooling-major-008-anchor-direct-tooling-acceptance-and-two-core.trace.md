# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 21:35:57
  - Trace: [034-anchor-to-anchor-tooling-major-008-canonical-build-parity-contin.trace.md](handoffs/034-anchor-to-anchor-tooling-major-008-canonical-build-parity-contin.trace.md)
  - Origin:
    - [relative](handoffs/034-anchor-to-anchor-tooling-major-008-canonical-build-parity-contin.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 21:55:35
  - Authors: Anchor
  - Why: Sigma must not be the first observer of shared Core/Tooling defects, and Major 008 requires VS Code capabilities to exist first in shared Tooling.
  - Summary: Direct Tooling proves durable authoring, bounded Role cache and exact numeric Package V1 lineage, while isolating real Role discovery source-authority failure and absolute-host-path leakage inside endpoint cache entries.
  - Status: ready/local

---

# Tooling Major 008 — Anchor Direct Tooling Acceptance And Two Core Blockers

## Supported Claim Or Question

- Supported Claim Or Question: Can the exact shared Core/Tooling frontier perform the Handoff capabilities expected by VS Code without host-private semantics, and what still blocks Sigma?
- Evidence Role: direct Anchor acceptance over the exact carried Major 008 Business/Core/VS Code frontier before real-host promotion.

## Provenance

- Known Source: exact Workspaces carried by the qualified Anchor-to-Anchor Major 008 continuation package, cold-grounded through its carried bootstrap and then exercised through the exact carried Core Tooling entrypoint.
- Preservation Basis: all generated Handoff/package material was disposable; carried product source was read-only.
- Provenance Limits: canonical VS Code emitted-runtime parity remains independently open; this Evidence does not claim Extension Host or Sigma acceptance.

## Evidence Material

- Material Kind: direct shared Core/Tooling operator-flow execution, package manufacture/orientation, exact Role qualification diagnostics, and cache-path inspection.
- Material: current Major 008 carried Business/Core/VS Code Workspaces; disposable authored Handoff; explicit endpoint/participant material bindings; produced Package V1 and its qualified orient/roundtrip receipts.

### Direct Tooling Acceptance Results

### PASS — native durable Handoff authoring

- `inspect-creation-contract tiinex.handoff.v1` exposes optional `From Reference` and `To Reference` inputs.
- `create-local-draft` successfully authored a valid Handoff with durable qualified Sigma and Anchor Role references.
- The authored Handoff passed integrity qualification without VS Code-private endpoint state.

### PASS — explicit participant and bounded external material closure

- Manufacture was exercised with only the `vscode` Workspace selected for carriage.
- Sigma and Anchor endpoint Roles plus an explicitly selected Loom participant Role were sourced from the separate open `business` Workspace through exact material bindings.
- Core manufactured a ready Package V1 with the external Role material bounded into cache rather than adding the Business Workspace to Outgoing.
- Package inspection and manufacture roundtrip were valid.

### PASS — exact numeric lineage required by Major 008

The produced package projected this actual lineage:

- Workspace: `001-3` trace + ZIP
- Cache: `001-3-1` trace + ZIP
- Participant Role pointer: `001-3-1-1-loom-role-pointer.trace.md`
- From Role pointer: `001-3-1-1-1-from-sigma-endpoint-role-pointer.trace.md`
- To Role pointer: `001-3-1-1-1-1-to-anchor-endpoint-role-pointer.trace.md`
- Handoff pointer: `001-3-1-1-1-1-1-handoff-pointer.trace.md`

This proves the shared Package V1 path can produce Workspace -> cache -> participant -> From -> To -> Handoff as one numeric Parent chain with no `e`/`p` pseudo-dimensions.

## Blocker 1 — real qualified Role discovery returns zero candidates

- Direct `project-handoff-endpoints <business-root> --workspace-id business` returns `status: ready` but `candidates: []` against the actual current Business Workspace.
- `project-operator-context` over all three explicit Workspace roots likewise exposes real Workspaces/Handoff leaves but returns no endpoint or participant Role candidates.
- Direct `inspect` of the same canonical Role artifact succeeds and reports exact qualified schema/integrity.
- The stricter runtime validation authority used by Role projection rejects `tiinex.party.role.v1` because compiled lineage source authority substitutes a historic `tiinex.party.v1` source commit for the current same-snapshot relative Parent.
- Observed contradiction:
  - current compiled/bootstrap schema snapshot: Tiinex/docs `3988951208eb9a8926e84ab42625d4b42fa00c2d`;
  - substituted historic parent source: Tiinex/docs `2a40646640f7468bcd250df6988b69e9f047f1bb`;
  - result: `compiled-validation-lineage-source-authority-unqualified`.
- This means normal Core-backed VS Code Role dropdown discovery would still be empty against real current Role artifacts even though synthetic projection tests pass.

### Required correction boundary

Correct Core schema-lineage source resolution so the canonical real Role artifacts qualify under exact current schema authority. Do not weaken Role qualification, bypass runtime authority in VS Code, recursively scan repositories, or edit Docs semantics unless a genuine unresolved semantic contradiction is proven and explicitly escalated.

## Blocker 2 — endpoint cache paths leak host filesystem paths

- In the same valid Package V1, the explicitly selected Loom participant cache entry is clean and Workspace-relative:
  - `material/3-business/.topics/roles/001-3-1-loom-canonical-holder-cutover-role.trace.md`
- Sigma/Anchor endpoint Role cache entries incorrectly include the disposable absolute host path, for example:
  - `material/1-business/mnt/data/major008_tooling_gate/business/.topics/roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md`
- The endpoint pointers still resolve, but the cache internal tree violates the Major 008 clean adapter-based cache invariant and leaks execution-host source layout into recipient material.

### Required correction boundary

Cache internal identity/path must derive from qualified Workspace/provenance/artifact target identity. Material-binding `sourcePath` is execution-only byte location and must never become recipient-facing cache path identity. Preserve current Package V1 representation and numeric lineage.

## Regression Expectations

- Add integration coverage using the actual current canonical Role artifact shape/source-authority pattern, not only synthetic Role fixtures.
- Add mixed endpoint + explicit participant external-cache coverage proving all cache entries use clean Workspace-relative qualified paths.
- Preserve durable endpoint authoring, explicit 0..N participant selection inputs, carried-vs-cache material behavior, Required Context cache closure, single/multi Package V1, and all Major 008 MUST NOT invariants.
- Canonical VS Code emitted-runtime parity remains a separate open gate after these shared-Core blockers are reconciled.

## Preservation And Fidelity

- Preservation State: carried Business/Core/VS Code product bytes remained read-only during the direct acceptance run; all authored Handoff/package probes were disposable and are not promoted as canonical product state.
- Fidelity Notes: Role discovery failure was reproduced against the real current canonical Role artifacts, while package/cache findings were read from the actual Package V1 produced by exact carried Core Tooling.
- Known Losses: canonical VS Code emitted-runtime parity, real Extension Host behavior, and Sigma acceptance remain outside this Evidence.

## Interpretation Limits

- Does Not Prove: real VS Code UI acceptance, canonical emitted-runtime parity, reload/re-attach UI behavior, or Major 008 closure.
- Must Not Be Treated As: authority for a new package format, recipient/meta JSON, host-private Role authority, generalized qualification weakening, or cache index metadata.
- Not Yet Used As: Sigma promotion.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [034-anchor-to-anchor-tooling-major-008-canonical-build-parity-contin.trace.md](handoffs/034-anchor-to-anchor-tooling-major-008-canonical-build-parity-contin.trace.md)
  - Value: PfeTM8V8JorQIyQncRfW6ERVucekmBHlIOtiVg7GHvI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: QPlHhjvSdQhjHmXPDRRRgBxx1dfAUfSKRTcEmU7e4xo