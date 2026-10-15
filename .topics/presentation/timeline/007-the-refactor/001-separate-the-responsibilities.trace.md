# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:43
  - Trace: [001-1-1-courier-before-the-formal-package.trace.md](../006-video-as-continuity/001-1-1-courier-before-the-formal-package.trace.md)
  - Origin:
    - [relative](../006-video-as-continuity/001-1-1-courier-before-the-formal-package.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:44
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: September responsibility split informed by practical monolith scaling and continuity limits, alongside other pressures.
  - Status: approved-for-publication

---

# Separate source, host, Tooling and ownership

The major refactor was informed by the **limit-seeking PoC experiment**: a ChatGPT Web-driven monolith could accumulate impressive functionality, but that did not mean its implementation remained easy to scale, revise or continue across sessions. The practical question shifted from *how many more features can we add?* to *which responsibilities must survive independently so future work remains possible?*

The answer was not to discard the experiment. It was to untangle it. In September, repository boundaries became visible in project decisions and implementation: different modules could evolve or be replaced without forcing one UI or host to own every artifact's meaning.

This is the later **major refactor**, not the first code cleanup or the invention of every boundary at once. Earlier experiments with schemas, traceable tools, viewers and handoff-like mechanisms were already under way. Likewise, the monolith's development pressure was one important motivation, not an independently established single cause for every subsequent design decision.

## Direct artifact anchors

- [September repository/bootstrap responsibility-boundary decision](https://github.com/Tiinex/business/blob/e6fc1ebb01b756129a8befd6bb1c8572d728859f/.topics/initiatives/001-3-6-4-1-repository-bootstrap-responsibility-boundary-decision.trace.md) — inspectable project decision about separating responsibilities, rather than just a commit listing.
- [Earlier June application LLM-orientation document](https://github.com/Tiinex/site/blob/cc4acebf4a0603ca50bca2bbce375bb3e8d00f77/tiinex.app.llm.v1.md) — illustrates the earlier Site-centered application surface against which the later separation can be understood.

## Reader's mental model

Think in responsibilities, not marketing modules: Docs defines canonical semantic contracts; Business holds project intent, human gates and Roles; Core supports shared host-neutral Tooling; viewers and host adapters present or operate on qualified information. Real authority comes from the actual qualified artifact and its contract, not the name of the repository containing a file.

## What remains open

Splitting repositories does not automatically repair conversational context loss, prove implementation/schema parity or make every host interoperable. Those are separate questions for qualification, grounding, test evidence and Handoff design. The refactor made it more practical to tackle them without returning to one monolithic owner of everything.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-courier-before-the-formal-package.trace.md](../006-video-as-continuity/001-1-1-courier-before-the-formal-package.trace.md)
  - Value: lfoCzPxqrhIC-UG1TyvX6hjPDWo58NdyTpW_KAyAq3A

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: gAFnjQzH_puOQypGZktC9QjcvEj-N_c3wYwfb_JOdJ8
