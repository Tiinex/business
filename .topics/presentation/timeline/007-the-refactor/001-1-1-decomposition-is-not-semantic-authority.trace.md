# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 22:03:27
  - Trace: [001-1-an-organizational-home.trace.md](001-1-an-organizational-home.trace.md)
  - Origin:
    - [relative](001-1-an-organizational-home.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:44
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: September repository decision separates implementation ownership from schema authority.
  - Status: approved-for-publication

---

# Repositories became responsibility boundaries

Following the limit-seeking Viewer work, Tiinex was separated into more explicit repositories. A **September 9 Business decision** distinguishes *the location of implementation code* from *the authority that defines what an artifact means*.

In that responsibility map:

- `Tiinex/docs` owns maintained schemas, validators and semantic contracts.
- `Tiinex/business` owns initiative/project intent, roles and human decisions.
- `Tiinex/core` owns host-neutral mechanics and qualification/packaging tooling.
- App, host and provider packages own bounded parts of the implementation, and can be replaced without quietly redefining semantics.

## Primary source

[September repository/bootstrap responsibility decision](https://github.com/Tiinex/business/blob/e6fc1ebb01b756129a8befd6bb1c8572d728859f/.topics/initiatives/001-3-6-4-1-repository-bootstrap-responsibility-boundary-decision.trace.md).

## Avoid a false origin story

This map was *recorded after extraction/refactoring*. It does not prove that every boundary was anticipated at the beginning, nor that refactor alone solved all environment and reliability problems.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-an-organizational-home.trace.md](001-1-an-organizational-home.trace.md)
  - Value: gE23HQJgO1oYJ502Ka-Ex9Fs4E43ps8iPgRYKlopKHQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: hFlixRcBRC1WbQ8QQB6-oZfBHrBzQvhFLLhsRErlUhY
