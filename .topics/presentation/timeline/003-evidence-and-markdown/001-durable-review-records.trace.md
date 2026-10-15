# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:30
  - Trace: [001-1-1-youtube-hud-and-proof.trace.md](../002-the-question-of-agent-review/001-1-1-youtube-hud-and-proof.trace.md)
  - Origin:
    - [relative](../002-the-question-of-agent-review/001-1-1-youtube-hud-and-proof.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:31
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: Markdown Topic evidence and schema genealogy.
  - Status: approved-for-publication

---

# Evidence needed to survive the conversation

One answer about what an agent had done was not enough if that answer vanished with a session or could not be checked. During May, inspectable Markdown Topic records, task-origin traces and explicit continuity contracts developed as **working artifacts**, rather than as a wholly finished specification designed first.

## Dated anchors

- [Portable Markdown Topic format, May 13](https://github.com/Tiinex/docs/blob/53fe17ea23d3da3d994f14a2cda1d904ca478510/topics/README.md) — durable, printable, readable without YAML frontmatter; with retained messages, role reviews, evidence and decisions.
- [Shared continuity-envelope schema, May 28](https://github.com/Tiinex/docs/blob/776fb804109ef51fad8d0f37c630bc32521c1500/.topics/.schemas/tiinex.continuation.v1.md) — defines an orienting header distinct from the artifact body's semantics.

## Why Markdown?

Markdown can remain readable in a normal text viewer, survive copy/transport, be versioned in Git and carry typed links without depending on a particular host UI. It is a choice of **artifact surface**, not a claim that validation should be done by prose alone. JavaScript, Python, stricter schema tooling and other runtimes can implement the mechanical checks.

## A crucial distinction

An artifact may have a correct envelope, checksum, current schema and Parent reference while making an unsupported claim. **Integrity is not truth.** A reviewer still needs to examine evidence and limitations.

## What this does not show

The May schemas were provisional and subsequently revised. The current Tiinex root schema must not be projected back onto those old snapshots as though it had already existed.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-youtube-hud-and-proof.trace.md](../002-the-question-of-agent-review/001-1-1-youtube-hud-and-proof.trace.md)
  - Value: Ki0LpOd1s1mVKApX1OmER7htAYz67zMH6e3ubDRZcvs

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: O-Swu3GgbsfgFP5M14W-8szNCIHjtp75QmaZLGP_pYk
