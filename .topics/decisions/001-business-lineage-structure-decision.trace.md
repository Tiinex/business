# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.party.organization.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/party/organization/tiinex.party.organization.v1.schema.md)
  - Created At: 2026-08-26 14:55:00
  - Trace: [001-tiinex.trace.md](../001-tiinex.trace.md)
  - Origin:
    - [relative](../001-tiinex.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 15:04:00
  - Authors: Anchor
  - Summary: Business lineage structure
  - Status: accepted/local
  - Why: Preserve the current authoring convention that keeps organizational lineage readable and dimension-consistent across Tiinex Business.

---

# Business Lineage Structure

## Decision

- State: accepted
- Subject: organizational lineage and filename discipline in tiinex/business
- Decision: `.topics/001-tiinex.trace.md` is the Tiinex organization root. Each real top-level semantic branch starts with its local branch-anchor dimension, normally `001`. A direct semantic child extends the parent's visible filename dimension path by exactly one child segment (`001` -> `001-1`, `001-2`, ...); deeper descendants extend the same path (`001-1` -> `001-1-1`, ...). The filename dimension path is a human-readable projection of declared Parent ancestry, never a replacement for Parent authority. Repository directories aid navigation but do not own semantic authority, and collection directories such as `decisions/` do not add invented semantic dimension levels merely because they store artifacts. New or materially updated Tiinex-authored organizational `.trace.md` filenames follow this full visible lineage-path rule. Schemas and explicitly non-organizational artifacts may retain their own authority roots.

## Basis

- A human contributor should be able to open current work locally and follow Parent upward when more context is needed.
- Path conventions alone are not enough to establish semantic ancestry.
- A full lineage-path filename lets a human infer parent/child shape before opening an artifact, while Parent remains the exact semantic authority.
- Git history preserves superseded current states, so current artifacts may be corrected without fabricating historical Parent facts.

## Consequences

- Roles, Initiatives, Financing, Funds, and other real subject branches use explicit local anchors; their semantic descendants extend the anchor's visible dimension path one segment per Parent edge.
- Tiinex is the Organization root; concrete Projects, Roles, funds, and work packages use their appropriate schemas.
- Business remains a manager-readable organizational surface; detailed implementation Tasks live in their natural repository while retaining truthful upward organizational context.
- New collection folders are not semantic parents by default, and no semantic branch should be created only as empty taxonomy.

## Review Conditions

- Review if Tiinex gains an explicit branch-anchor schema or another declared authority that supersedes this local anchor convention.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-tiinex.trace.md](../001-tiinex.trace.md)
  - Value: p4YGHsMqWThhcRwqAOWh1RznaqBKd_pndsSvDXyZycQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: MRQmbtUsgj-Bt8FUBjSO9CKlFoKIPYOoXopTtpWVizY
