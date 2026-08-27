# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.resource.v1](https://github.com/Tiinex/docs/blob/master/.topics/.schemas/resource/tiinex.resource.v1.schema.md)
  - Created At: 2026-08-26 15:02:00
  - Trace: [001-bounty-fund.trace.md](001-bounty-fund.trace.md)
  - Origin:
    - [relative](001-bounty-fund.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 15:06:00
  - Authors: Anchor
  - Summary: Bounty financing model
  - Status: draft/local
  - Why: Materialized from the current Anchor/Sigma business design conversation under the received Anchor-to-Anchor Handoff.

---

# Bounty Financing Model

## Decision

- State: accepted
- Subject: financing and lineage shape for Tiinex bounties
- Decision: keep the bounty program inside the Tiinex Bounty Fund lineage rather than creating a separate top-level `bounties` catalog. Donations may enter the Bounty Fund directly; a specific bounty branches from that fund and preserves commitment, requested work, eligibility, allocation, judging, payout, and evidence as separate semantics.

## Basis

- The Bounty Fund is the economic pool while a specific bounty is a bounded use of that pool.
- Allocation or reservation is not payout. Reserved funds can later be released without overwriting the original commitment.

## Consequences

- Supporters can contribute to the Bounty Fund so future bounty payouts need not be personally financed by the maintainer.
- Funding source, bounty sponsor, custodian/payment operator, and payout source remain distinct.
- Existing Financial Instrument, Task, Condition, Resource Allocation, Decision, Allocation Usage, and Evidence schemas should be pressure-tested before adding a bounty-specific schema.
- An individual bounty may live as a descendant branch inside `funds/bounty/`; no sibling top-level bounty catalog is required by the current model.

## Review Conditions

- Review if repeated real bounties show that composition across existing schemas is materially cumbersome or fails to preserve required bounty semantics.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-bounty-fund.trace.md](001-bounty-fund.trace.md)
  - Value: 7bBbUYC7s19hkydtdRehVMJ-J8bgXq6WwGjVwGO2so4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 52Ngfoy9BvWtryqH7EIzZjDKlG0IP4z8A59fZugsMrA
