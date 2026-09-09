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
  - Created At: 2026-09-09 16:47:23
  - Authors: Anchor
  - Why: Keep extension hosts independently evolvable without ambiguous repository identity or host-specific authority leakage.
  - Summary: VS Code and Chrome extension hosts with explicit repository identities and shared-contract boundaries.
  - Status: ready/local

---

# Extension repository frontier

## Objective

Keep editor/browser integrations explicit as extension hosts rather than ambiguous repository names or forks.

## Repository identities

- `Tiinex/extension-vscode` is the current repository identity for the VS Code host previously carried as `Tiinex/vscode`.
- `Tiinex/extension-chrome` is the Chrome host frontier.

## Boundary

Extensions consume public Core, App, Runtime and Interop capabilities as needed. They do not become semantic authority, copy shared implementation, or absorb environment-specific Interop behavior simply because they can host it.

## Turn-2 direction

Repository-local Tasks own the implementation and qualification work. Business keeps only the controlling cross-repository continuity and progress boundary.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Value: J7eMDpiRtxZpCqeB-lUxH-EtODAqs4XIYFcndqClJnI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: aLvz6PeBPza3P9sjr3c4OmNe878LlAAFAQTjmm402uQ