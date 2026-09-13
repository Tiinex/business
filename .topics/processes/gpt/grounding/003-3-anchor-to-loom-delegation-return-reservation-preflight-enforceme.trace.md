# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-13 11:46:07
  - Trace: [003-grounding-major-001-delegation-return-reservation-preflight.trace.md](003-grounding-major-001-delegation-return-reservation-preflight.trace.md)
  - Origin:
    - [relative](003-grounding-major-001-delegation-return-reservation-preflight.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-13 11:58:37
  - Authors: Anchor
  - Why: Business can define delegation readiness, but current Tooling only fails missing reservation at return manufacture time.
  - Summary: Route the remaining early-enforcement gap to Loom without weakening explicit sibling-index uniqueness.
  - Status: ready/local

---

# Anchor To Loom — Delegation Return Reservation Preflight Enforcement

## Handoff Parties

- Purpose: add host-neutral Tooling enforcement that detects missing or unusable non-Major return-carrier reservation before delegation is treated as transport-ready, while preserving explicit coordinated uniqueness and current manufacture semantics.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role — Successor Evolution Continuation](business::.topics/roles/001-1-1-1-anchor-successor-evolution-role.trace.md)
- To: Loom
- To Kind: role
- To Reference: [Loom Role](business::.topics/roles/001-3-loom-role.trace.md)

## Transfers

- delegation-return-reservation-preflight-enforcement
  - Transfer Kind: work-and-responsibility
  - Description: add or extend a portable Tooling preflight surface that can qualify whether an expected non-Major return has one explicit coordinated package sibling index in controlling delegation material before the recipient is sent to work.
  - Boundary: Tooling may validate explicit reservation evidence but must not auto-allocate, infer, scan for, increment, or guess a sibling index in isolated runtimes.

- regression-preservation
  - Transfer Kind: responsibility
  - Description: preserve current non-Major manufacture behavior requiring explicit `--package-sibling-index`, byte-identical duplicate idempotence, divergent collision failure, and existing Major carrier semantics.
  - Boundary: this work does not redefine carrier lineage, semantic Parent authority, Workspace identity, acceptance, or Role authority.

## Required Context

- business-preflight-contract
  - Material: accepted Business decision defining reservation ownership, timing, recipient behavior, and fail-closed semantics.
  - Material Reference: [Delegation Return-Carrier Reservation Preflight Contract](business::.topics/processes/gpt/grounding/003-2-delegation-return-carrier-reservation-preflight-contract.trace.md)
  - Purpose: semantic/process authority for the Tooling preflight.
  - Availability: available

- loom-role
  - Material: current Loom Role boundary.
  - Material Reference: [Loom Role](business::.topics/roles/001-3-loom-role.trace.md)
  - Purpose: implementation authority boundary.
  - Availability: available

## Reference Context

- current-manufacture-behavior
  - Material: portable `handoff` behavior already requires explicit `--package-sibling-index` for non-Major continuation and refuses local next-slot discovery.
  - Purpose: preserve existing return-time uniqueness semantics while moving detection earlier.
  - Availability: available

## Retained Responsibilities

- process-policy
  - Retained By: Anchor
  - Responsibility: own Business process semantics, orchestration policy, integration disposition, and final acceptance of any returned Tooling change.

- canonical-semantics
  - Retained By: Axiom
  - Responsibility: any change to canonical schema/method meaning must be separately routed rather than inferred by Loom.

- human-gate
  - Retained By: Sigma
  - Responsibility: human acceptance/observation only when explicitly controlling; Sigma is not the carrier-index allocator or transport repairer.

## Exclusions And Dependencies

- no-auto-allocation
  - Kind: excluded-scope
  - Description: do not add local next-slot discovery or any heuristic that claims globally unique reservation from filesystem state.

- no-major-semantic-change
  - Kind: excluded-scope
  - Description: preserve Major carrier semantics and existing qualified Handoff/Recovery behavior.

- schema-authority-boundary
  - Kind: unresolved-dependency
  - Description: if preflight requires canonical schema changes rather than Tooling-only qualification/projection, return an exact Axiom-owner follow-up instead of inventing semantics.
  - Responsible Party Or Role: Loom

## Completion Expectation

- Signal Kind: return
- Signal Meaning: one qualified Loom → Anchor return carrying the bounded Core/Tooling implementation and evidence, or an explicit blocker that names the missing authority; no sibling index is guessed and no Sigma transport repair is required.
- Return To: Anchor
- Return To Reference: [Anchor Role — Successor Evolution Continuation](business::.topics/roles/001-1-1-1-anchor-successor-evolution-role.trace.md)

## Acceptance Evidence

- preflight passes when controlling delegation material carries one valid explicit reservation;
- preflight fails visibly for missing, ambiguous, out-of-range, or conflicting reservation;
- existing non-Major manufacture with an explicit sibling index remains green;
- existing Major carrier manufacture remains green;
- no path derives a sibling index by scanning local outputs, carrier names, dimensions, or neighboring files;
- focused and broad Core validation evidence is returned with the exact candidate bytes.

## Interpretation Limits

- Does Not Mean: Tooling owns Business process policy or may allocate globally unique sibling indexes from local state.
- Must Not Be Used To Claim: a preflight PASS creates semantic authority, recipient acceptance, project completion, or human acceptance.
- Authority Limits: Loom may implement and qualify host-neutral Tooling mechanics only within its Role boundary; semantic insufficiency routes to Axiom and integration acceptance remains Anchor-owned.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [003-grounding-major-001-delegation-return-reservation-preflight.trace.md](003-grounding-major-001-delegation-return-reservation-preflight.trace.md)
  - Value: PawxbSgttLQEH7zXEqGu8k2SQa3nh-KVcUQpLVaQxGM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: ETXNZFAFAUoa0o0ZGfuqDcnxQsunC0aKbDYmAk1NXW0