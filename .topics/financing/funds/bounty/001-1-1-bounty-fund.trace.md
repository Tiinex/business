# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:59:00
  - Trace: [001-1-funds.trace.md](../001-1-funds.trace.md)
  - Origin:
    - [relative](../001-1-funds.trace.md)
- Current
  - Current Schema: [tiinex.resource.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/resource/tiinex.resource.v1.schema.md)
  - Created At: 2026-08-26 15:02:00
  - Authors: Anchor
  - Summary: Tiinex Bounty Fund
  - Status: accepted/local
  - Why: Materialized from the current Anchor/Sigma business design conversation under the received Anchor-to-Anchor Handoff.

---

# Tiinex Bounty Fund

## Resource Identity

- Resource Label: Tiinex Bounty Fund
- Resource Kind: funds

## Resource Role

- Resource Role: availability

## Resource Boundary

- Resource Boundary: Tiinex project funding destination earmarked for future public bounties and bounty payouts; individual bounty commitments and payouts require descendant artifacts

## Resource State

- Resource State: unknown

## Interpretation Limits

- Limits: this artifact identifies the bounty funding destination and its use boundary. It does not state an authoritative current balance, prove receipt or custody, create a specific bounty obligation, or constitute accounting.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-funds.trace.md](../001-1-funds.trace.md)
  - Value: HtUMdKLV37Rcm-RlatIrRSqX90zVcdXmc3Zi7xV4tjM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: pBpDDPAlhNO3MzIj_m-3jvpXJRxldC_G83UzgSe3bQ4
