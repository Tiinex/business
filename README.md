# Tiinex Business

Tiinex is an open-source project for keeping the **context around work readable and portable**. It stores provenance — where material came from, why it exists, what it depends on, what changed, and what should not be inferred — in readable Markdown artifacts that remain useful outside one chat, app, or AI provider.

This repository is Tiinex's current organizational surface. It explains what the project is, how far it has progressed, where it is going next, how responsibilities are divided, what financial facts are actually known, and which claims are still unknown.

## 60-second orientation

- **What problem is Tiinex solving?** Important work often survives while the reasoning and context around it disappear into chats, tools, undocumented assumptions, or private state. Tiinex aims to make that context inspectable and recoverable with the work itself.
- **How far along is it?** Tiinex is past the idea-only stage: it already has a substantial artifact/provenance model, working Tooling and recovery mechanics, public code, a demonstrated Viewer PoC, and a functioning Business provenance model. It is now consolidating those pieces into a qualified public foundation; it is not yet presented as a fully production-qualified or commercially mature product.
- **Who is it for?** The currently evidenced audience is people and tools that need to inspect, review, continue, or hand off work over time. AI/LLM use is important, but Tiinex is not defined as an AI product.
- **Where is the project now?** Tiinex is in **Foundation Readiness**: broad feature expansion is deliberately paused while organizational truth, public surfaces, human usability, recovery, and cold-start behavior are made coherent enough to trust.
- **Where is it going?** The current roadmap is phase-gated: finish Foundation → establish a qualified public baseline and thaw development → prove a repeatable product/contributor loop → build sustainable project operation and evidence-led adoption.
- **Is Tiinex a company?** This repository describes a project organization. It does not establish legal incorporation, employees, ownership, representation authority, or accounting correctness.
- **Who makes the final human calls?** Sigma carries explicit human judgment and acceptance where required. Anchor, Axiom, and Loom are declared collaboration roles/capacities; they are not proof of employees or legal officers.
- **What do we know about money?** Tiinex is currently founder-led and has substantial uncompensated founder work behind it. The founder pledged 1000 SEK from personal funds toward the public challenge bounty. Submissions are now closed and the challenge is in review/funding; the pledge is still not recorded as received or paid money until receipt/payment evidence exists. Overall cash balance, budget, runway, recurring costs, sustainable founder compensation, and secured external funding are not established and must not be guessed.
- **What would funding change?** The earliest material funding goal is sustainable dedicated founder capacity: replacing indefinite dependence on uncompensated personal availability with predictable focused project work. Later funding should attach to explicit roadmap/resource needs such as infrastructure, services, expertise, contributor support, or bounties.

## Start here

For the best first read — especially on mobile — open **[Tiinex Executive Grounding](.topics/executive/001-executive-grounding.trace.md)**. It is written as the five-minute organizational view before deeper detail.

Then choose the question you have:

- **How far have we already come?** [Current Progress And Maturity](.topics/initiatives/001-4-current-progress-and-maturity.trace.md)
- **What should happen next, and in what order?** [Tiinex Roadmap](.topics/initiatives/001-5-roadmap.trace.md)
- **How is the roadmap going right now?** [Roadmap Follow](.topics/initiatives/001-5-1-roadmap-follow.trace.md) resolves linked work without copying Epic status into the Roadmap.
- **Where are we right now?** [Foundation Readiness](.topics/initiatives/001-6-foundation-readiness-operating-reconciliation-task.trace.md)
- **What is being changed in Business right now?** [Tiinex Business Development](.topics/business-development/001-business-development-project.trace.md) is the active workbench; it keeps at most one active lineage per working Role.
- **What are the main product areas?** [Initiatives](.topics/initiatives/001-initiatives.trace.md)
- **Who/what carries responsibilities?** [Roles](.topics/roles/001-roles.trace.md)
- **What would funding enable and how should money be traceable?** [Funding Readiness And Financial Provenance](.topics/financing/001-2-funding-readiness-and-financial-provenance.trace.md)
- **Where would general project funding belong?** [Tiinex General Fund](.topics/financing/funds/general/001-1-2-general-fund.trace.md) — current balance remains unknown until real receipt/economic-party evidence exists.
- **How can someone show simple appreciation?** [Voluntary Support And Tips](.topics/financing/001-3-voluntary-support-and-tips.trace.md) keeps Tip Jars distinct from project funds and from governance/priority.
- **How could PayPal, Kickstarter, Sponsors, direct transfer, or similar routes fit without hardcoding them?** [Funding Channels And Campaigns](.topics/financing/001-4-funding-channels-and-campaigns-discovery.trace.md) is the current provider-neutral Discovery; none of those example providers is claimed active.
- **What is the current sustainability need?** [Sustainable Dedicated Founder Capacity](.topics/financing/001-2-1-sustainable-founder-capacity-resource-need.trace.md)
- **What is the organizational root?** [Tiinex](.topics/001-tiinex.trace.md)

## Financial provenance in plain language

Tiinex aims to make economic claims inspectable through the same provenance principles as the rest of the project. A promise should not silently become cash received; an invoice should not silently become a payment; an earmarked amount should not silently become free balance; and a tax estimate should not silently become a legally determined tax liability.

The intended chain is to preserve the real economic party and event — for example need, pledge/contribution, receipt, invoice/instrument, allocation, usage or payment evidence — and then derive views such as available balance or tax reserve from those records. This is an operating goal, not a claim that Business is already a certified accounting system.

## A few Tiinex terms

You do not need these terms to understand the project, but they appear in the artifacts:

- **Artifact** — a readable file that carries information together with the context needed to interpret it.
- **Provenance** — the visible trail around information: where it came from, why it exists, what changed, what it depends on, and what limits apply.
- **Parent / lineage** — the explicit path from detailed work toward its broader context. It answers “what larger thing does this continue or belong under?” without relying on folder location alone.
- **Foundation Readiness** — the current stabilization phase before broad ordinary feature development resumes.
- **Workspace** — a place/surface where work is done or taken over.
- **Discovery Follow** — a bounded way to keep observing the current state of one outcome without duplicating all underlying technical work into Business.

## Reading and authority boundary

`.topics/**` carries current Tiinex Business semantic/provenance authority. This README is the reception desk: it summarizes and routes to that material, and should be corrected if it drifts rather than treated as a competing source of truth.

Detailed technical work belongs in its natural Docs, Site, or Tooling context and should connect upward to Business when organizational context matters. Business is intentionally not a duplicate software issue tracker.

`business-development/` is likewise an **active Business-repository workbench**, not the durable organization map. It keeps at most one active lineage per currently working Role, and every surviving leaf should make sense if it appears directly in the Business Feed. Completed improvement lineages leave current HEAD after their outcomes land and role-level checks are complete; Git history keeps their provenance.

A local IDE, terminal, or remote PC may be needed for implementation or deep technical inspection. It should **not** be required merely to understand the organization, inspect priorities, or make normal executive decisions from the repository/web/LLM surface.

For a blank LLM reading this repository, [`llms.txt`](llms.txt) provides a bounded reading route and explicit “do not guess” rules.
