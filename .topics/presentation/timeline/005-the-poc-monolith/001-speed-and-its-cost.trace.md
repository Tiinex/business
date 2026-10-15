# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:38
  - Trace: [001-1-1-1-1-1-1-the-viewer-becomes-its-own-lens.trace.md](../004-tooling-and-viewers/001-1-1-1-1-1-1-the-viewer-becomes-its-own-lens.trace.md)
  - Origin:
    - [relative](../004-tooling-and-viewers/001-1-1-1-1-1-1-the-viewer-becomes-its-own-lens.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:39
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: An intentional limit-seeking ChatGPT Web monolith experiment: rapid feature growth until scaling and continued development became unsustainable.
  - Status: approved-for-publication

---

# How far can a monolith go when the development environment is a chat?

The proof of concept was not simply an application that accidentally grew too large. **The developer deliberately kept adding features to an increasingly monolithic Viewer while building through ordinary ChatGPT Web conversations.** The point was exploratory: find out how far this way of working could be pushed before adding capabilities, scaling the implementation, and even continuing the work became unsustainable.

This was a practical **limit-seeking experiment**, not a controlled benchmark with a predefined feature count or a measured failure threshold. It tested two things at once: what a working application could acquire quickly with LLM assistance, and how much complexity a conversational development workflow could carry before its overhead outweighed its speed.

## The experiment as remembered by its developer

1. **Keep shipping capabilities.** Instead of starting with a cleanly separated product architecture, work rapidly on a functional proof-of-concept Viewer. Try different artifact views, source-handling and interaction ideas, and keep extending what the working system can demonstrate.
2. **Develop primarily through ChatGPT Web.** The switch away from VS Code/Copilot was partly economic: ongoing token and subscription costs had become difficult to sustain. A flat-rate conversational interface made prolonged experimentation more accessible, but the conversation itself was not a dependable durable project environment.
3. **Observe where iteration breaks down.** A feature-rich monolith can still run while becoming increasingly costly to understand, revise, test and hand to a new session. The developer's report is that the system reached a point where **scaling and continuing development felt untenable**.
4. **Treat that limit as a finding.** The later architectural separation was a response to real pressure encountered during this style of development, not evidence that the ideal module boundaries were known from the beginning.

The outcome was simultaneously a useful, working PoC **and** a warning that adding more functionality is different from preserving the ability to continue building. The experiment exposed development-continuity problems alongside software-structure problems; it did not establish that ChatGPT Web has a universal maximum project size.

## Inspectable source anchors

- [Early Lineage Viewer and LLM-facing application orientation, June 19](https://github.com/Tiinex/site/blob/cc4acebf4a0603ca50bca2bbce375bb3e8d00f77/tiinex.app.llm.v1.md) — shows the existing application ambitions and explicit interface/orientation concerns.
- [Application state runtime during continued Site development](https://github.com/Tiinex/site/blob/207668389fb16f416c752acf2beaa49baca8a399/src/app/state-runtime.js) — a commit-pinned source file illustrating implementation evolution; **not** an exhaustive inventory of monolith features or a measured scalability result.
- [Later repository responsibility-boundary decision](https://github.com/Tiinex/business/blob/e6fc1ebb01b756129a8befd6bb1c8572d728859f/.topics/initiatives/001-3-6-4-1-repository-bootstrap-responsibility-boundary-decision.trace.md) — evidence of explicit boundaries adopted during the later refactor, not proof of the exact point at which the earlier experiment became unsustainable.

## What this chapter can and cannot establish

- **Firsthand account:** an intentional push to fit many capabilities into a ChatGPT Web-driven monolith, a quickly working PoC (approximately two weeks by recollection), and a practical limit to continued development and scaling.
- **Dated GitHub artifacts:** Site code and interface material existed and changed over time. They corroborate development activity, **not** the exact failure threshold or every reason the developer chose to refactor.
- **Interpretation:** the experience motivated a stronger separation between durable source, user-facing views, Tooling and conversational sessions. It is not a controlled comparative study of AI development platforms.

**Question to carry forward:** if an experiment can build features faster than it can preserve the knowledge needed to change them, where should continuity actually live?

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-1-1-1-1-the-viewer-becomes-its-own-lens.trace.md](../004-tooling-and-viewers/001-1-1-1-1-1-1-the-viewer-becomes-its-own-lens.trace.md)
  - Value: VNm-cWzFAsgY3-pzWHJ31QZjyyzJHOwX7n0QPZ-yjdA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: e5dee0gidRiP-PlSBsKXzhcdFIHcic8sN76Fe5paqQ8
