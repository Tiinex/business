# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:31
  - Trace: [001-durable-review-records.trace.md](001-durable-review-records.trace.md)
  - Origin:
    - [relative](001-durable-review-records.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:32
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: Early exporter explicitly read YouTube feedback state and wrote source-neutral Markdown.
  - Status: approved-for-publication

---

# Turning a stream signal into a portable Topic

On **May 13, 2026**, Tiinex/docs included a readable Topic convention and an exporter. The original README says that the exporter reads topic-shaped state from `youtube/tools/feedback-review-state.json`, while explicitly warning that the durable records should remain **source-neutral** rather than YouTube-specific.

The sample Topic carried retained messages, AI-simulated role reviews, an evidence register and a follow-up step. There was no requirement for a reader to run the YouTube host or a special UI to understand the record.

## Inspect it

- [The original Topics README / exporter guidance](https://github.com/Tiinex/docs/blob/53fe17ea23d3da3d994f14a2cda1d904ca478510/topics/README.md).
- [The concrete example Topic](https://github.com/Tiinex/docs/blob/53fe17ea23d3da3d994f14a2cda1d904ca478510/topics/agent-topic-1-hud-upkeep-and-proof.topic.md).

## Distinct levels of evidence

The README **describes** an exporter path and source file. The checked-in Topic **shows** a resulting readable artifact. This does not by itself establish end-to-end reliability of every external-channel import, or prove that the now-unavailable old `youtube` repository remains usable.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-durable-review-records.trace.md](001-durable-review-records.trace.md)
  - Value: O-Swu3GgbsfgFP5M14W-8szNCIHjtp75QmaZLGP_pYk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: rlYEm8v3mxM_dVxPcjo5zrA4en47CQ8UZYTUX3KhMlY
