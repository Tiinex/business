# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:59:00
  - Trace: [Funds](../001-1-funds.trace.md)
  - Origin:
    - [relative](../001-1-funds.trace.md)
- Current
  - Current Schema: [tiinex.resource.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/resource/tiinex.resource.v1.schema.md)
  - Created At: 2026-08-29 13:24:00
  - Authors: Anchor; Sigma
  - Summary: Tiinex General Fund
  - Status: draft/local
  - Why: Restore a truthful general project-funding destination so unrestricted or not-more-specifically-targeted project funding has a stable provenance anchor without pretending a balance or bank account already exists.

---

# Tiinex General Fund

## Resource Identity

- Resource Label: Tiinex General Fund
- Resource Kind: funds

## Resource Role

- Resource Role: availability

## Resource Boundary

- Resource Boundary: default Tiinex project-funding destination when no more specific project fund is explicitly selected; later use remains bounded by separately declared recipient/economic-party, legal, financial, restriction, allocation, and usage context

## Resource State

- Resource State: unknown

## Operating Boundary

- A pledge or support route does not create General Fund balance.
- Receipt evidence must identify the real economic recipient or custodian before funds can be projected as received.
- Available balance should be derived from supported receipts, restrictions, allocations, usage, transfers, reversals, and other relevant events.
- A future legal entity, account, or accounting system may become relevant, but this artifact does not assume one exists now.

## Interpretation Limits

- Limits: this artifact identifies a persistent project-funding destination. It does not state an authoritative current balance, prove receipt/custody/ownership, establish a bank account or legal entity, determine tax/accounting treatment, or constitute accounting.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Funds](../001-1-funds.trace.md)
  - Value: HtUMdKLV37Rcm-RlatIrRSqX90zVcdXmc3Zi7xV4tjM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:QOCsuZ-T8IdFTzTIwViXv3EUJ5mxRpEVyIoxIrX03-I
