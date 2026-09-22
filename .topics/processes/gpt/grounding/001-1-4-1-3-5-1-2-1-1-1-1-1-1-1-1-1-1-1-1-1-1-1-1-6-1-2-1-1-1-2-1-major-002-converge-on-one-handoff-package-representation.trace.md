# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 11:36:22
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-2-major-002-one-handoff-package-representation-evidence.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-2-major-002-one-handoff-package-representation-evidence.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-2-major-002-one-handoff-package-representation-evidence.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-22 11:36:33
  - Authors: Anchor
  - Why: Route cardinality must not change the recipient format or filename/Parent-lineage grammar.
  - Summary: Package V1 numeric lineage is the single recipient-facing representation; Phase 2 mechanics may be reused internally but not remain a second normal package standard.
  - Status: ready/local

---

# Anchor Decision — Converge Major 002 On One Handoff Package Representation

## Decision

- State: accepted
- Subject: final recipient-facing Handoff package representation and VS Code/Core ownership boundary for Major 002
- Decision: there is exactly one normal recipient-facing Handoff Package representation. Route cardinality must not select another package format. Package V1's numeric Parent-lineage surface is the representation baseline. JSON-free exact-byte/cache/closure mechanics developed in artifact-first Phase 2 may be reused internally, but Phase 2 must not remain a second normal recipient-facing standard.

## Basis

- The latest multi-route carrier visibly violates Tiinex filename/Parent lineage through route-path/hash names and `e`/`p` pseudo-dimensions.
- Current Package V1 already implements the required Workspace -> cache -> participant -> From -> To -> Handoff numeric Parent chain for one selected route.
- The original compatibility JSON problem required replacement of reconstruction mechanics, not replacement of the Handoff Package representation.
- Maintaining two normal builders creates a recurring risk that one route-count path silently reintroduces semantic/representation drift.

## Consequences

- Loom owns convergence of single- and multi-route manufacture/inspection/grounding onto one Package V1-style recipient surface.
- Kodax owns VS Code consumption of shared Core discovery/manufacture/transport mechanics and explicit provenance of open Workspace roots. VS Code may present/select but must not reconstruct Role/Handoff/cache/package semantics.
- Cache trace/ZIP occupy one numeric lineage dimension beneath their Workspace and above route-bound pointers.
- Participant/From/To/Handoff pointers remain numeric Parent descendants and resolve into Workspace/cache via shared adapters and qualified link/material targets.
- No `recipient-v2.transport.json`, equivalent durable machine manifest, `e`/`p` dimension, route hash/path slug, or route-count-dependent package standard is permitted on the normal recipient surface.
- Transport may project one or many qualified routes, but package filename/prefix presentation must not rewrite artifact lineage or pretend one route is the identity of a multi-route carrier.

## Review Conditions

- Review immediately if Loom finds an unavoidable semantic contradiction in canonical Docs or if Package V1 cannot absorb JSON-free verification without introducing a second durable truth surface.
- Axiom remains dormant unless such an exact semantic contradiction is returned.
- Reopen Sigma only after Anchor proves single-route and multi-route structural parity and Kodax proves open-Workspace Role discovery against the same shared Core mechanics.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-2-major-002-one-handoff-package-representation-evidence.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-2-major-002-one-handoff-package-representation-evidence.trace.md)
  - Value: zzBRkzdAmQ4FBGQSIB6OO5KSbZaYi1tW4ydmjEeAnUs

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: iw-Wr8TFzUVhTIeordOqmmelBIY_yOGVue_RaEd_lwg