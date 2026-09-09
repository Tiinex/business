# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-09 14:17:46
  - Trace: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Origin:
    - [relative](../001-turn-2-stable-full-source-frontier.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-09 15:45:03
  - Authors: Anchor
  - Why: Keep cross-repository intent in Business while moving executable Tasks/Subtasks into each owning repository.
  - Summary: Provider, Verse and Interop repository decomposition under the controlling Turn-2 epic.
  - Status: active/local

---

# Turn 2 repository decomposition frontier

## Objective

Establish repository-owned implementation frontiers for provider, Verse and Interop responsibilities while preserving one controlling Refactor integration frontier.

## Operating Boundary

Business owns the cross-repository objective and progress visibility. Each implementation repository owns its own Task/Subtask lineage, qualification evidence and returned source. Repository-local workers should not need to mutate Business to perform their scoped work.

## Current Repository Families

- Providers: Native and GitHub are first-party provider implementations over provider-neutral Core/App contracts.
- Verses: Native, Atlas and Playthings are independently versionable presentation frontiers over shared App/Universe/Workspace mechanics.
- Interop: generic provider-agnostic bootstrap/capability contracts live in Interop; OpenAI-specific environment grounding and adaptations live in Interop OpenAI.

## Stability Direction

Each repository should be independently understandable, package/release ready when distribution applies, and traceable back to this Business frontier without copying cross-repository implementation into Business.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Value: J7eMDpiRtxZpCqeB-lUxH-EtODAqs4XIYFcndqClJnI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: FSTPBfQmP7ZXOwuLt5OxiGGRIC7uF4WtwqPKJO54Dzw