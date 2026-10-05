# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Trace: [001-processes.trace.md](../001-processes.trace.md)
  - Origin:
    - [relative](../001-processes.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-05 20:24:37
  - Authors: Anchor; Sigma
  - Why: Prevent Process authoring and maintenance from relying on ad hoc Topic lineages or model memory; make typed topology and acceptance discipline explicit.
  - Summary: Reusable typed process for creating, maintaining, verifying and accepting durable Tiinex Process material.
  - Status: ready/local

---

# Process Development And Maintenance

## Current Read

This reusable process governs creation, revision, maintenance, verification, acceptance and controlled supersession of durable Tiinex Process material.

It exists so Process authoring does not depend on ad hoc prose conventions, directory intuition, or one model's memory of how earlier Process trees happened to be shaped.

The process root owns the durable purpose, scope and interpretation boundary. Executable process positions use `tiinex.transition.definition.v1`; durable branch, loop, composition or sub-process topology edges use `tiinex.relation.v1` when the relation itself deserves artifact ownership. Supporting Topics remain valid only when their main value is explanatory/topic semantics rather than executable position semantics.

## Applicable Work

Use this process when creating a reusable Process, materially revising an existing Process, correcting its typed topology, changing its applicability/boundaries, or maintaining it after dogfood exposes a structural weakness.

Minor typo-only edits that do not change Process semantics may follow the owning Workspace's ordinary maintenance discipline without replaying the full process, provided no schema, topology, applicability or authority meaning changes.

## Design Direction

Read the descendant topology as the reusable shape:

`Establish Process Need, Owner And Mode -> Recover Existing Process Semantics -> Design Typed Process Topology -> Author Or Revise Process Material -> Qualify Applicability And Interpretation Boundaries -> Exercise And Verify Process -> Process Acceptance Review -> {Accepted Process Outcome | Return To Process Design}`.

The accepted branch delegates landing to the reusable Accepted Change Landing sub-process rather than embedding current transport/landing mechanics here. The rework branch returns by typed Relation to topology design and does not create a cyclic Parent chain.

## Interpretation Limits

- This process defines reusable Process-development semantics; its presence does not prove that any Process is currently being created, revised, accepted, landed or active.
- Directory placement does not determine Process type, step type, applicability, execution state, currentness or acceptance.
- A Process root may remain `tiinex.topic.v1` while that schema truthfully owns reusable identity/scope. A dedicated Process-root schema requires separate schema-development justification.
- Provider-/host-specific Process material belongs in its semantically owning interop/host Workspace.
- Existing historical Process material is not invalid merely because it predates this process; migration/supersession is separate qualified work.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-processes.trace.md](../001-processes.trace.md)
  - Value: 45zoHVoM9WjJL_ONe7kDaotO2BRdnuHnzObbSXGimc4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: McmCUbZACvnoPZ1nYZoYnI7X_5pkrkimAZAU8r2UMxc