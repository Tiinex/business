# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-04 19:50:00
  - Trace: [001-session-grounding-and-continuity-process.trace.md](001-session-grounding-and-continuity-process.trace.md)
  - Origin:
    - [relative](001-session-grounding-and-continuity-process.trace.md)
- Current
  - Current Schema: [tiinex.transition.definition.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/transition/definition/tiinex.transition.definition.v1.schema.md)
  - Created At: 2026-10-06 16:17:50
  - Authors: Anchor; Sigma
  - Why: Turn lineage/recovery packaging into a reusable continuity habit across Roles without duplicating identical behavior into every Role.
  - Summary: Make meaningful Tiinex checkpoints produce durable packages plus explicit branch, new-session, human-action, and next-frontier disposition without creating transfer authority.
  - Status: ready/local

---

# Maintain Durable Checkpoint Package Discipline

## Transition Identity

- Name: Maintain Durable Checkpoint Package Discipline
- Version: 1
- Canonical Identifier: tiinex.process.session-grounding-continuity.maintain-durable-checkpoint-package-discipline.v1
- Transition Family: session-grounding-and-continuity
- Human Label: Maintain Durable Checkpoint Package Discipline

## Purpose And Scope

- Purpose: Make durable checkpoint packaging and explicit operator disposition a routine Tiinex continuity practice at meaningful recovery, branch, handover, return, acceptance, or survivability boundaries.
- Semantic Boundary: Checkpoint packaging preserves recoverability and makes the next operator action explicit; package presence alone never creates Handoff, responsibility transfer, Role holder state, recipient authority, acceptance, current-work selection, or remote-mutation authority.
- Intended Domains: Tiinex sessions already governed by the owning Session Grounding And Continuity profile
- Not Intended For: manufacturing a package after every message/tool call, replacing qualified Handoff at a real responsibility-transfer boundary, or treating chat chronology as durable state

## Input Roles

- session continuity state
  - Meaning: the bounded current session state, latest qualified carrier/recovery boundary, and host survivability observations available at a natural checkpoint
  - Minimum Count: 1
  - Maximum Count: 1
  - Acquisition Policy: invocation-provided
  - Target Kind: non-artifact

## Output Roles

- checkpoint continuity disposition
  - Meaning: a durable checkpoint package when meaningful plus an operator-facing disposition stating branch safety, whether a new session is recommended, package identity, any required human action, and the exact next frontier
  - Minimum Count: 1
  - Maximum Count: 1
  - Target Kind: non-artifact

## Lifecycle And Continuity Effects

### Lifecycle Effects

- produce checkpoint continuity disposition
  - Target Binding: checkpoint continuity disposition
  - Effect: create-new
  - Logical Continuity: no-subject-effect

### Parent Effects

- none

## Relation Effects

- none

## Applicability And Conditions

- Applicability Meaning: applicable at a natural durable checkpoint where meaningful progress, branch/restart opportunity, recipient handover/return, acceptance boundary, or host/runtime survivability risk makes a fresh package materially improve recoverability
- Unknown Meaning: if no meaningful checkpoint boundary exists, continue without package manufacture rather than turning every ordinary turn into transport noise

## Operator Disposition Contract

When a checkpoint package is produced, present the smallest human-facing disposition needed to continue safely. Where the active host supports the concepts, distinguish at least:

- `BRANCH?`: whether branching from the current response is safe;
- `NEW CHAT?`: whether a fresh/cold session is recommended rather than merely allowed;
- `SUGGESTED TITLE`: optional host-facing branch/session label when the host exposes one;
- `PACKAGE`: the exact carrier/checkpoint filename or identity;
- `UPLOAD AFTER?`: whether the operator must re-upload the package after a host transition because volatile runtime/attachment state may not survive;
- `HUMAN ACTION?`: `none` or the exact bounded action such as test, acceptance, commit, push, or other external/manual execution;
- `NEXT?`: the exact bounded continuation frontier.

These fields are presentation/disposition only. Host-specific naming/branching syntax belongs to the selected host adaptation rather than this reusable Business transition.

## Package And Transfer Boundary

- If no qualified responsibility transfer exists, a recovery/checkpoint carrier remains pointerless and must not invent a Handoff route or recipient.
- If a real responsibility-transfer boundary exists, use the applicable qualified Handoff/package semantics instead of treating a generic checkpoint as equivalent.
- Prefer frequent meaningful recoverability checkpoints over relying on one long-lived sandbox/chat, but do not equate checkpoint frequency with semantic progress or acceptance.
- When Tooling can project exact transport text, a host may render/save it as a non-authoritative convenience projection so later recovery does not depend on a still-working sandbox.

## Authoring Bindings

- none

## Placement Intent

### Destination Bindings

- none

### Output Placements

- checkpoint continuity disposition
  - Output Binding: checkpoint continuity disposition
  - Placement Intent: no-materialization

## Interpretation Limits

- Does Not Prove: Handoff, recipient transfer, acceptance, Role holder state, current Task selection, currentness, completion, remote mutation authority, or that a new chat is required merely because a package was manufactured
- Must Not Be Inferred: that all Roles need duplicated Role-specific checkpoint prose; this transition is the reusable continuity habit and Role material should only specialize genuinely Role-specific transfer/return behavior
- Execution Boundary: concrete package identity, Handoff routing when present, host survivability, operator action, and next-work authority remain grounded in their qualified owning artifacts and runtime observations.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-session-grounding-and-continuity-process.trace.md](001-session-grounding-and-continuity-process.trace.md)
  - Value: 4hM7bfYIE-c-B5fNnOKhcfS1_p9JTbgfdsZCIbfdrUE

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: -ZJrXneGhLfc056ogQmi3-ZvnXC-o_JV1OE8mRg7BTE