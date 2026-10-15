# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:48
  - Trace: [001-qualified-continuity.trace.md](001-qualified-continuity.trace.md)
  - Origin:
    - [relative](001-qualified-continuity.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:49
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: Late summer distinguished qualified responsibility transfer from a byte carrier.
  - Status: approved-for-publication

---

# Handoff meaning and package mechanics diverged

A key late-summer distinction is that the **Handoff** and the **Handoff Package** became separate types. The first describes what work or responsibility is being transferred, from whom, to whom and under what constraints. The second describes a carrier/recipient entry surface and exactly which material was transported.

- [August 22 Handoff schema source](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md).
- [September 1 Handoff Package schema source](https://github.com/Tiinex/docs/blob/25cb94d68a46d8670d437869e67c4555e74b2f26/.topics/.schemas/coordination/handoff/package/tiinex.handoff.package.v1.schema.md).

A ZIP can preserve files while still leaving authority unknown. Conversely, a Handoff may name work without the recipient having a sufficient package or supported runtime to perform it. Package membership is not automatically authority, and a passing integrity check is not a truth guarantee.

The task for a reviewer is to inspect the exact source and ask which boundary was actually checked, not accept "portable" or "verified" as universal verdicts.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-qualified-continuity.trace.md](001-qualified-continuity.trace.md)
  - Value: Qu3WL9dYGn060RzwtCrTmO5IEib7icuv6yXt83-jbp0

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: GQpCCse380RF35f4gQjjz7ggwfnSgWqugtbUkg5ZQm0
