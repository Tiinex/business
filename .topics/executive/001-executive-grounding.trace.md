# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.party.organization.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/party/organization/tiinex.party.organization.v1.schema.md)
  - Created At: 2026-08-26 14:55:00
  - Trace: [Tiinex](../001-tiinex.trace.md)
  - Origin:
    - [relative](../001-tiinex.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 10:32:00
  - Authors: Anchor; Sigma
  - Why: Give a new CEO, contributor, reviewer, or blank LLM one bounded current read of Tiinex before they descend into initiative, role, financing, or implementation detail.
  - Summary: Executive grounding for what Tiinex is, why it exists, where it is now, what resources and limits are known, and which claims remain unknown.
  - Status: draft/local

---

# Tiinex Executive Grounding

This is the five-minute organizational read of Tiinex. It is written for a CEO, contributor, reviewer, sponsor, journalist, or LLM that should be able to understand the project without knowing Tiinex terminology first.

## What You Can Safely Say About Tiinex

**Tiinex is an open-source project for keeping the context and provenance of work readable in Markdown artifacts you own.** In simpler terms: the work should carry enough visible context that a later human or tool can understand where it came from, why it exists, what it depends on, what limits apply, and how to continue it without needing one old chat, app, or hidden memory.

Tiinex is currently in a stabilization phase called **Foundation Readiness**. Business does not claim that Tiinex is fully production-ready, commercially mature, legally incorporated as a company, fully funded, or complete across every product surface.

## Five-Minute Operating Picture

- **Problem:** important work often outlives the conversation, application state, undocumented assumptions, or tool-specific memory that explained it. The result may remain while the reasoning, dependencies, boundaries, and continuation path become difficult to recover.
- **Approach:** keep that context in readable artifacts with explicit provenance and continuity. Software can help discover, validate, navigate, repair, package, and present the material, but the explanation should not disappear when one software tool is unavailable.
- **Current audience:** people and tools that need to inspect, review, continue, or hand off work over time. Maintainers, contributors, human Viewer users, and LLM/Tooling consumers are evidenced use cases. A validated commercial buyer segment, market-size claim, pricing model, and authoritative adoption count are not established here.
- **Current state:** Foundation Readiness. Broad ordinary feature expansion is intentionally held while organizational truth, public first-contact surfaces, human comprehension, recoverability, and cold-start behavior are reconciled.
- **Product shape:** Core defines the meaning/rules of Tiinex artifacts; Tooling provides shared mechanics around them; Viewer provides the human-facing reading/navigation experience; Business carries organizational priorities, responsibilities, financing boundaries, external obligations, and manager-readable outcomes.
- **Human decision boundary:** Sigma carries explicit human judgment and acceptance where required. Anchor, Axiom, and Loom are collaboration roles/capacities. Their existence as artifacts does not prove employees, permanent holders, legal officers, or universal authority.
- **Progress:** Tiinex is past the idea-only stage. It already has a substantial public artifact/provenance model, working Tooling and recovery mechanics, public code, a demonstrated Viewer PoC, and a current Business operating model. It is not yet claimed as a fully qualified stable public product baseline.
- **Roadmap:** finish Foundation Readiness → establish a qualified public baseline and thaw ordinary development → prove a repeatable product/contributor loop → build sustainable project operation and evidence-led adoption. This is phase-gated, not a guaranteed calendar. Current execution state is resolved through Roadmap Follow from the linked work artifacts rather than copied into the Roadmap.
- **Financial position:** Tiinex is founder-led and substantial uncompensated founder work has already been invested. The founder has pledged 1000 SEK from personal funds toward the current public bounty, but the pledge is not treated as received money until receipt/payment evidence exists. Business does not establish an authoritative cash balance, budget, runway, recurring operating cost, sustainable founder compensation amount, or secured external funding. General Fund is a persistent project-funding destination with unknown balance; Bounty Fund remains purpose-bounded. Voluntary Tip Jars are support routes and must state their real recipient rather than being silently treated as project money. No PayPal, Kickstarter, GitHub Sponsors, bank-transfer, or other funding provider is currently implied as active; provider-neutral channels/campaigns remain a bounded Discovery.
- **Near-term work:** finish Foundation Readiness; close the public challenge fairly; prove that Business alone can truthfully orient a blank LLM; reconcile public first-contact surfaces; preserve strong human navigation outcomes demonstrated by the PoC; measure Tooling friction before optimizing unsupported causes; and qualify Business + Docs + Site together before the next stable recovery boundary.
- **Executive usability goal:** understanding and directing Tiinex should work from ordinary repository/web/LLM surfaces, including on mobile. A local IDE, terminal, or remote PC is an escalation path for implementation or deep technical inspection, not a prerequisite for understanding the organizational picture.

## Plain-English Tiinex Terms

- **Artifact:** a readable file carrying information together with enough context to interpret and continue it.
- **Provenance:** the visible trail around information — where it came from, why it exists, what changed, what it depends on, and what limits apply.
- **Parent / lineage:** the explicit path from a detailed artifact toward the broader context it continues. Folder location alone does not define that relationship.
- **Foundation Readiness:** the current stabilization gate before broad ordinary feature development resumes.
- **Workspace:** a working surface — a place where work is opened, continued, or handed over.
- **Discovery Follow:** a bounded way to keep observing the current state of one outcome across its natural sources. It avoids copying every technical detail into Business merely so an executive can see status.

## Why This Matters

A later reader should not have to reconstruct important context from repository archaeology, a months-old conversation, a particular AI provider, or somebody's memory before they can understand a piece of work.

The Tiinex vision is therefore not simply “store Markdown.” It is to make provenance and continuity a normal readable property of the work itself. Tools and interfaces can improve the experience, but the durable explanation remains inspectable and portable.

AI/LLM workflows are useful consumers and strong pressure tests for this idea because hidden or missing context quickly changes model behavior. They are not the identity boundary: Tiinex should remain meaningful for human-to-human review and continuation as well.

## What Exists Today

Tiinex has four coordinated areas:

- **Core** — the artifact/provenance semantics: how lineage, policies, schemas, relations, coordination, and interpretation boundaries are represented coherently.
- **Tooling** — shared operational mechanics such as discovery, validation, integrity/repair, recovery/Handoff operations, projection, and evidence return.
- **Viewer** — the human-facing experience for reading, navigating, inspecting, and interacting with Tiinex material.
- **Business** — the organizational view: priorities, roles/responsibility boundaries, financing, external obligations, risks, and manager-readable outcomes.

Detailed technical work belongs near the implementation or semantics it changes. Business should explain why that work matters organizationally and how to follow it upward, not duplicate every software task.

Tiinex is **not** one Viewer, one command-line tool, one schema repository, an autonomous agent framework, a general-purpose AI runtime, or a claim that every Markdown file is automatically a Tiinex artifact.

## Maturity And Product Evidence

Tiinex is **past the idea-only stage but not yet at a fully qualified stable public baseline**. That distinction is now recorded in [Current Progress And Maturity](../initiatives/001-4-current-progress-and-maturity.trace.md) rather than being inferred from repository size or development history.

A human-observed Viewer proof of concept demonstrated useful comprehension outcomes: recognizable workspaces and artifact patterns, separate Feed/Tree/Lineage views, progressive disclosure, visible current/degraded states, and the ability to follow Parent/lineage from detailed work toward wider project and organizational context.

That PoC is **evidence of product value and interaction patterns**, not authority for the current runtime or semantics. The current implementation may recover, improve, or explicitly reject an old behavior with reason. Important human value should not disappear silently merely because a refactor is technically cleaner.

Current maturity is uneven by surface: Core semantics are a working substantial foundation; Tooling is operationally useful with uneven companion/qualification coverage; Viewer value is demonstrated but the current Site baseline still has qualification/release risks; Business is a coherent foundation candidate; public open-source operation and financial sustainability are not yet fully established.

## How Work Is Organized

Business records the management-level picture: intended outcome, priority, dependency, responsibility/Role boundary, risk, external obligation, and the condition for calling work done. Code-level and schema-level subtasks belong in the repository/workspace where that work naturally lives.

A **Parent** link gives a human-readable path from detailed work back to its wider context. This lets a developer work locally without needing Business to mirror every technical subtask, while still allowing an executive or later reader to climb toward the organizational reason for the work.

A **Workspace** is where work happens. Business should not create many Workspaces just to collect status.

When ongoing status observation is useful, a **Discovery Follow** can be attached to an outcome/Epic and inspect only the declared scope. A separate Research artifact is useful when there is a real research question worth preserving; it is not a ritual step before every Follow.

Discovery reports observations. It does not automatically declare work completed. Stronger conclusions still belong in the appropriate evidence, validation, decision, or acceptance artifact.

## Roles And Human Decision Boundary

Current declared collaboration capacities are:

- **Sigma** — human structural judgment, priority, observation, feedback, bias probing, and explicit human acceptance where required.
- **Anchor** — architecture, cross-role coherence, review, and continuity.
- **Axiom** — schema recovery/design and semantic reconciliation when a demonstrated gap exists.
- **Loom** — shared/portable Tooling implementation and qualification within bounded authority.

These are organizational roles/capacities, not evidence of employees, headcount, permanent holders, legal representation, or governance rights. Important acceptance and authority must be explicit in the artifact that owns that truth rather than inferred from conversational role names.

## Resources, Financing, And Constraints

Known organizational resources include the Tiinex Business, Docs, and Site repositories/workspaces; current Tiinex Tooling; public GitHub material; canonical Docs semantics; and the declared Role capacities above.

Known financial truth is intentionally narrow but now has a clearer provenance model. The Bounty Fund lineage still records its resource state as **unknown**. The public challenge records a **1000 SEK** commitment with a 2026-09-01 deadline/closing condition and required fair closure process. A separate contribution artifact records that the founder has **pledged 1000 SEK from personal funds** toward that payout; no receipt/custody/payment is inferred from the pledge.

The founder also reports several months of concentrated Tiinex work and accepts an initial uncompensated period to continue the project. Indefinite unpaid full-time work is not treated as sustainable runway. The first material funding need is therefore predictable dedicated founder capacity, followed by explicit delivery resources when real needs exist.

Business does not currently provide an authoritative total balance, operating budget, runway, recurring cost base, salary/compensation amount, secured funding, or tax liability. [Funding Readiness And Financial Provenance](../financing/001-2-funding-readiness-and-financial-provenance.trace.md) defines how contributions, invoices, receipts, allocations, derived balances, and tax estimates should remain distinguishable without pretending Business is already certified accounting.

## Current Priorities And Foundation Exit

Current work is deliberately narrow:

- complete Foundation Readiness and keep the operating picture understandable to a non-technical manager;
- close the public challenge/bounty fairly and preserve the result/payout provenance;
- complete the Business repository-only cold-start gate using truly isolated LLM tests;
- reconcile GitHub/repository/site first-contact surfaces with current provenance;
- preserve or recover the strong human navigation and lineage-comprehension outcomes demonstrated by the PoC;
- measure Tooling iteration friction before claiming causes or optimizing unsupported theories;
- qualify Business + Docs + Site together before declaring the next stable recovery boundary.

Broad unrelated Core/Tooling/Viewer feature expansion, speculative schemas created only for organizational neatness, and arbitrary test proliferation/deletion remain on hold.

Foundation is ready to thaw only when the organization is understandable and truthful from Business, public projections agree with current provenance, external obligations are closed, human-product and Tooling quality are evidence-bounded, repository-only cold start works without hidden pre-context, the three-workspace recovery boundary qualifies, and Sigma accepts the result.

## Known Unknowns — Do Not Guess

Business currently does **not** establish:

- authoritative cash balance, budget, runway, recurring operating cost, or secured financing;
- permanent staffing/headcount, employment relationships, or guaranteed Role availability;
- reliable calendar delivery dates, detailed 6–18 month estimates, or funded capacity assumptions beyond the current phase-gated roadmap;
- validated commercial segmentation, pricing/revenue plan, market-size claim, or authoritative current user/adoption count;
- production/release qualification for every Tiinex surface;
- complete schema/runtime companion coverage in Tooling or Viewer;
- finished public contribution, security/support, governance, and funding guidance across the organization;
- long-term adoption or commercial-sustainability success metrics.

A reader or LLM should state these as unknown or undeclared rather than filling them with plausible assumptions.

## Read Deeper / Verify

- Organization root: [Tiinex](../001-tiinex.trace.md)
- Current progress/maturity: [Tiinex Current Progress And Maturity](../initiatives/001-4-current-progress-and-maturity.trace.md)
- Roadmap: [Tiinex Roadmap](../initiatives/001-5-roadmap.trace.md)
- Current roadmap roll-up: [Tiinex Roadmap Follow](../initiatives/001-5-1-roadmap-follow.trace.md)
- Current Foundation gate: [Foundation Readiness And Operating Reconciliation](../initiatives/001-6-foundation-readiness-operating-reconciliation-task.trace.md)
- Current Business-repository workbench: [Tiinex Business Development](../business-development/001-business-development-project.trace.md)
- Repository-only LLM acceptance: [Business Repository-Only Cold-Start Acceptance](../initiatives/001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
- Product areas: [Initiatives](../initiatives/001-initiatives.trace.md), [Core](../initiatives/001-1-core-project.trace.md), [Tooling](../initiatives/001-2-tooling-project.trace.md), [Viewer](../initiatives/001-3-viewer-project.trace.md)
- Responsibility boundaries: [Roles](../roles/001-roles.trace.md)
- Financial truth: [Financing](../financing/001-financing.trace.md), [Funding Readiness And Financial Provenance](../financing/001-2-funding-readiness-and-financial-provenance.trace.md), [Sustainable Dedicated Founder Capacity](../financing/001-2-1-sustainable-founder-capacity-resource-need.trace.md), [Tiinex Bounty Fund](../financing/funds/bounty/001-1-1-bounty-fund.trace.md), [Founder Bounty Contribution Pledge](../financing/funds/bounty/001-1-1-2-founder-bounty-contribution-pledge.trace.md), [Tiinex General Fund](../financing/funds/general/001-1-2-general-fund.trace.md), [Voluntary Support And Tips](../financing/001-3-voluntary-support-and-tips.trace.md), [Funding Channels And Campaigns](../financing/001-4-funding-channels-and-campaigns-discovery.trace.md)
- External obligation: [Public Challenge Closure And Bounty Decision](../initiatives/001-7-1-public-challenge-closure-and-bounty-decision-task.trace.md)
- Public LLM first contact: [Repository LLM Cold-Start And Bootstrap Surface](../initiatives/001-8-1-repository-llm-cold-start-and-bootstrap-surface-task.trace.md)

## Interpretation Limits

This artifact is an executive synthesis of current Business authority. It is not legal advice, accounting, a product-release claim, or a substitute for the linked provenance. If a more specific current artifact disagrees with this synthesis, inspect that artifact and correct this summary rather than treating the summary as competing authority.
---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex](../001-tiinex.trace.md)
  - Value: p4YGHsMqWThhcRwqAOWh1RznaqBKd_pndsSvDXyZycQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:esDgVwGISDuNI5sPxe0oxKlDS3YEwKsVlV-XSY8KCs8
