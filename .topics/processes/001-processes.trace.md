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
  - Created At: 2026-08-29 16:07:00
  - Authors: Anchor; Sigma
  - Why: Give reusable organizational behavior an artifact-native home where lineage shape can carry more of the process than explanatory prose.
  - Summary: Proposed Processes branch for artifact-native process definitions and their observable topology.
  - Status: proposed/local

---

# Processes

## Current Read

This proposed branch tests whether Tiinex processes can be represented primarily by artifact lineage: descendants express progression, siblings express alternative branches, and typed non-parent relations express returns or other graph edges that must not become `Parent`.

## Design Direction

Keep process definitions small and inspectable. A process definition describes an intended reusable shape; real work keeps its own real schemas and lineage. Execution is not required to reproduce a process tree mechanically, and variation is not automatically failure.

## Next Artifacts

The first representation experiment is Development And Acceptance. This branch is not yet a claim that Tiinex has settled a universal Process schema, process-step schema, workflow engine, or conformance model.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex](../001-tiinex.trace.md)
  - Value: p4YGHsMqWThhcRwqAOWh1RznaqBKd_pndsSvDXyZycQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: -dIbKFmhRYlDVjL-4TkCoeb6KCK-5wH6l4U8zsPgj8s
