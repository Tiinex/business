# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Trace: [001-processes.trace.md](../001-processes.trace.md)
  - Origin:
    - [relative](../001-processes.trace.md)
- Current
  - Current Schema: [tiinex.process.v1](https://github.com/Tiinex/docs/blob/2262a1c4b35e887d116d0d01a864074a9f1641c2/.topics/.schemas/process/tiinex.process.v1.schema.md)
  - Created At: 2026-10-03 19:28:08
  - Authors: Anchor; Sigma
  - Why: Prevent new work from inventing incompatible creation, execution, follow-up, and closure conventions.
  - Summary: Reusable outer lifecycle for spawning, owning, executing, following, accepting, landing, and reducing Tiinex work.
  - Status: ready/local

---

# Tiinex Work Lifecycle

## Process Identity

- Name: Tiinex Work Lifecycle
- Version: 1
- Canonical Identifier: tiinex.process.work-lifecycle.v1
- Human Label: Tiinex Work Lifecycle

## Purpose And Scope

- Purpose: Provide one reusable lifecycle for turning an observed need into bounded Tiinex work, executing it through the applicable process, following it from the organizational boundary without duplicating implementation truth, and reducing terminal history when the current frontier is settled.
- Semantic Boundary: Defines reusable Tiinex Work Lifecycle process semantics; it does not prove invocation, execution, authority, acceptance, current work, or completion.
- Intended Domains: qualified Tiinex work for the Tiinex Work Lifecycle process
- Not Intended For: inferring applicability from carriage, directory placement, filename order, Role presence, or host presentation

## Applicability And Conditions

- Applicability Meaning: applicable only when a qualified Entry, Handoff, controlling work artifact, relation, invocation, or other owning authority selects this reusable Process for the bounded work.
- Unknown Meaning: if applicability, authority, entry, or governing work is unresolved, Process applicability remains unresolved rather than being inferred from discovery or proximity.

## Process Topology

- Topology Meaning: typed Transition Definitions and qualified Relations in this Process lineage define reusable positions and durable non-parent topology where represented.
- Entry Meaning: Process entry is established by qualified invocation/context and typed topology; semantic Parent and filename order do not independently select an executable entry.
- Outcome Meaning: outcomes are established by qualified topology plus real execution/return/evidence artifacts; Process definition presence does not establish an outcome.
- Transition Family: work-lifecycle

## Interpretation Limits

- Does Not Prove: that this Process ran, is current, was accepted for a particular context, or grants mutation authority.
- Must Not Be Inferred: that semantic Parent, filename lineage, directory position, carrier presence, or apparent chronology is executable Process topology or current-work authority.
- Execution Boundary: typed Process topology defines reusable semantics; real work lineage, qualified invocation/context, Handoffs, Returns/Reductions, Evidence, and accepting authority remain the truth about what actually happened.

## Related Artifacts

### Preserved Legacy Definition Notes

### Purpose

Provide one reusable lifecycle for turning an observed need into bounded Tiinex work, executing it through the applicable process, following it from the organizational boundary without duplicating implementation truth, and reducing terminal history when the current frontier is settled.

### Current Read

This process is the ordinary outer lifecycle for new Tiinex work. It is not a workflow engine and does not make a process applicable merely because the process exists. A real work artifact remains authoritative about what actually happened.

Use this lifecycle to avoid session-local conventions for creating Tasks, Projects, Decisions, Discovery, or other work-bearing artifacts. The lifecycle establishes the question sequence; the selected schema, Scaffold capability, Workspace authority, and specialized Process establish the actual artifact shape.

### Composition With Existing Processes

- Ordinary implementation/development may use [Development And Acceptance](../development-and-acceptance/001-development-and-acceptance-process.trace.md).
- Accepted candidates that require an explicit landing boundary may use [Accepted Change Landing](../accepted-change-landing/001-accepted-change-landing-process.trace.md).
- Specialized work, such as Docs schema development, may bind its own qualified Process instead of duplicating that process here.
- A Process reference is grounding and an operating contract; it is not proof that execution occurred or conformed.

### Entry And Cold-start Boundary

A Session Entry may carry the applicable Process as required Grounding Material together with the current bounded work, Role material, and participating Workspaces. A cold LLM should therefore be able to recover both `what work is current` and `how that class of work is intended to proceed` without inventing a new execution convention.

### Project, Task, And Business Boundary

Follow the accepted [Project, Task, And Spawn Topology Decision](../../decisions/001-1-project-task-and-spawn-topology-decision.trace.md). Project hierarchy, Task decomposition, semantic Parent, filename dimension, and Workspace placement are distinct concerns. A Project exists only when it owns a real bounded coordinated outcome; it is not a visual grouping node. A child Project is a subproject when direct Project continuity is real. A Task is one bounded executable unit and may have Task children for subtasks without inventing a Project.

Business owns organizational why, priority, main-project outcome, and acceptance/disposition when those concerns are organizational. Implementation truth remains in the natural Workspace that owns the affected domain. Tiinex-specific development work should normally remain semantically traceable through Parent ancestry to its governing Business Project. Business follow-up should derive child work/disposition rather than copy repository implementation detail.

When that ancestry crosses repositories, durable child work is materialized only after the upstream Parent has qualified immutable published recovery. If that Parent is not yet published, checkpoint/publish the upstream spawn boundary and stop; do not create parentless implementation work or temporary durable `workspace::path` ancestry to repair later.

### Reduction Boundary

Terminal or superseded execution history should become Reduction material once it no longer needs to appear current. If unresolved work remains, preserve a short explicit frontier and spawn or continue bounded work through this lifecycle rather than leaving long historical execution lineages looking active.

### Next Artifacts

- [Establish Work Need And Boundary](001-1-establish-work-need-and-boundary.trace.md)

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-processes.trace.md](../001-processes.trace.md)
  - Value: 45zoHVoM9WjJL_ONe7kDaotO2BRdnuHnzObbSXGimc4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:sURwVt47jYrUQOQoan6vYIUEcyQXa3DdZfFo83mscFM
