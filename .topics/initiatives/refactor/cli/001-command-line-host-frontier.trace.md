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
  - Created At: 2026-09-09 18:20:58
  - Authors: Anchor
  - Why: Establish CLI as an independently evolvable host without duplicating shared mechanics.
  - Summary: Dedicated CLI host over public Core/Runtime/Provider/Interop contracts.
  - Status: ready/local

---

# Command-line host frontier

## Objective

Establish `Tiinex/cli` as the thin first-party command-line host over public Core, Runtime, Provider and Interop contracts without turning CLI into a second implementation core.

## Boundary

- CLI owns command-line operator experience and composition.
- Core owns portable artifact, validation, lineage, Handoff and package mechanics.
- `runtime-native` owns portable execution/orchestration when runtime behavior is required.
- Providers own source/material access.
- Interop owns external environment/capability integration.
- CLI must not introduce provider-, OpenAI-, VS Code- or browser-specific branches into shared contracts.

## Turn-2 direction

Create a minimal package/release-ready repository with repo-local Task/Subtasks. Implement only the command surfaces needed by qualified operator workflows, prioritizing reuse of the existing portable Tooling path rather than duplicated command implementations.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Value: J7eMDpiRtxZpCqeB-lUxH-EtODAqs4XIYFcndqClJnI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: JhilZJBE9iabLvOhmc8s8Ky20N7t25C3B1YLxkIvKoA