# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-04 22:58:46
  - Trace: [010-repair-stage-all-workspaces-command-registration-task.trace.md](010-repair-stage-all-workspaces-command-registration-task.trace.md)
  - Origin:
    - [relative](010-repair-stage-all-workspaces-command-registration-task.trace.md)
- Current
  - Current Schema: [tiinex.relation.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/relation/tiinex.relation.v1.schema.md)
  - Created At: 2026-10-04 22:59:51
  - Authors: Anchor
  - Why: Keep the final hotfix transfer explicit without broadening the stable-Major scope.
  - Summary: Select the existing grounding and recipient guidance for the bounded Stage All command registration hotfix.
  - Status: ready/local

---

# Stage All Command Hotfix Grounding Applicability

## Relation Declaration

- Relation Type: session grounding applicability bundle
- Relation Direction: selected guidance set -> bounded current work
- Relation Scope: final VS Code Stage All command registration hotfix and Sigma acceptance

## Relation Target

- Target: [Repair Stage All Workspaces Command Registration Before Stable Major](010-repair-stage-all-workspaces-command-registration-task.trace.md)
  - Relation Type: applicability target
  - Relation Direction: selected guidance -> controlling Task
  - Relation Scope: current hotfix
- Target: [Portable Session Grounding And Continuity](native::.topics/.processes/session-grounding-and-continuity/001-session-grounding-and-continuity-process.trace.md)
  - Relation Type: selected portable guidance member
  - Relation Direction: applicability bundle -> portable process authority
  - Relation Scope: recipient transfer and recovery
- Target: [Tiinex Session Grounding And Continuity Profile](../processes/session-grounding-and-continuity/001-session-grounding-and-continuity-process.trace.md)
  - Relation Type: selected Tiinex guidance member
  - Relation Direction: applicability bundle -> Tiinex profile
  - Relation Scope: Anchor/Sigma acceptance

## Relation Boundary

- This Relation establishes guidance applicability only.
- Relation targets are not Parent, and this Relation establishes no Parent ancestry among the Task or guidance artifacts.
- It does not establish Build success, acceptance, Task completion, or mutation authority.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [010-repair-stage-all-workspaces-command-registration-task.trace.md](010-repair-stage-all-workspaces-command-registration-task.trace.md)
  - Value: ku3HQx5pun22FM0kiclMfNHVMx8PL0Se5h3Q0te5K3U

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 6hBiI9uJnsALXzVxW87BoykwHFAD3yZI3p5dPq8BAh4