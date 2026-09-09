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
  - Created At: 2026-09-09 16:47:25
  - Authors: Anchor
  - Why: Create the durable runtime architecture and work lineage now while deferring speculative execution implementation until shared contracts are stable.
  - Summary: First-party host-neutral runtime frontier for grounded execution over Core, Providers and Interop.
  - Status: ready/local

---

# Portable Tiinex Runtime

## Objective

Establish a first-party portable runtime that can be hosted by VS Code, CLI, services or future hosts without embedding provider, environment or host-specific behavior.

## Runtime model

`runtime-native` orchestrates grounded Roles, Tasks, execution state, capability resolution, Handoff-aware workflows, interruption/recovery and execution evidence. Hosts execute the runtime; Providers resolve source/material; Interop exposes external environment capabilities.

## Turn-2 boundary

Create the durable repository/task frontier and public package/release readiness now. Do not invent a large runtime implementation until Core, Interop, Provider and host contracts are sufficiently stable to keep the runtime portable.

## Initial workstreams

- execution model and lifecycle
- grounded Role/Task loading
- capability discovery/resolution
- provider and Interop consumption boundaries
- Handoff transition and recovery
- trace/evidence production
- host-neutral qualification
- future VS Code native-chat bridge as an extension-vscode task, not a VS Code-specific runtime

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Value: J7eMDpiRtxZpCqeB-lUxH-EtODAqs4XIYFcndqClJnI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: J4YII_DXdQ1anoBAkyui3bUot3tX6ClP5IFJVtBxILY