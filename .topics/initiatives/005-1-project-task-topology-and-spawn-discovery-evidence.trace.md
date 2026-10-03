# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-03 21:49:10
  - Trace: [005-project-work-topology-rollout-and-current-spawn-repair-task.trace.md](005-project-work-topology-rollout-and-current-spawn-repair-task.trace.md)
  - Origin:
    - [relative](005-project-work-topology-rollout-and-current-spawn-repair-task.trace.md)
- Current
  - Current Schema: [tiinex.evidence.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/evidence/tiinex.evidence.v1.schema.md)
  - Created At: 2026-10-03 21:49:47
  - Authors: Anchor
  - Why: Bound the migration before any implementation lineage is resumed.
  - Summary: Qualify reuse of existing Project/Task schemas, the Work Lifecycle refinement, and the remaining current cross-repository ancestry repair.
  - Status: ready/local

---

# Project/Task Topology And Spawn Discovery Evidence

## Supported Claim Or Question

- Supported Claim Or Question: whether current Tiinex schemas/processes can support scalable Project → Project and Task → Task decomposition without new schema types, and what gap remains for interruption-safe cross-repository spawning
- Evidence Role: qualify the topology Decision and bound the immediate repair Task without starting implementation work
- Target Artifact: [Qualify Project/Task Topology And Repair Current Spawn Ancestry](005-project-work-topology-rollout-and-current-spawn-repair-task.trace.md)
- Review Context: fresh-start work modeling before deterministic lineage-maintenance implementation resumes

## Provenance

- Known Source: current carried Business, Docs, Core, and Native Workspace material in carrier `017-1-1-1-1-1-1`
- Preservation Basis: direct inspection of `tiinex.project.v1`, `tiinex.task.v1`, Business Lineage Structure Decision, Tiinex Work Lifecycle, Business Projects 003/004, Native Task 001, and Core Task 001/001-2
- Provenance Limits: the Business Projects in the current carrier are not assumed published merely because they are carried locally; immutable cross-repository Parent repair therefore remains gated on the next pushed Business revision

## Evidence Material

- Material: the current Project schema defines a bounded coordinated effort and preserves Parent as direct continuity ancestry; the Task schema explicitly supports Subtasks and one bounded executable unit of work; current Business Lineage Structure already says repository boundaries preserve semantic Parent while filename dimensions remain local; the pre-refinement Work Lifecycle required real Parent continuity but did not enforce publish-before-child cross-repository spawning; the carried Work Lifecycle now makes that interruption-safe ritual explicit; Business Project 003 currently follows Native Task 001 only through coordination while Native Task 001 Parents to a local Native Decision; Business Project 004 currently follows Core Task 001 only through coordination while Core Task 001 has no Parent.
- Material Kind: current-state semantic/schema/process audit and bounded migration-gap evidence
- Schema Reuse Finding: no separate Subproject or Subtask schema is required for the desired topology; Project → Project and Task → Task are representable with current schemas and Parent continuity.
- Spawn Gap Finding: current authoring correctly requires exact immutable recovery for cross-Workspace Parent; this carrier closes the process-side gap by explicitly requiring publish-before-child and forbidding provisional parentless implementation work.
- Current Debt Finding: Business Projects 003/004 are the intended governing outcomes, but their Native/Core root Tasks are not yet direct semantic descendants of those Business Projects.

## Preservation And Fidelity

- Preservation State: no implementation lineage mutation is performed by this Evidence
- Fidelity Notes: Workspace placement, filename dimension, Project hierarchy, Task decomposition, and semantic Parent are treated as distinct projections
- Known Losses: none

## Interpretation Limits

- Not Yet Used As: proof that Business Projects 003/004 are immutable published Parent authority
- Does Not Prove: that every future Tiinex work item requires a Project; Project remains a meaningful outcome boundary, not mandatory grouping
- Must Not Be Treated As: authority to create parentless repository work before the publication gate or to begin lineage-maintenance/schema-extraction implementation before current ancestry repair

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [005-project-work-topology-rollout-and-current-spawn-repair-task.trace.md](005-project-work-topology-rollout-and-current-spawn-repair-task.trace.md)
  - Value: omoMbziiaeFBfla9vcO_XR704ZWSXhnQopCe--1QffU

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: vLxtWvCVgabHo_BCIW6H2GKXJkyBtVW-oM4RcOZPvoU