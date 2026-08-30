# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.transition.definition.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/transition/definition/tiinex.transition.definition.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Trace: [Acceptance Review](001-1-1-1-acceptance-review.trace.md)
  - Origin:
    - [relative](001-1-1-1-acceptance-review.trace.md)
- Current
  - Current Schema: [tiinex.relation.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/relation/tiinex.relation.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Authors: Anchor; Sigma
  - Why: Represent the accepted branch as an artifact sibling and let it delegate the landing details to a separate sub-process instead of expanding the higher-level process with current tooling mechanics.
  - Summary: Proposed accepted branch from Acceptance Review that hands the accepted candidate into the Accepted Change Landing sub-process.
  - Status: proposed/local

---

# Accepted Outcome Path

## Relation Declaration

- Relation Type: process branch uses sub-process
- Relation Direction: accepted branch -> sub-process definition
- Relation Scope: development-and-acceptance process-definition topology
- Relation Family: process composition

## Relation Target

- Target: [Accepted Change Landing](001-2-accepted-change-landing-process.trace.md)

## Relation Boundary

The relation target is not the Tiinex continuity Parent. This relation is the accepted branch in the proposed higher-level process and delegates its landing detail to a separate reusable sub-process. The sub-process target is not this artifact's Tiinex `Parent`. This relation does not assert that any real Epic is accepted, landed, committed, pushed, or complete; real acceptance and landing evidence remain owned by the artifacts appropriate to that execution.

## Interpretation Limits

- Sibling position expresses that this accepted path is an alternative to the Return To Development path at the same represented acceptance branch point.
- Process composition does not require the higher-level process to duplicate the sub-process descendants.
- The branch does not require every real execution to materialize a matching relation artifact.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Acceptance Review](001-1-1-1-acceptance-review.trace.md)
  - Value: 3g643_gSe0ys7HFbGiTE7C2NI1KbnVijZd_fehDQi0g

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: IGR-WR-ykk32zHeqsSyb53qfJPkpIgnkX26WLUWlPmM
