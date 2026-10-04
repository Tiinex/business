# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/8145c280093dff5d0b67db2aa72d5f5c12b6c7cb/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.party.organization.v1](https://github.com/Tiinex/docs/blob/d0e2b274558c2ee931c84318e4b84411a9da3265/.topics/.schemas/party/organization/tiinex.party.organization.v1.schema.md)
  - Created At: 2026-08-26 14:55:00
  - Trace: [Tiinex](../001-tiinex.trace.md)
  - Origin:
    - [relative](../001-tiinex.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Authors: Anchor; Sigma
  - Why: Give reusable organizational behavior an artifact-native home where lineage shape can carry more of the process than explanatory prose.
  - Summary: Business process catalog root for reusable Tiinex process definitions and their Workspace-local process directories.
  - Status: ready/local

---
# Processes

## Current Read

This artifact is the Business-local process catalog root for reusable Tiinex process definitions. Direct process-definition roots use this artifact as their real Parent when that ancestry is truthful, while each process owns a dedicated subdirectory under `.topics/processes/<process-handle>/`.

Process definitions describe reusable operating shapes. Real Projects, Tasks, Decisions, Discovery, Handoffs, Evidence, and other work remain authoritative about what actually happened. A process artifact is therefore not an execution log, workflow-engine state, or proof of conformance.

## Placement Convention

- Keep the Workspace-local process catalog/root artifact directly beneath `.topics/processes/`.
- Give every reusable process its own subdirectory beneath `.topics/processes/<process-handle>/`.
- Keep the process-definition root and its ordinary steps/branches inside the owning process directory.
- Give a true independently followable sub-process its own nested directory only when that semantic boundary is useful; folder nesting alone does not manufacture Parent continuity.
- Viewer/tooling should discover process material from artifacts rather than requiring a manually maintained README/index.

## Applicability Boundary

Process inventory does not establish process applicability. A work artifact, Entry grounding contract, qualified Decision, specialized domain process, or other semantic authority must identify the process that applies. When applicability is uncertain, preserve that uncertainty rather than selecting a process by filename or directory proximity.

## Current Process Families

- `work-lifecycle/`: outer lifecycle for spawning, placing, executing, following, accepting, landing, and reducing work.
- `session-grounding-and-continuity/`: Tiinex-specific readiness/Role profile composed with separately selected portable session-grounding material.
- `development-and-acceptance/`: reusable develop/verify and acceptance-return process.
- `accepted-change-landing/`: reusable landing and landed-state verification process.
- `human-mediated-external-execution/`: bounded human-operated external execution boundary.
- `bounded-generative-visual-source-production/`: bounded generative source/freeze/derive/review process.

Workspace-local process authority may also exist under another Workspace's own `.topics/processes/` root when that Workspace owns the governed domain, as Docs does for Schema Development.
---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex](../001-tiinex.trace.md)
  - Value: ktyPg8Ak50TwtAgUsEWAaM2Dejwhv0RY49fT8AkCwRg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: xpTqB9Rfn0HDs-IWaFLmc62f7OSnYKubfmZSqnoM2ec