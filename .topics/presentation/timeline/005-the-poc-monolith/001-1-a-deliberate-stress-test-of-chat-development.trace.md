# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:39
  - Trace: [001-speed-and-its-cost.trace.md](001-speed-and-its-cost.trace.md)
  - Origin:
    - [relative](001-speed-and-its-cost.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:40
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: Deliberate feature growth until scaling and even continuing the work became expensive.
  - Status: approved-for-publication

---

# What the monolith was actually testing

The developer describes the proof-of-concept monolith as an **intentional limit-seeking experiment** carried out largely through ordinary ChatGPT Web. The aim was to keep integrating useful features and observe how far this could go before the effort to understand the combined code, make reliable changes, scale the implementation and even continue development became disproportionate.

This is more specific than "a monolith that later needed a refactor." The same experiment was testing the **software** and the **conversational development environment** carrying the work.

## Questions the experiment raised

- How quickly can a conversational workflow expand a working UI?
- When does the cost of re-grounding, debugging and making coherent changes begin to dominate?
- How much architecture can remain implicit in conversation before it is too expensive to maintain?

## Evidence boundary

The motive and subjective point of unsustainability are developer testimony. They were **not** measured in a published benchmark with fixed feature counts, model control groups or reproducible break-even metrics. The July [site runtime](https://github.com/Tiinex/site/blob/f42cd25de946966360fe2c58e7229b608d72b55e/app.js) is a concrete code checkpoint but cannot by itself prove when the experiment felt unsustainable.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-speed-and-its-cost.trace.md](001-speed-and-its-cost.trace.md)
  - Value: e5dee0gidRiP-PlSBsKXzhcdFIHcic8sN76Fe5paqQ8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: iKDBb_LT10OsdYu7SNM0Qgo-NKJIIPujt8htQdYvOCc
