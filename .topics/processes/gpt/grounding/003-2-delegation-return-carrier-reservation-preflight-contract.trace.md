# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-13 11:46:07
  - Trace: [003-grounding-major-001-delegation-return-reservation-preflight.trace.md](003-grounding-major-001-delegation-return-reservation-preflight.trace.md)
  - Origin:
    - [relative](003-grounding-major-001-delegation-return-reservation-preflight.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-13 11:57:54
  - Authors: Anchor
  - Why: Repeated qualified returns blocked at manufacture because delegation omitted the required package sibling reservation.
  - Summary: Require explicit durable non-Major return-carrier sibling reservation before delegation dispatch; specialists never guess indexes.
  - Status: ready/local

---

# Delegation Return-Carrier Reservation Preflight Contract

## Decision

- State: accepted
- Subject: non-Major delegation readiness and return-carrier sibling reservation
- Decision: a non-Major delegation that is expected to return a new Tiinex Handoff carrier is not transport-ready until the delegating/orchestrating owner has explicitly reserved one unique package sibling index for that return branch and carried that reservation in durable controlling material. The recipient/specialist must use exactly that reservation and must never guess, discover, increment, recycle, or otherwise invent a sibling index.

## Ownership And Timing

- The delegating/orchestrating owner owns reservation before dispatch because that owner has the program-wide concurrency view required to coordinate uniqueness across parallel branches.
- The reservation must be explicit in the controlling Handoff, Task, Recovery, or equivalent qualified delegation material that reaches the recipient before work begins. Chat-only memory does not satisfy the preflight.
- The reservation binds one intended non-Major return branch. It is transport coordination metadata only; it does not create artifact Parent semantics, Workspace identity, Role authority, acceptance, completion, or source provenance.
- Major carrier progression keeps its existing semantics and is not converted into this non-Major sibling-reservation rule.

## Preflight

Before sending a non-Major delegation that is expected to produce a return carrier, Anchor or the qualified delegating owner must establish all of the following:

1. the intended return is non-Major and will manufacture a new carrier in the current carrier lineage;
2. one explicit package sibling index in the supported range has been coordinated for that return branch;
3. the exact reserved index is present in durable delegation material visible to the recipient;
4. the recipient is instructed to use that exact index when manufacturing the return and not to discover an alternative locally;
5. any known parallel return branches use distinct explicitly coordinated sibling indexes.

If any item is unresolved, the delegation is **transport-not-ready** and should not be dispatched as return-capable work.

## Recipient / Specialist Behavior

- A recipient that has an explicit reservation uses exactly that index for the expected non-Major return carrier.
- A recipient that lacks the reservation, observes an ambiguous/conflicting reservation, or encounters a divergent output collision fails closed and returns the blocker to the delegating owner. It must not ask Sigma or another human gate to invent an index and must not scan local files to choose one.
- A failed or abandoned reservation remains audit history for that branch and is not silently recycled. A replacement return uses a newly coordinated explicit reservation from the delegating/orchestrating owner.
- Byte-identical duplicate transport at one exact reserved output remains governed by Tooling idempotence rules; a divergent collision remains a hard failure rather than a trigger to choose another index.

## Relationship To Existing Grounding Discipline

This contract extends, and does not weaken, the accepted Grounding Major 001 operating reliability and specialist qualified-return decisions:

- package-only qualified return remains the normal completion path;
- package/manufacture failure remains a blocker rather than permission for loose patches or human-applied source;
- Sigma remains outside ordinary transport repair and index invention;
- specialists retain epistemic responsibility for their bounded work while Anchor retains orchestration, reconciliation, scope and carrier-coordination responsibility;
- `grounded-to-act` remains bounded route readiness and does not imply carrier reservation unless the controlling delegation material actually declares it.

## Tooling Enforcement Boundary

Current portable Tooling correctly fails non-Major carrier manufacture when `--package-sibling-index` is absent and refuses local next-slot discovery. That protects uniqueness at return time but does not prove the reservation existed before delegation.

Therefore the durable process rule above is controlling now, while an owner-bounded Core/Loom follow-up should add a pre-dispatch/preflight surface that can qualify the reservation in the controlling delegation material before the specialist is sent to work. That follow-up must preserve the same fail-closed semantics and must not introduce automatic sibling allocation in isolated runtimes.

## Review Conditions

Review when portable Tooling gains a qualified delegation-preflight mechanism, when carrier semantics change materially, or when fresh-role replay finds another recurring transport-repair class. Any automation may reduce operator gestures but must preserve explicit coordinated uniqueness, durable carriage of the reservation, and the separation between transport metadata and semantic authority.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [003-grounding-major-001-delegation-return-reservation-preflight.trace.md](003-grounding-major-001-delegation-return-reservation-preflight.trace.md)
  - Value: PawxbSgttLQEH7zXEqGu8k2SQa3nh-KVcUQpLVaQxGM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: KzJf93XP35ZOxFrXJsRTSOr46vfQR5dOiQSh7qq8dqU