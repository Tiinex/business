# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:58:00
  - Trace: [001-financing.trace.md](001-financing.trace.md)
  - Origin:
    - [relative](001-financing.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 15:05:00
  - Authors: Anchor
  - Summary: Financing lineage model
  - Status: draft/local
  - Why: Materialized from the current Anchor/Sigma business design conversation under the received Anchor-to-Anchor Handoff.

---

# Financing Lineage Model

## Decision

- State: accepted
- Subject: Tiinex financing lineage
- Decision: model financial history as append-oriented lineage under concrete funds. Real receipts, allocations, usage, reversals, releases, and transfers belong in the affected fund lineage; there is no separate donations catalog. Current balances are projections over preserved events rather than mutable source fields.

## Basis

- This preserves true origin and keeps receipt, allocation, actual use, and later correction as distinct claims.
- It avoids counting internal fund-to-fund movement as new external income and keeps payment-provider transport separate from economic source and purpose.

## Consequences

- General Fund is the default unrestricted destination when no explicit fund is selected.
- Provider transaction identifiers may support technical reconciliation/idempotency but are not Tiinex semantic identity.
- Public artifacts must not publish sensitive payer, billing, account, or provider metadata merely because a payment service exposes it.
- Refunds, reversals, releases, and corrections append later events rather than rewriting historical events.
- Currency remains truthful in its original denomination. Cross-currency totals require a separately grounded projection with exchange rate, source, and time.
- Provider fees and currency conversions should remain visible as their own economic events or projections when they materially affect later accounting.
- Bookkeeping, tax, accounting, and administrative outputs may be derived later but are not claimed to be satisfied by the lineage alone.

## Review Conditions

- Review when real payment integrations or jurisdiction-specific bookkeeping requirements expose missing semantics.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-financing.trace.md](001-financing.trace.md)
  - Value: 2Ja7fNJ6bWvxuydz7ZnW5c4gkMip1K38pEE55WYV0xM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: T_WL3JYPFXYjvpRF_9K6VWpgeuurRfsRCTSyUYCzBV0
