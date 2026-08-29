# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Business Development](001-business-development-project.trace.md)
  - Origin:
    - [relative](001-business-development-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Operating Model And Portfolio Structure
  - Status: accepted/local

---

# Operating Model And Portfolio Structure

## Objective

Maintain the minimal professional Tiinex operating structure: one organization root, bounded Roles and Projects, manager-readable work packages, truthful cross-repository context, and recoverable continuation without turning Business into a technical task tracker.

## Done Criteria

- Business exposes stable organizational anchors without becoming a central implementation task store.
- Core, Tooling, and Viewer have bounded Project roots with only the work packages needed to explain current or next organizational outcomes.
- A human developer can start from local current work, understand the outcome and Done boundary, and follow truthful Parent context upward when more explanation is needed.
- Stale intermediate decisions, handoffs, validation reports, and superseded orchestration material do not dominate current HEAD when Git history is the appropriate recovery boundary.
- Anchor continuation can be reconstructed from durable current artifacts and a qualified Handoff rather than conversation memory.

## Scope

- Business and portfolio structure only; do not implement product subtasks here.
- Prefer a small number of meaningful durable anchors over corporate-style taxonomy.
- Preserve historical corpora and explicit current-frontier decisions.

## Dependencies

- Current Business coordination decision and consolidated Roles.
- Discovery across Business, Docs, and Site.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Business Development](001-business-development-project.trace.md)
  - Value: dxtfDTU66MwQI1ezqdpysgc1grW7UMmHOkoFRHyW3co

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 6szv3sF87vzGXGZc5wjmlrRrY-CXj-bXEXb6jC9cUts
