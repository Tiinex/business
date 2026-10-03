# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-24 19:06:00
  - Trace: [057-anchor-to-anchor-minimal-coldstart-behavioral-gate-transition.trace.md](handoffs/057-anchor-to-anchor-minimal-coldstart-behavioral-gate-transition.trace.md)
  - Origin:
    - [relative](handoffs/057-anchor-to-anchor-minimal-coldstart-behavioral-gate-transition.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-24 19:07:00
  - Authors: Anchor
  - Why: the prior full-Workspace replays exposed historical test-lineage leakage; the remaining grounding-quality proof therefore uses the frozen standalone minimal Workspace plus exact external cache authority.
  - Summary: Run and disposition one genuinely fresh minimal-coldstart Anchor session, then classify the unchanged retrospective without contaminating the test instrument or thawing VS Code.
  - Status: ready/local

---

# Tooling Major 008 — Minimal Cold-Start Behavioral Acceptance

## Objective

Obtain independent behavioral evidence from the frozen minimal-coldstart-001 carrier. The producing Anchor must not coach the recipient or modify the test carrier during the first run.

Sigma is an explicitly required human participant in this current work because Sigma transports the package into a genuinely fresh session, observes the run and supplies the post-run retrospective/human acceptance judgment.

## Done Criteria

- a genuinely fresh no-precontext Anchor receives only minimal-coldstart-001 plus its transport text;
- no corrective Tiinex explanation is supplied during the first run;
- the recipient completes or returns an exact blocker from the package/tooling/material it received;
- only after the first run, the unchanged retrospective is supplied and answered from that run;
- the returned run + retrospective are classified against durable source/tooling authority, with each demonstrated miss assigned to the narrowest durable owner;
- if a real durable defect is found, repair it and repeat with another genuinely fresh session rather than coaching the existing recipient;
- if the minimal behavioral gate passes, record Sigma acceptance and proceed to the remaining Core-freeze gate before any VS Code work resumes.

## Scope

- independent recipient behavior for the frozen minimal-coldstart carrier;
- post-run diagnostic classification and only evidence-supported durable repair;
- Core/Business/Docs continuity needed to preserve and disposition the gate.

## Dependencies

- Evidence 026 machine-qualifies the frozen minimal-coldstart-001 test instrument and records its exact SHA-256.
- Sigma supplies independent transport/observation and human acceptance.
- VS Code remains frozen until this gate and subsequent Core freeze close.

## Interpretation Limits

- This Task is producer continuity and is not carried inside minimal-coldstart-001.
- It does not prescribe what conclusions the fresh recipient must reach beyond the bounded work encoded in the frozen test instrument.
- Machine grounded-to-act is not behavioral acceptance.
- No remote mutation, release or VS Code authority is granted.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [057-anchor-to-anchor-minimal-coldstart-behavioral-gate-transition.trace.md](handoffs/057-anchor-to-anchor-minimal-coldstart-behavioral-gate-transition.trace.md)
  - Value: nq0oGKIZZRyNmgHhGWX52uQhUbzMCCAlxGL4e63mmyM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:3SfpKj_T_7cUSs_QwVhcW9g3PJ7YkzyueeKQ1MFDAMY
