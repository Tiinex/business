# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-03 19:28:09
  - Trace: [001-1-establish-work-need-and-boundary.trace.md](001-1-establish-work-need-and-boundary.trace.md)
  - Origin:
    - [relative](001-1-establish-work-need-and-boundary.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-03 19:28:10
  - Authors: Anchor; Sigma
  - Why: Provide one deterministic stage in the reusable Tiinex Work Lifecycle.
  - Summary: Choose semantic ownership, Scaffold placement, and a qualified applicable process without guessing.
  - Status: ready/local

---

# Classify Owner, Placement, And Applicable Process

## Objective

Choose the natural semantic owner before authoring work.

## Classification

- **Organizational owner:** Business when why, priority, initiative, main-project outcome, funding, role, or cross-repository acceptance/disposition is the primary authority.
- **Implementation owner:** the Workspace whose domain is actually changed. Workspace identity does not imply Project identity; one Project may span multiple Workspaces and one Workspace may carry work from multiple Projects.
- **Work shape:** choose Project only for a real bounded coordinated outcome with its own purpose/scope/outcome boundary. Project → Project expresses a genuine subproject. Choose Task for one bounded executable unit; Task → Task expresses ordinary subtasks. Do not insert Project merely to group Tasks or satisfy Viewer layout.
- **Ancestry:** for Tiinex-specific development, identify the nearest governing Business Project before repository work is materialized. Related Project/Task relations supplement but do not replace direct Parent when continuation ancestry is known. Canonical authority artifacts may keep domain-native ancestry; the bounded work that changes them should still enter through Project/work ancestry unless explicitly classified otherwise.
- **Placement:** use the qualified Scaffold capability for the selected Workspace; ordinary subject work belongs beneath that Workspace's work capability rather than an invented directory. Project hierarchy does not mirror repository directories.
- **Process binding:** select a qualified specialized Process when one is applicable; otherwise use the smallest established generic process such as Development And Acceptance.

Process inventory is not applicability. When Project-vs-Task meaning, ancestry, placement, or process applicability is unclear, stop and disposition instead of guessing.

## Entry Binding

For a new session, an Entry may include the selected Process and bounded work as Grounding Material. This creates no execution occurrence or transfer authority by itself.

## Exit Condition

The owning Workspace, artifact family/schema, target placement, Business relationship if any, and applicable Process are explicit.

## Next Artifact

- [Create Bounded Work](001-1-1-1-create-bounded-work.trace.md)

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-establish-work-need-and-boundary.trace.md](001-1-establish-work-need-and-boundary.trace.md)
  - Value: g39fo-xLlEbOSuILM3RrtnhGOpiUuVydSxoVfWQ7c0E

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: dgzKVy_8fBzEgYIwetANemkvdBZYGXytej3wOTWZyK8