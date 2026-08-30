# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:58:00
  - Trace: [001-financing.trace.md](../001-financing.trace.md)
  - Origin:
    - [relative](../001-financing.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:59:00
  - Authors: Anchor
  - Why: Materialized from the current Anchor/Sigma business design conversation under the received Anchor-to-Anchor Handoff.
  - Summary: Funds
  - Status: accepted/local

---

# Funds

## Current Read

This branch groups persistent Tiinex project funding destinations. It is a subject branch and does not itself represent a fund, balance, contribution, allocation, or financial instrument.

## Design Direction

Each concrete fund owns its own Resource-rooted lineage. General Fund is the default project-funding destination when no narrower project fund is explicitly selected; Bounty Fund is purpose-bounded. Receipts, allocations, usage, reversals, releases, and transfers belong with the affected fund instead of being duplicated into a separate donations catalog.

## Next Artifacts

General Fund and Bounty Fund are the current persistent destinations. Add future purpose-specific fund roots only when a real commitment, restriction, or allocation requires them. A fund artifact does not by itself prove custody, receipt, or balance.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-financing.trace.md](../001-financing.trace.md)
  - Value: LTTkyewmuNe9TEAVXdu4Nl28fHjw18N_PzWcMOCIYqg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: HtUMdKLV37Rcm-RlatIrRSqX90zVcdXmc3Zi7xV4tjM
