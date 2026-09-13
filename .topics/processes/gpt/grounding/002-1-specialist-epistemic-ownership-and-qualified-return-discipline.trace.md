# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-12 19:09:24
  - Trace: [002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md](002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
  - Origin:
    - [relative](002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-12 20:58:22
  - Authors: Anchor
  - Why: Live VS Code iterations showed focused-test green returns masking compile/integration failures and a specialist asking Sigma to apply a Git patch, creating human debugging burden and transport drift.
  - Summary: Require specialists to own coarse workspace health, retain epistemic responsibility through human observations, and return only qualified Handoff carriers rather than shifting debugging or patch application to Sigma.
  - Status: ready/local

---

# Specialist Epistemic Ownership And Qualified Return Discipline

## Decision

- State: accepted
- Subject: specialist completion, validation and transport behavior under Anchor-orchestrated work
- Decision: a specialist owns the epistemic case for its bounded implementation until it can either return a qualified workspace/Handoff carrier with sufficient health evidence or explicitly return a blocker. Anchor review and Sigma human observation do not replace specialist-owned validation, and Sigma must not be used as the default debugger, patch applier, repository repair operator or integration-test team.

## Required Operating Behavior

- A specialist must distinguish `implemented`, `validated`, `implementation-ready`, and `human-accepted`; inability to run a required gate must remain visible rather than being converted into a green return.
- Coarse workspace-health gates precede feature-specific confidence where the repository supports them: exact/locked environment restoration, typecheck/compile, ordinary build and broad existing validation are evaluated before focused regression tests are treated as completion evidence.
- Focused tests support the epistemic case but do not substitute for coarse repository health. A feature-local green test suite cannot justify an implementation-ready return while the ordinary workspace build or compile gate is red or unknown.
- When a required environment cannot be reproduced exactly, the specialist should diagnose the environment boundary, preserve the candidate change, and return the missing evidence/blocker explicitly. It must not claim that plausibility, source inspection or focused tests prove the unavailable gate.
- Sigma may be used as a bounded external sensor for observations that genuinely require the real human/Windows/host environment. The specialist frames the hypothesis, requests the minimum discriminating observation, explains what outcomes mean, and retains responsibility for diagnosis and technical next steps.
- Sigma is not expected to author or repair source, apply Git patches, choose technical fixes, restore repositories, or discover ordinary compile/build regressions for a specialist.
- Normal completion transport remains the qualified Handoff package plus its exact routing text. Loose Git patches, loose changed files, copy/paste source edits or instructions for Sigma to apply implementation deltas are not a substitute for the Handoff carrier.
- A specialist that has changed carried workspace bytes must package those exact candidate bytes through the qualified Tiinex Handoff path. If it cannot manufacture the required carrier, that is a blocker to return, not a reason to shift application work to the human operator.
- Anchor audits scope, authority, evidence sufficiency, reconciliation and program impact. Anchor should not silently become the specialist's primary QA/debugger by discovering routine repository-health failures after every return.

## Evidence Triggering This Decision

- In the live VS Code Major 003 lane, focused clipboard/icon tests passed while the ordinary TypeScript build later failed on a carried compile error.
- A later lifecycle repair again produced strong focused evidence while the real Windows build/restart flow exposed additional integration failure.
- The current specialist iteration attempted to hand Sigma a Git patch/application step instead of preserving the package-only transport convention, despite the carrier/tooling contract already defining normal operator completion as a Handoff package plus routing text.
- These events create a process regression in which Anchor becomes a repeated downstream auditor and Sigma becomes an external debugger/patch applier. That pattern increases human correction turns, weakens automation readiness and undermines fresh-role trust.

## Consequences

- Specialist Tasks/Handoffs should carry outcome-oriented validation expectations rather than accumulating one new micro-test for every discovered symptom.
- Repeated failures of the same completion discipline are grounding/process evidence and should be routed to the narrowest durable Role/process owner rather than taught privately in chat.
- Human live gates remain valuable for product behavior, accessibility, host-specific observations and acceptance, but they occur after the specialist has exhausted the validation available within its bounded workspace/runtime.
- Transport purity is part of recoverability: project state intended to survive chat/provider/runtime loss must reside in qualified carried bytes, not in a human-applied patch that exists only because a particular conversation asked for it.

## Review Conditions

- Review after fresh specialist sessions consistently return build-clean or explicitly blocked work without Sigma debugging/application help.
- Review if a repository lacks meaningful coarse health gates; that is a repository/tooling capability gap to route, not permission to silently weaken the completion standard.
- Review if a future automated transport host provides an equivalent qualified carrier mechanism; automation may change the operator gesture but must preserve exact-byte provenance and return authority.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md](002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
  - Value: mK4JerPYAZOZ_kE5IiYaXyvvMaJG088uZtuBc-a9VBw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: M0IBsQHaRz3Hh9eKZRqybTcJjpociEog75rut7F0r5c