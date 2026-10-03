# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-03 17:57:00
  - Trace: [002-fresh-start-roadmap.trace.md](002-fresh-start-roadmap.trace.md)
  - Origin:
    - [relative](002-fresh-start-roadmap.trace.md)
- Current
  - Current Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-10-03 21:16:05
  - Authors: Anchor; Sigma
  - Why: Remove maintenance improvisation risk and make lineage structural changes safe for LLM, CLI, and IDE consumers.
  - Summary: Coordinate deterministic lineage Move/Prepend capability without duplicating implementation truth across Workspaces.
  - Status: ready/local

---

# Deterministic Lineage Maintenance Project

## Project Identity

- Description: Business coordination boundary for making Tiinex lineage relocation and ancestor insertion deterministic enough that LLMs, CLI hosts, and IDE operators do not improvise filesystem renames or semantic Parent changes.
- Boundary: Business owns the organizational need, priority, acceptance boundary, and cross-Workspace disposition. Core owns shared lineage/path semantics. Host-specific UX remains in its natural Workspace and is spawned only after the Core contract is qualified.
- Related Task: Deterministic Lineage Maintenance Projection And Apply in the Core Workspace.
- Evidence Basis: observed process-directory relocation debt plus bounded Core/VS Code discovery preserved in the Core Task lineage carried with this Project.

## Project Purpose And Scope

- Description: Establish one shared lineage-maintenance capability that safely supports whole-lineage and bounded-segment Move with directory-local re-dimensioning while preserving semantic Parent, plus explicit Prepend/Insert Ancestor operations that intentionally change Parent relationships.
- Boundary: Arbitrary sibling/major reordering, generic filesystem rename, lifecycle completion inference, and remote mutation are outside the first implementation boundary.
- Related Task: Deterministic Lineage Maintenance Projection And Apply.

## Parties And Resources

- Relevant Parties: Sigma for operator intent and final acceptance; Anchor for cross-Workspace integration; Core as semantic implementation owner; VS Code/CLI/LLM hosts as consumers of the shared Core capability.
- Relevant Resources: Tiinex Work Lifecycle; Development And Acceptance; current lineage resolver, directory-local path allocator, lineage-integrity planner/apply capability, Scaffold relocation transform, Reduction/recovery semantics, and existing Viewer/VS Code host boundaries.
- Roles: existing Tiinex Role material governs authority; this Project assigns no new Role holder by itself.

## Coordination State

- Description: Discovery is complete enough to create one bounded Core Task. Current tooling has the necessary primitives but no general Move/Prepend operation, no path re-dimensioning apply contract, and no general directory-local filename namespace audit. The Core Task is therefore the current implementation authority.
- Boundary: No lineage mutation is claimed by this Project. A VS Code operator Task is deliberately not spawned until Core exposes a qualified host-neutral plan/apply contract.
- Evidence Basis: the carried Core discovery/operation-contract Evidence.

## Milestones And Outcomes

- Description: Qualify the Core operation model; implement read-only projection and local atomic apply; add directory-local namespace qualification; dogfood the capability by repairing the process-directory dimensions that exposed the gap; then spawn and land host UX against the stable Core contract; accept and reduce terminal maintenance history.
- Boundary: Milestones are desired coordinated outcomes, not completion claims. Implementation truth stays in the owning work artifacts.

## Interpretation Limits

- Does Not Prove: that any current lineage has already been moved, normalized, prepended, accepted, or landed by the new capability.
- Must Not Be Treated As: authority to infer Parent from filename dimensions, mass-renumber unrelated sibling roots, rewrite immutable historical recovery references, or bypass per-artifact qualification.
- Open Questions: final plan schema/API names and host interaction surface are implementation details owned by the Core Task and later host work.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [002-fresh-start-roadmap.trace.md](002-fresh-start-roadmap.trace.md)
  - Value: 0lbTmm4m-d_EHAaV0GWMO9DTne_rEO4SmwmM9pqfvcY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Zee3uAtN8vc5y-r-7p5puHMG-b9ajbl_4JQQQxd2AUg