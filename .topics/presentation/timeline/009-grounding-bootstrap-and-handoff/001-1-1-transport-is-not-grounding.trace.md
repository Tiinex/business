# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:49
  - Trace: [001-1-how-the-late-contracts-diverged.trace.md](001-1-how-the-late-contracts-diverged.trace.md)
  - Origin:
    - [relative](001-1-how-the-late-contracts-diverged.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:50
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: Disambiguate transfer, qualification and warranted claims.
  - Status: approved-for-publication

---

# Transport, qualification, grounding and truth are different

Transport says **which bytes arrived**. Integrity can demonstrate those bytes match a declared digest. A schema contract may permit structural and semantic qualification for a bounded kind of record. Grounding asks whether the *recipient* identified the correct sources, frontier and authority boundaries. Truth or warranted inference requires examination of the real evidence behind claims.

A valid package can still contain a mistaken explanation. A fluent recipient can still invent a missing parent, overstate a Role's authority or miss the currently active Handoff. Therefore a trustworthy review requires negative tests, missing-source behavior and explicit uncertainties.

## Source anchors

- [Carrier schema](https://github.com/Tiinex/docs/blob/25cb94d68a46d8670d437869e67c4555e74b2f26/.topics/.schemas/coordination/handoff/package/tiinex.handoff.package.v1.schema.md); [authoritative Handoff contract](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md); [cold-entry recovery implementation](https://github.com/Tiinex/core/blob/7a4c0e1eab27559eef417cf5eb1c15d47483d199/src/tooling/portable/handoff/bootstrapRecovery.js).

## Observable failure cases worth testing

- source bytes altered after sealing;
- a nonselected Handoff mistaken for the active route;
- a recipient inventing access to a Workspace or Role absent from the package;
- a correct but irrelevant historical Parent treated as authorization to perform new work;
- an interpretation trusted merely because a checksum matches.

Any tested outcome should report exact tool versions, source versions, host limitations and whether failure was detected, blocked or only noted.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-how-the-late-contracts-diverged.trace.md](001-1-how-the-late-contracts-diverged.trace.md)
  - Value: GQpCCse380RF35f4gQjjz7ggwfnSgWqugtbUkg5ZQm0

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 2uxRd7APsbXwq8DqWzqkxPGFeV9fgbjrrhWSVudyJqc
