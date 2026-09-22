# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 20:45:58
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 11:37:49
  - Authors: Anchor
  - Why: The latest carrier proves the remaining blocker is representation convergence plus host Role/Workspace discovery, not a need for another package standard.
  - Summary: Finish one Package V1-style single/multi carrier, numeric Workspace-cache-pointer lineage, adapter-resolvable cache material, and VS Code shared-Core consumption.
  - Status: ready/local

---

# Major 002 — Final Handoff Package Convergence And VS Code Shared-Core Completion

## Objective

Finish the Handoff packaging capability originally targeted by Major 002: one clean recipient-facing Handoff Package representation for single and multi Handoffs, numeric artifact/filename Parent lineage, adapter-resolvable Workspace/cache/Role material, and VS Code that consumes the shared Core implementation without a duplicated semantic/package layer.

## Scope

Parallel bounded recovery across Core package manufacture/inspection/grounding and VS Code host discovery/controller integration required to converge the existing Handoff packaging implementation. No unrelated refactor is in scope.

## Done Criteria

### One package representation

- Normal manufacture uses one recipient-facing Handoff Package representation for both one and many Handoff routes.
- Route count never selects a second normal package format.
- Artifact-first Phase 2 may survive only as internal reusable mechanics or explicit non-production specimen coverage; it cannot be reachable as an alternate normal recipient surface.
- `tiinex-recipient-v2.transport.json` and any equivalent durable compatibility/meta manifest remain absent.

### Numeric Workspace/cache/pointer lineage

- Workspace artifact and Workspace ZIP share one numeric dimension.
- If route-bounded detached material is required, one cache/material artifact and one cache/material ZIP share the next numeric dimension and declare the Workspace artifact as Parent.
- The cache/material artifact becomes the Parent ancestor for route-bound pointers.
- For the canonical one-participant example, the visible dimensions are exactly of the form:
  - `001-5-1` Workspace trace + Workspace ZIP
  - `001-5-1-1` cache trace + cache ZIP
  - `001-5-1-1-1` participant pointer
  - `001-5-1-1-1-1` From pointer
  - `001-5-1-1-1-1-1` To pointer
  - `001-5-1-1-1-1-1-1` Handoff pointer
- Missing optional participants do not reserve empty dimensions.
- Multiple participants continue the same numeric Parent chain.
- Multiple Handoff routes branch only through numeric descendant/sibling dimensions beneath their qualified Workspace/cache ancestor. No letters, route-path slugs, hashes, endpoint/participant pseudo-dimensions, or source-path-derived filename prefixes are allowed.

### Cache/material behavior

- Cache ZIP contains only exact material not already satisfied by the carried Workspace representation.
- Cache internal layout preserves adapter-resolvable material identity using qualified source/target workspace-relative paths or equivalent canonical adapter identity.
- Opaque `.bin` names are not emitted when exact source path/media identity is known.
- Role/Handoff pointers reference exact Workspace/cache material through shared Core adapter/link/material resolution such as qualified workspace-relative/permalink targets; package-local invented prefixes are not semantic identity.
- Cache is carriage/material only and creates no Role/Handoff semantics or second machine-maintained truth index.

### Role, participant and endpoint pointers

- Participant pointer(s), From pointer, To pointer and Handoff pointer are real Tiinex pointer artifacts whose declared Parent exactly matches the numeric filename lineage.
- From precedes To in the endpoint chain.
- Pointer meaning remains navigation/grounding only; Role/Handoff semantics remain owned by the referenced authoritative artifacts.
- Role identity can resolve from carried open Workspaces directly or from cache only when required material is not carried in a selected Workspace.

### VS Code shared-Core completion

- Live Role discovery starts from the actual `vscode.workspace.workspaceFolders` selected/open by the operator and uses shared Core projection against each exact qualified Workspace.
- The operator can distinguish provenance for every visible Workspace/Role candidate: host root -> qualified Workspace artifact -> projected Role/Handoff material.
- Nested fixture/test Workspaces do not appear unless they are actually explicit operator Workspace roots.
- VS Code does not create private Role/cache/package lineage, pointer naming, route projection, closure, or material-resolution semantics.
- Attach calls shared Core qualification using exact Handoff identity; duplicate Attach remains fail-closed/idempotent.
- Pack single and Pack multi use the same shared Core manufacture path and representation.
- Transport consumes each exact qualified route from that same carrier without rewriting filename dimensions/prefixes.

### Acceptance

- Golden surface test for a single route matches the clean Package V1-style shape.
- Golden surface test for a multi-route package proves the same grammar, same package format, numeric route branches, and no `e`/`p`/hash/source-path naming.
- Roundtrip orientation/grounding works without a compatibility JSON/meta manifest.
- Single-route Attach -> Pack -> Transport passes.
- Multi-route Attach -> Pack -> Transport passes.
- Cache-grounded Role/participant resolution passes with an adapter-resolvable internal cache tree.
- Open-Workspace Role discovery passes in VS Code with nested repository fixtures present.
- Loom and Kodax return exact deltas, tests, residual risks and qualified Handoffs to Anchor. Neither may self-promote to Sigma.

## Dependencies

- Exact latest-known Sigma carrier and carried Business/Core/VS Code Workspaces.
- Anchor Package Representation Convergence Evidence and Decision.
- Existing canonical Docs semantics remain read-only authority.

## Ownership Boundaries

- Core owns package manufacture/inspection/grounding, cache/material closure, route/pointer lineage, adapter resolution and shared Role/Handoff projection.
- VS Code owns host root selection, presentation/controller lifecycle and invocation of Core; it must not duplicate shared semantics.
- Docs/Axiom are unchanged unless an exact semantic contradiction is returned.
- Anchor owns fan-in and Sigma sequencing.

## Exclusions

- No cosmetic renaming of Phase 2 while retaining it as a second production representation.
- No `e`/`p` replacement with another nonnumeric pseudo-dimension.
- No source-path/hash-based recipient filename disambiguation.
- No post-pack deletion of generated metadata.
- No fixture deletion/movement to hide discovery bugs.
- No VS Code-local package/Role/cache semantic engine.
- No remote commit/push/release/publication/deployment.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-anchor-to-sigma-reconciled-real-host-acceptance-gate.trace.md)
  - Value: Ebr-Lo3KdDKoEI-6ReFR7bO19XoV_SD1UhqGTKehMZk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: UHveabmJPnd_Xcd2Zq0VujGITB3GYRIsOnunsLN1zwU