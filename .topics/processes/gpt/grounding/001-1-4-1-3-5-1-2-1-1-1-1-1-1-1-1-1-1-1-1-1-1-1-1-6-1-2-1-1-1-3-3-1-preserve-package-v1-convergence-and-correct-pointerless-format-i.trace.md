# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 13:08:12
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-3-major-002-pointerless-package-v1-format-alignment-evidence.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-3-major-002-pointerless-package-v1-format-alignment-evidence.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-3-major-002-pointerless-package-v1-format-alignment-evidence.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-22 13:08:39
  - Authors: Anchor
  - Why: The final fan-in blocker is an exact Core format-identity mismatch, not a representation or host design problem.
  - Summary: Keep the accepted single/multi Package V1 convergence; correct only the Workspace-only bundle format declaration that blocks ZIP serialization.
  - Status: ready/local

---

# Anchor Decision — Preserve Package V1 Convergence And Correct Pointerless Format Identity Only

## Decision

- State: accepted
- Subject: disposition of the final integrated Workspace-only Pack failure after Loom/Core + Kodax/VS Code convergence.
- Decision: preserve the accepted Package V1 single/multi-route convergence and accepted Kodax host changes unchanged; open one Core-only micro-correction so Workspace-only/pointerless manufacture declares the same `tiinex.handoff.package.v1` transport format that it already emits and inspects.

## Basis

- Routed Core convergence is green and structurally matches the locked numeric lineage/cache model.
- Kodax's VS Code bridge is green against the reconciled Core up to package integration.
- The only integrated package failure is a bundle-format/inspection-format mismatch in the Workspace-only Core builder.
- A disposable minimal correction restores pointerless, multi-route, bridge and package-integration acceptance without any semantic or host change.

## Consequences

- Loom may change only the Workspace-only transport-format declaration plus the smallest regression needed to prevent recurrence.
- Package V1 remains the single normal recipient-facing representation for pointerless, single-route and multi-route carriage.
- Phase 2/artifact-first specimen paths remain explicit specimens only and may not be reintroduced as normal manufacture.
- Kodax/VS Code is frozen for this micro-correction.
- Anchor retains final fan-in and Sigma sequencing.

## Review Conditions

- Stop if the correction requires any Handoff/Role/cache lineage redesign, VS Code mutation, Docs/schema change, or weakening of ZIP format-consistency validation.
- If the bounded tests and integrated package regression are green, return immediately to Anchor.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-3-major-002-pointerless-package-v1-format-alignment-evidence.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-3-3-major-002-pointerless-package-v1-format-alignment-evidence.trace.md)
  - Value: Y3yxvxebLSJ8KKzGfuwjqTGzUkLQ-mFWnPclOwqIwcA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: uoyIM611FO2mhhFIsqZLEf3SJAbfKGHpYTmU6r76b1o