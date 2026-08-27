# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:59:00
  - Trace: [funds.trace.md](../funds.trace.md)
  - Origin:
    - [relative](../funds.trace.md)
- Current
  - Current Schema: [tiinex.resource.v1](https://github.com/Tiinex/docs/blob/master/.topics/.schemas/resource/tiinex.resource.v1.schema.md)
  - Created At: 2026-08-26 15:01:00
  - Authors: Anchor
  - Summary: Tiinex General Fund
  - Status: draft/local
  - Why: Materialized from the current Anchor/Sigma business design conversation under the received Anchor-to-Anchor Handoff.

---

# Tiinex General Fund

## Resource Identity

- Resource Label: Tiinex General Fund
- Resource Kind: funds

## Resource Role

- Resource Role: availability

## Resource Boundary

- Resource Boundary: default unrestricted Tiinex project funding destination when no more specific fund is explicitly selected; later use remains bounded by separately declared organizational, project, legal, financial, and allocation context

## Resource State

- Resource State: unknown

## Interpretation Limits

- Limits: this artifact identifies a persistent funding destination. It does not state an authoritative current balance, prove that funds have been received, prove custody or ownership, or constitute accounting.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [funds.trace.md](../funds.trace.md)
  - Value: bep1ZhcKdu9k6dPIeCMHMgy5hiKqAvFA3e7CItKmHqk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: JHdQ3wqrY55CDVWuWAHbqSKi0X074rIU3NY10fK0P-c