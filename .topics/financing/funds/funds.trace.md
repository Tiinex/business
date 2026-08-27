# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:58:00
  - Trace: [financing.trace.md](../financing.trace.md)
  - Origin:
    - [relative](../financing.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:59:00
  - Authors: Anchor
  - Why: Materialized from the current Anchor/Sigma business design conversation under the received Anchor-to-Anchor Handoff.
  - Summary: Funds
  - Status: draft/local

---

# Funds

## Current Read

This branch groups persistent Tiinex project funding destinations. It is a subject branch and does not itself represent a fund, balance, contribution, allocation, or financial instrument.

## Design Direction

Each concrete fund owns its own Resource-rooted lineage. Receipts, allocations, usage, reversals, releases, and transfers belong with the affected fund instead of being duplicated into a separate donations catalog.

## Next Artifacts

General Fund, Bounty Fund, and future purpose-specific fund roots when their boundaries are explicit.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [financing.trace.md](../financing.trace.md)
  - Value: 0VYrDWW46FFpadoVL9t-AL68Hm2DhRaOC02TcbB5KjU

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: bep1ZhcKdu9k6dPIeCMHMgy5hiKqAvFA3e7CItKmHqk