# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:42
  - Trace: [001-1-the-rough-screen-recording-protocol.trace.md](001-1-the-rough-screen-recording-protocol.trace.md)
  - Origin:
    - [relative](001-1-the-rough-screen-recording-protocol.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:43
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: June Courier staging predates the July video workaround and late-summer schema split.
  - Status: approved-for-publication

---

# Handoff ideas existed before the ZIP contract

An important chronology guard: the video workaround did not *invent* the concept of transferring work. Earlier code already explored that problem.

The **June 12–13 Courier experiment** included bounded artifact staging, receipt-like handling and attempts to move material across a work boundary in the VS Code context. The code is not the same semantic object as a late-August Handoff or a September Handoff Package.

- [Courier staging implementation at the June source revision](https://github.com/Tiinex/ai-vscode-tools/blob/e43532ff719bc00e43720a0bc3f20f6e9db7dec6/src/courierBridge/staging.ts).
- [Later explicit Handoff schema, August 22](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md).
- [Distinct Handoff Package schema, September 1](https://github.com/Tiinex/docs/blob/25cb94d68a46d8670d437869e67c4555e74b2f26/.topics/.schemas/coordination/handoff/package/tiinex.handoff.package.v1.schema.md).

## The combined story

The earlier Courier tooling shows work-transfer interest *before* screen recordings. The July recordings explain why the developer considered **machine-readable, portable and recoverable** transport a pressing practical need. Those are compatible statements — not competing claims about one invention date.

## What remains uncertain

How much June Courier code was used in a live workflow and exactly which requirements from video transferred into later implementations cannot be inferred from the source code alone.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-the-rough-screen-recording-protocol.trace.md](001-1-the-rough-screen-recording-protocol.trace.md)
  - Value: ESm0HQImvouGjkL8y7Utj9tTeko8FcmYK5MD5_Zzqy0

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: lfoCzPxqrhIC-UG1TyvX6hjPDWo58NdyTpW_KAyAq3A
