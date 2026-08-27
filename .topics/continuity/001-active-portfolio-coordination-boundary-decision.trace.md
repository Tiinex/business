# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 21:31:12
  - Authors: Anchor, Sigma
  - Why: Establish one explicit active coordination frontier in tiinex/business while preserving older carried material as history and allowing implementation work to remain in its natural repository.
  - Summary: Active Tiinex portfolio coordination begins from this decision; Business anchors cross-repository initiatives and processes without becoming a central implementation task store.
  - Status: accepted/local

---

# Active Tiinex Portfolio Coordination Boundary Decision

This decision establishes the current business-level coordination frontier for Tiinex after the role consolidation and repository discovery review.

## Decision

- State: accepted
- Subject: active Tiinex portfolio coordination, cross-repository initiative anchoring, and continuation frontier
- Decision: treat this decision and its descendants as the current Business coordination lineage for the reset. Tiinex/business owns stable organizational anchors such as Roles, Initiatives, and later reusable Process material when Business is their natural home; implementation Tasks, Decisions, Evidence, Handoffs, and other work artifacts may remain in their natural repositories and bind back through stable permalinks. Older carried Business cache and prior handoff material remain available as historical/reference evidence and are not rewritten by this decision.

## Basis

- Cross-repository work should not be forced into Business merely to appear coordinated.
- Stable Business anchors let Discovery and permalinks connect work without collapsing repository ownership, artifact lineage, and organizational scope into one hierarchy.
- The current Roles have been explicitly landed in Business, while Initiative and Process structure is now being designed from observed real work rather than invented taxonomy.

## Consequences

- New Initiative roots and future Business-level Process material should continue from the active Business surface established after this decision, not from older transport/cache scaffolding by default.
- A Handoff that carries this Business reset forward must declare this decision as its direct Parent and continue the same lineage as a child artifact, so Discovery can surface the decision or a later descendant as the current frontier.
- Historical material remains readable and useful for audit, dogfooding, and recovery; this decision does not delete, rewrite, publish, or retroactively reclassify source authority.
- Read-only or historical treatment is a governance boundary unless separately enforced by Tooling or repository permissions.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:k9BfNtThdKxDYV-qs5hZ_3bevbm9jFwl5G_tk0-iQsw
