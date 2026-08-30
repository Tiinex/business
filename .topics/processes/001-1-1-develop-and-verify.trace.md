# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Trace: [Development And Acceptance](001-1-development-and-acceptance-process.trace.md)
  - Origin:
    - [relative](001-1-development-and-acceptance-process.trace.md)
- Current
  - Current Schema: [tiinex.transition.definition.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/transition/definition/tiinex.transition.definition.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Authors: Anchor; Sigma
  - Why: Represent the development-side gate as a reusable artifact instead of burying it in process prose.
  - Summary: Turn bounded implementation work into a candidate outcome that the responsible development role has checked at the level appropriate to that work.
  - Status: proposed/local

---

# Develop And Verify

## Transition Identity

- Name: Develop And Verify
- Version: 1
- Canonical Identifier: tiinex.process.development-acceptance.develop-and-verify.v1
- Transition Family: development-and-acceptance-process
- Human Label: Develop And Verify

## Purpose And Scope

- Purpose: Turn bounded implementation work into a candidate outcome that the responsible development role has checked at the level appropriate to that work.
- Semantic Boundary: This definition represents one reusable position in the proposed process topology. It does not execute work, create an acceptance result, or prove that a real lineage took this step.
- Intended Domains: Tiinex organizational and repository development work where an owning outcome has explicit acceptance criteria.
- Not Intended For: provider-specific workflow code, hidden runtime state, task-status reporting, or automatic conformance claims.

## Input Roles

- bounded work
  - Meaning: the concrete owning Epic, Task, work package, or other bounded outcome being implemented
  - Minimum Count: 1
  - Maximum Count: 1
  - Acquisition Policy: invocation-provided
  - Target Kind: artifact

## Output Roles

- locally verified candidate outcome
  - Meaning: a candidate outcome the development role considers implemented and locally checked, without claiming higher-level acceptance
  - Minimum Count: 1
  - Maximum Count: 1
  - Target Kind: non-artifact

## Lifecycle And Continuity Effects

### Lifecycle Effects

- produce locally verified candidate outcome
  - Target Binding: locally verified candidate outcome
  - Effect: create-new
  - Logical Continuity: no-subject-effect

### Parent Effects

- none

## Relation Effects

- none

## Applicability And Conditions

- Applicability Meaning: applicable when bounded work is being implemented and the responsible development role can perform the checks appropriate to its scope before presenting the outcome for acceptance.
- Unknown Meaning: if the owning work, verification evidence, criteria, or authority needed to interpret this step is unresolved, applicability remains unresolved rather than guessed.

## Authoring Bindings

- none

## Placement Intent

### Destination Bindings

- none

### Output Placements

- locally verified candidate outcome
  - Output Binding: locally verified candidate outcome
  - Placement Intent: no-materialization

## Interpretation Limits

- Does Not Prove: that implementation is correct, complete, merged, accepted, production-ready, or free of remaining work.
- Must Not Be Inferred: that disappearance of active development artifacts alone proves this transition occurred or that acceptance should succeed.
- Execution Boundary: a runtime may render or compare this definition, but real execution truth remains in the real lineage and its evidence.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Development And Acceptance](001-1-development-and-acceptance-process.trace.md)
  - Value: W3iJjUK4Yk6BZx6ko6BbLuKgkZaoa3TMvG0v_Rj762o

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: TVNEkcfMCoRed5e2emp6ZcOym8H-se7r1rb95ul3n74
