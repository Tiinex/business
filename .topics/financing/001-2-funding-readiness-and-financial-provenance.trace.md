# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:58:00
  - Trace: [Financing](001-financing.trace.md)
  - Origin:
    - [relative](001-financing.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 13:02:00
  - Authors: Anchor; Sigma
  - Why: Make Tiinex financing useful as operational provenance rather than only a fundraising narrative, while explaining the project's real sustainability need without inventing budget, tax, accounting, or legal certainty.
  - Summary: Funding readiness, sustainable founder capacity, and the financial-provenance model for contributions, invoices, receipts, allocations, balances, and tax-related estimates.
  - Status: draft/local

---

# Funding Readiness And Financial Provenance

## Current Financial Read

Tiinex is currently a founder-led open-source project with substantial uncompensated founder work already invested. The founder is willing to continue through an initial uncompensated period so work does not stop merely because external funding is not yet available.

That willingness is **not** treated as an indefinite sustainable operating model. Without sustainable funding, concentrated project capacity may eventually have to fall back toward intermittent spare-time availability. The organizational risk is therefore continuity and delivery capacity, not a claim that Tiinex immediately ceases to exist without funding.

Current Business does not establish an authoritative cash balance, operating budget, runway, recurring cost base, founder compensation amount, secured external funding, revenue, or tax liability.

A separate current contribution artifact records the founder's **1000 SEK pledge from personal funds toward the public bounty payout**. It remains a pledge until receipt/transfer evidence exists. Founder-funded support is project commitment evidence; it is not external financing and must not be projected as recurring runway.

## Funding Readiness

The first funding case is deliberately small and concrete:

1. **Sustainable dedicated founder capacity** — provide enough predictable support that focused Tiinex work does not depend indefinitely on uncompensated personal availability.
2. **Delivery resources** — fund real project costs such as infrastructure, services, external expertise, hardware/compute, contributor support, or bounties when a bounded need exists.
3. **Broader operating capacity** — add support, governance, contributor, or adoption resources only when repeated external activity demonstrates the need.

Funding should be tied to roadmap milestones and explicit resource needs. Tiinex does not need to pretend that financing will create the project from nothing: substantial work already exists. The financing case is that stable resources can convert demonstrated momentum into more predictable delivery and lower continuity risk.

See [Sustainable Founder Capacity](001-2-1-sustainable-founder-capacity-resource-need.trace.md) for the current resource need and [Tiinex Roadmap](../initiatives/001-5-roadmap.trace.md) for phase order. See [Funding Channels And Campaigns](001-4-funding-channels-and-campaigns-discovery.trace.md) for the still-unresolved provider-neutral entrypoint model; no example provider should be projected as active until a real binding exists.

## Financial Provenance Operating Model

Tiinex should be able to support real economic use cases without pretending that the Tiinex project label is automatically a legal person, bank account, employer, tax subject, or accounting entity.

The core rule is: **preserve the actual economic party, event, state, source, and interpretation boundary; derive summaries from those records instead of asking a dashboard to become the source of truth.**

### Contributions and funding

Keep offered, pledged, received, restricted, allocated, used, returned, and withdrawn states distinct. A pledge is not a balance. A contribution receipt is not permission to use funds outside its declared boundary. External funding must remain distinguishable from founder-funded support. General Fund and purpose-specific funds are funding destinations, not proof that money is present. Personal Tip Jars are support routes/instruments and remain outside project funds unless a separate contribution event establishes otherwise.

Relevant current schema families include `tiinex.resource.need.v1`, `tiinex.resource.contribution.v1`, `tiinex.resource.contribution.receipt.v1`, `tiinex.resource.budget.v1`, `tiinex.resource.allocation.v1`, and `tiinex.resource.allocation.usage.v1`.

### Invoices and payment

A real invoice can be represented as a bounded `tiinex.instrument.financial.v1` instrument whose issuer/recipient roles, amount/currency, use boundary, status, and related resources are explicit. Creating or sending the invoice must not be interpreted as payment received. Receipt/payment evidence belongs in a separate resource/evidence trail.

The artifact must identify the actual issuer or economic party. It must not silently treat “Tiinex” as the legal invoice issuer if another person or future legal entity is the real issuer.

### Balance and available funds

A useful balance should be a **derived projection** from supported receipts, restrictions, allocations, usage, transfers, reversals, and other relevant events. It should distinguish at least received funds from pledged funds and unrestricted availability from earmarked/committed amounts.

A manually typed “balance” without a traceable derivation may be a note, but it should not outrank the underlying financial provenance.

### Tax-related estimates

Tiinex may help preserve and derive a tax reserve or estimated tax exposure when the relevant economic party, jurisdiction, period, classification assumptions, amounts, and authoritative rule sources are known.

A tax estimate is not the same thing as a legally determined tax liability, filing, assessment, or tax actually paid. Those states must remain distinguishable. When tax rules or classifications are uncertain, the uncertainty and source date must travel with the estimate rather than being hidden behind one number.

### Founder work

Founder time and in-kind effort may be preserved as contribution provenance when useful. Historical uncompensated work should not be assigned an invented monetary value, treated as a receivable, or converted into project runway without a separate evidence-backed reason.

## Funding Transparency Goal

A sponsor, contributor, founder, reviewer, or future accountant should eventually be able to ask questions such as:

- What was promised, and what was actually received?
- Which economic party received or paid it?
- What was restricted or earmarked?
- What has been allocated or used, and for what purpose?
- What amount is still available according to the underlying events?
- Which amounts are estimates rather than settled facts?
- What tax assumptions and source rules are behind a reserve estimate?
- Which roadmap outcome was a contribution intended to enable?

The answer should be inspectable through lineage rather than requiring trust in one opaque dashboard.

## What Financing Does Not Yet Establish

- an amount required for sustainable founder compensation;
- a project budget or monthly burn rate;
- secured or recurring external funding;
- a legal entity, employer, payroll structure, or accounting system;
- a current tax classification or tax reserve amount;
- invoice numbering/legal requirements for any jurisdiction;
- accounting balances suitable for statutory reporting;
- investment terms, valuation, equity, or expected financial return.

Those details should be added only when the real party, jurisdiction, event, amount, and evidence exist.

## Interpretation Limits

This artifact defines the Business operating boundary for funding and financial provenance. It is not accounting, bookkeeping certification, tax/legal/investment advice, a financial statement, or evidence that any pledged resource has been received. Specialized professional/legal/accounting requirements may later become necessary; Tiinex provenance should help preserve their sources and results rather than claiming to replace them.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Financing](001-financing.trace.md)
  - Value: LTTkyewmuNe9TEAVXdu4Nl28fHjw18N_PzWcMOCIYqg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:-mdHGn9grRbUvrLrdxO9SNzLfacqy1C4kpoUjtX-QJk
