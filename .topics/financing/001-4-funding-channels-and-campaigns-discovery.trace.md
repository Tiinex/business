# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:58:00
  - Trace: [Financing](001-financing.trace.md)
  - Origin:
    - [relative](001-financing.trace.md)
- Current
  - Current Schema: [tiinex.discovery.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/discovery/tiinex.discovery.v1.schema.md)
  - Created At: 2026-08-29 13:57:00
  - Authors: Anchor; Sigma
  - Why: Explore the minimum provider-neutral artifact model needed for Tiinex to present multiple funding/support entrypoints without hardcoding PayPal, Kickstarter, or another provider into organizational semantics.
  - Summary: Funding channels and campaigns discovery for provider-neutral support routes, campaign presentation, provider bindings, and traceable financial events.
  - Status: draft/local

---

# Funding Channels And Campaigns

## Discovery Intent

- Intent: determine the smallest readable model that lets an artifact-driven Tiinex runtime discover and present one or more ways to support a person, project, fund, milestone, bounty, or campaign while preserving the real recipient, purpose, provider boundary, and later financial provenance.
- Starting Question: how can Tiinex express a support proposition once, expose it through one or several channels, and later tell which real contributions came through which channel without making any provider the semantic type?

## Discovery Field

- Field: Tiinex Financing semantics and representative public support/crowdfunding/payment routes.
- In Scope: long-lived support routes such as a Tip Jar or general project support; bounded campaigns with a target outcome; one-to-many channel/provider bindings; public entrypoints; channel/provider state; recipient/economic-party identity; contribution/receipt provenance; provider-neutral presentation; examples such as PayPal, Kickstarter, GitHub Sponsors, direct transfer, and a Tiinex-owned presentation surface.
- Out Of Scope: creating provider accounts, launching a real campaign, storing secrets, payment credentials, API implementation, webhook code, tax/legal classification, securities analysis, accounting treatment, or claiming any example provider is currently available to Tiinex.

## Discovery Method

- Method: test a working separation against several materially different routes rather than designing around one provider. The working hypothesis is **support/funding proposition or campaign -> channel binding -> provider/presentation implementation -> contribution/receipt event -> fund/allocation/usage**. Compare where provider-specific rules belong and reject any model that requires the Campaign or organizational purpose to become `PayPal`, `Kickstarter`, or another provider type.
- Evidence Approach: preserve provider capabilities/rules as external or technical context; preserve organizational purpose and economic events in Tiinex artifacts; create Finding/Decision artifacts only when a distinction survives multiple test cases.

## Discovery Boundaries

- Boundary: Campaign, Channel, Provider Adapter, Financial Instrument, Contribution, Receipt, Fund, Allocation, and Usage are not declared equivalent. This Discovery does not yet establish a canonical Funding Channel schema or Campaign schema.
- Runtime Boundary: Business may declare public semantic configuration such as purpose, recipient, active/proposed route, and safe locator when justified. Secrets and provider-specific execution belong behind appropriate host/technical boundaries.
- Authority Boundary: a visible channel or campaign does not prove money was received; actual economic events and their evidence own that claim.

## Discovery Outcome

- Outcome: planned discovery. Current Business financing requirements and the artifact-driven runtime direction support the provider-neutral hypothesis strongly enough to preserve and test it, but no permanent Campaign/Channel schema or provider adapter contract is accepted yet.
- Current Useful Distinction: a Campaign should own **what support is trying to achieve and why**; a Channel should own **where/how someone can participate**; provider-specific implementation should stay below that; financial event artifacts should own **what actually happened**. This remains a working hypothesis until the Discovery produces accepted findings.
- Next Artifacts: create bounded Findings when concrete provider comparisons expose stable requirements; create a Decision/schema work item only if the same distinctions remain useful across multiple channels and support forms.

## Interpretation Limits

- Limits: this artifact does not prove that Tiinex has PayPal, Kickstarter, GitHub Sponsors, bank-transfer support, an active campaign, received funding, provider approval, a legal fundraising structure, or settled tax/accounting treatment. The named providers are test cases, not commitments or endorsements.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Financing](001-financing.trace.md)
  - Value: LTTkyewmuNe9TEAVXdu4Nl28fHjw18N_PzWcMOCIYqg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 1YVYlJwGFiuzrapMGdSS5idTzHJpd0lQzo9gIxFa8v4
