# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-06 00:10:00
  - Trace: [Bounded Generative Visual Source Production](004-bounded-generative-visual-source-production-process.trace.md)
  - Origin:
    - [relative](004-bounded-generative-visual-source-production-process.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-06 00:11:00
  - Authors: Anchor; Sigma
  - Why: Make host/model context an explicit production boundary when earlier visual material can contaminate a new source candidate.
  - Summary: Process step for establishing or refreshing one bounded generative context before visual-source creation.
  - Status: candidate/local

---

# Establish Generative Context Boundary

## Current Read

Before a new visual-source candidate is generated, declare which prior visual material is relevant and which is not. If the host or model demonstrably resurfaces unrelated prior material, treat the boundary as failed rather than silently prompt-debugging an unbounded number of times.

This is an operating boundary, not a claim about model internals or prompt precedence.

## Design Direction

Use the smallest boundary needed for the current source candidate. Keep process, runtime, and unrelated project semantics out of the generative instruction when they do not describe visible output. When a boundary probe fails, fail visibly and re-establish the boundary through the strongest available user/host mechanism.

## Next Artifacts

- [Generate Bounded Visual Source Candidate](004-1-1-generate-bounded-visual-source-candidate.trace.md)

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Bounded Generative Visual Source Production](004-bounded-generative-visual-source-production-process.trace.md)
  - Value: ze9D4fCvIzcuQMYgRPyXeo7glu46TK5rGm5Ux63Y8QQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:xQyIsBSY2f-9TZRpHE0e0Ap1SlEvvsNzthOUN7KEEVU
