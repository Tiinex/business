# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:44
  - Trace: [001-1-1-decomposition-is-not-semantic-authority.trace.md](001-1-1-decomposition-is-not-semantic-authority.trace.md)
  - Origin:
    - [relative](001-1-1-decomposition-is-not-semantic-authority.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:45
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: September work checked bootstrap recovery without assuming every host can run it.
  - Status: approved-for-publication

---

# Cold recovery became a concrete implementation question

Decomposition only helps if the recipient can still find its sources and use the package after a boundary crossing. This pushed the system toward explicit package-local bootstrap descriptors, source membership, links and integrity checks.

By **September 18**, Core contained concrete portable-bootstrap recovery logic. The code treats the bootstrap as a specific material and checks available package findings rather than trusting a ZIP name.

- [Core bootstrap recovery implementation checkpoint](https://github.com/Tiinex/core/blob/7a4c0e1eab27559eef417cf5eb1c15d47483d199/src/tooling/portable/handoff/bootstrapRecovery.js).
- [Package schema describing the carrier boundary](https://github.com/Tiinex/docs/blob/25cb94d68a46d8670d437869e67c4555e74b2f26/.topics/.schemas/coordination/handoff/package/tiinex.handoff.package.v1.schema.md).

## Practical result sought

A cold recipient should recover the supplied Workspace frontier and declared route, or explain why it cannot. This is narrower than promising platform-independent execution in arbitrary hosts.

## Limit

The presence of a recovery implementation does not establish universal portability; runtime availability, model behaviour, source completeness and recipient tests remain separate evidence obligations.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-decomposition-is-not-semantic-authority.trace.md](001-1-1-decomposition-is-not-semantic-authority.trace.md)
  - Value: hFlixRcBRC1WbQ8QQB6-oZfBHrBzQvhFLLhsRErlUhY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: mVqZ1IOhtsfNJtBrkOsdF-_9O47mSlg6nA0E_MrcwRY
