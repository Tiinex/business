# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 15:04:00
  - Trace: [001-business-lineage-structure-decision.trace.md](001-business-lineage-structure-decision.trace.md)
  - Origin:
    - [relative](001-business-lineage-structure-decision.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-10-03 21:48:27
  - Authors: Anchor; Sigma
  - Why: Prevent Project-as-folder drift and parentless cross-repository development work.
  - Summary: Establish scalable Project/Task/Subtask topology, Workspace-independent project structure, and interruption-safe cross-repository spawn ancestry.
  - Status: ready/local

---

# Project, Task, And Spawn Topology Decision

This Decision refines the Business lineage convention so project structure, execution lineage, Workspace placement, and Process guidance remain separate concepts rather than collapsing into one filename or folder hierarchy.

## Decision

- State: accepted
- Subject: Tiinex Project/Task topology and cross-Workspace work spawning
- Decision: A Project represents a real bounded coordinated outcome, not a grouping container. A Project may have another Project as direct Parent when the child is a genuine subproject with its own purpose/scope/outcome boundary; no separate Subproject schema is introduced. A Task represents one bounded executable unit of work and may have Task children when execution needs subtasks; Project must not be introduced merely to group Tasks. Project hierarchy is independent of Workspace topology: one Project may span one or many Workspaces, and one Workspace may carry work from many Projects. Business is an organizational Workspace and is not itself the universal Project root. Main Tiinex Projects normally live in Business when they own the cross-Workspace or organizational outcome; repository-local subprojects/tasks live in their natural owning Workspaces when they own a real bounded contribution. A `Tiinex` umbrella Project may exist only if a real umbrella project/outcome warrants it; the Organization must not be duplicated as an empty taxonomy Project.
- Spawn Ancestry: Tiinex-specific development work should normally remain semantically traceable through declared Parent ancestry to the governing Business Project. When a new child Project/Task must cross a repository boundary, the upstream Parent must first exist as qualified immutable published material. The child is authored only after that Parent can be represented with exact Parent bytes plus a commit-pinned recovery reference. A `workspace::path` selector may help runtime resolution but must never be left as durable substitute provenance.
- Interruption Safety: if the upstream Business Project is new and not yet published, stop after authoring/checkpointing the upstream spawn boundary. Do not materialize parentless implementation work "to fix later". After publish, materialize the child with the real cross-repository Parent from its first durable bytes.
- Relation Boundary: `Related Project`, `Related Task`, coordination prose, and Business follow-up are supplementary relations. They must not replace Parent when direct continuation ancestry is known and intended.

## Basis

- Current Project and Task schemas already support the necessary logical shapes: Project artifacts can continue Project ancestry and Task explicitly allows Subtasks, so new `Subproject` or `Subtask` schema types would add taxonomy without adding semantics.
- Repository/Workspace layout is an implementation ownership boundary, not a project taxonomy. Coupling one Project to one Workspace would make both cross-Workspace Projects and multiple Projects within one Workspace awkward.
- Parentless implementation work creates a recovery gap: a cold successor can see that Business intended work and that repository work exists, but cannot prove the intended direct ancestry.
- Temporary cross-Workspace selectors create cleanup debt and can survive interruptions. A two-phase publish/materialize ritual leaves every interruption point truthful instead.
- Projects should remain meaningful manager/coordination boundaries; Tasks and Task children are the cheaper decomposition tool when independent project semantics are absent.

## Consequences

- Work Lifecycle must classify whether the next boundary is a Project or Task before authoring; it must not use Project as a generic grouping node.
- Project → Project is the ordinary subproject mechanism when a real child project boundary exists. Task → Task is the ordinary subtask mechanism.
- Cross-repository spawn has an explicit publication gate. If the intended Parent is not immutable/published, the child work does not yet exist.
- Reverse follow-up should be derived from the Parent/child graph where possible rather than requiring Business to maintain duplicate lists of implementation state.
- Canonical authority artifacts such as schemas, generic Processes, Workspace roots, and Scaffold definitions may retain their own domain-native ancestry. The bounded development work that changes those authorities should still enter through the appropriate Project/work ancestry unless explicitly classified as an exception.
- The current Business Projects `003 Native Schema Authority Extraction` and `004 Deterministic Lineage Maintenance` already express the governing outcomes, but their current Native/Core root Tasks do not yet carry those Business Projects as semantic Parent. That is current migration debt and must be repaired after the Business Project bytes are published, before either implementation frontier resumes.

## Review Conditions

- Review if Tiinex later gains a dedicated graph relation that intentionally supersedes Parent for spawned-work ancestry.
- Review if transactional multi-Workspace publication allows exact cross-repository Parent authority before Git publication without weakening recovery semantics.
- Do not introduce a new Project level solely because a Viewer wants a visual group; improve Viewer projection instead.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-business-lineage-structure-decision.trace.md](001-business-lineage-structure-decision.trace.md)
  - Value: yrgTdisjDp_Msb0sv69J9Agpr_x478fLFG6qSNnpxhI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Dr7Bu5HX8T1JiUa4z5TpCSHOXAazXjWqFQXSJU8XP_o