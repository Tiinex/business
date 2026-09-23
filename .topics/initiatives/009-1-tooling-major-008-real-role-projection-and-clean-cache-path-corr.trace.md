# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 21:55:35
  - Trace: [009-tooling-major-008-anchor-direct-tooling-acceptance-and-two-core.trace.md](009-tooling-major-008-anchor-direct-tooling-acceptance-and-two-core.trace.md)
  - Origin:
    - [relative](009-tooling-major-008-anchor-direct-tooling-acceptance-and-two-core.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 21:56:04
  - Authors: Anchor
  - Why: Direct Tooling acceptance proved these two Core defects would otherwise reach VS Code/Sigma even though synthetic Major 008 tests were green.
  - Summary: Correct shared Core Role projection against real canonical Role artifacts and remove absolute host-path leakage from endpoint cache entries while preserving Package V1.
  - Status: ready/local

---

# Tooling Major 008 — Real Role Projection And Clean Cache Path Correction

## Objective

Close the two shared Core/Tooling blockers found by Anchor's direct Major 008 Tooling acceptance, without changing Package V1 representation or moving semantic responsibility into VS Code.

The shared path must first qualify the actual current canonical Role artifacts from explicit Workspace roots, and then manufacture external endpoint/participant Role material into a clean Workspace-relative cache tree whose recipient-facing identity never depends on host filesystem paths.

## Done Criteria

- `project-handoff-endpoints` against the actual current qualified Business Workspace returns the canonical Role/Identity candidates expected from that Workspace instead of an empty candidate set.
- `project-operator-context` over explicit open Workspace roots exposes those same qualified candidates without repository-wide recursive discovery or host-private inference.
- Resolve the current `tiinex.party.role.v1 -> tiinex.party.v1` runtime validation source-authority contradiction correctly:
  - preserve exact schema/lineage authority;
  - do not weaken Role qualification generically;
  - do not special-case VS Code;
  - prefer the canonical same-snapshot relative Parent authority where that is what the existing schema contract establishes;
  - if Core cannot determine the intended authority without changing canonical semantics, stop and return a precise Axiom blocker rather than editing Docs or guessing.
- Add regression coverage using the actual current canonical Role artifact/source-authority shape, not only synthetic Role fixtures.
- External endpoint Role material and explicit participant Role material both use recipient cache paths derived from qualified Workspace/provenance/artifact identity.
- Absolute/local `sourcePath` is treated only as the execution-time byte locator and never appears in a recipient-facing cache entry path.
- Mixed external-cache package coverage proves clean paths for at least:
  - one participant Role;
  - From Role;
  - To Role.
- The positive mixed-cache package retains the exact numeric lineage already accepted by Major 008: Workspace -> cache -> participant(s) -> From -> To -> Handoff.
- Carried-Workspace material remains direct and is not needlessly duplicated into cache.
- Existing external Required Context cache closure remains green.
- Existing durable optional `From Reference` / `To Reference` authoring remains green.
- Existing explicit 0..N participant selection semantics remain green.
- Single and multi Handoff manufacture remain on the same Package V1 path.
- No recipient/meta JSON, cache index, `e`/`p` pseudo-dimensions, source-path/hash filename dimensions, or second recipient representation is introduced.
- Return one qualified Loom-to-Anchor Handoff carrying exact Core changes and bounded Evidence.

## Scope

- Loom / Core only.
- Role/Identity projection authority and schema-lineage source resolution used by shared Tooling.
- Cache internal path canonicalization for material bindings/requirements.
- Focused Core integration/regression tests for the exact two blockers.

## Dependencies

- [Tooling Major 008](001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
- [Anchor Direct Tooling Acceptance And Two Core Blockers](009-tooling-major-008-anchor-direct-tooling-acceptance-and-two-core.trace.md)
- Exact current Core Workspace carried with the Loom Handoff.
- Exact current Business canonical Role artifacts carried for realistic projection tests.

## Exclusions

- Do not change VS Code source or emitted runtime.
- Do not close or bypass the still-open canonical VS Code emitted-runtime parity Task.
- Do not redesign Package V1 or its numeric pointer lineage.
- Do not add recipient/meta JSON or cache manifest/index authority.
- Do not relax Role qualification to make discovery pass.
- Do not recursively scan repository Roles as a substitute for explicit Workspace-root projection.
- Do not edit canonical Docs semantics unless a genuine contradiction is proven and escalated through Axiom.
- Do not perform remote commit, push, publish, release, deployment, or registry mutation.

## Completion Boundary

Completion means the exact shared Core/Tooling flow can discover the real current Roles and manufacture clean external endpoint/participant cache material while preserving the accepted Package V1 lineage. It does not complete canonical VS Code build parity, real-host Sigma acceptance, or Major 008 itself.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [009-tooling-major-008-anchor-direct-tooling-acceptance-and-two-core.trace.md](009-tooling-major-008-anchor-direct-tooling-acceptance-and-two-core.trace.md)
  - Value: QPlHhjvSdQhjHmXPDRRRgBxx1dfAUfSKRTcEmU7e4xo

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: XzQTGVPOvWPyZh_O9dR4wtmPh_pnwbCaIktjpLvheqI