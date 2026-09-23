# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 20:07:53
  - Trace: [006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md](006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
  - Origin:
    - [relative](006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-22 20:16:10
  - Authors: Anchor
  - Why: The parity-only Kodax return exposed a single internal TypeScript interface omission that must be dispositioned before canonical emitted-runtime regeneration can resume.
  - Summary: Authorize the exact VS Code type-surface correction that aligns HandoffLeavesResult with Core's existing findings output and packageBuilder's existing consumer contract.
  - Status: ready/local

---

# Tooling Major 008 — Handoff Leaves Result Findings Contract Reconciliation

The emitted-runtime parity tranche exposed one VS Code-local TypeScript contract mismatch. This Decision resolves only that mismatch so the existing parity Task can resume without broadening Major 008 semantics.

## Decision

`HandoffLeavesResult` in `src/tiinex/bootstrap.ts` shall declare the optional `findings` collection already returned by the shared Core `project-handoff-leaves` operation and already consumed by `src/packageBuilder.ts`.

The bounded source correction is therefore type-surface reconciliation only:

- add `findings?: Array<{ severity: string; code: string; message: string }>;` to `HandoffLeavesResult`;
- do not change `projectHandoffLeaves` runtime behavior;
- do not change `packageBuilder.ts` error handling;
- do not change Core source, Package V1, Role/participant semantics, cache/material closure, Workspace discovery semantics, or pointer lineage.

After this exact correction, resume the existing emitted-runtime parity Task and run the repository-owned build. The known missing/stale emitted outputs remain the build-parity target.

## Basis

The exact carried Core operation currently returns `findings: []` and `findingSummary` in the compact `project-handoff-leaves` result. VS Code `packageBuilder.ts` already treats `projected.findings` as the shared qualification/error channel. The local `HandoffLeavesResult` interface is the sole contradictory surface: it omits `findings` even though both producer output and consumer behavior include it.

This is a compile-time representation omission in the VS Code bridge, not a semantic disagreement and not evidence for any Core or package redesign.

## Consequences

Kodax is authorized to make exactly the bounded VS Code type-surface correction above, then rerun the original emitted-runtime parity work under `005-1-tooling-major-008-vs-code-emitted-runtime-parity-correction.trace.md`.

If the canonical build exposes any additional semantic source defect, stop and return that exact blocker. Missing external build dependencies may be reported as environment blockers, but generated runtime must not be hand-authored as a workaround.

Major 008 remains the sole active Major lineage. No Sigma promotion occurs until emitted-runtime parity, deterministic Core/package acceptance, and the remaining real-host acceptance gates pass.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md](006-tooling-major-008-kodax-emitted-runtime-build-blocker-evidence.trace.md)
  - Value: Xb0mpOfj1U2z7Ph9GrYLoQ22CdV2DPem1cpoauvNuAA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: jfUlOMcIdh2Xc90A1yvlN_DSV_YEZ1TrIHY0-VO5CT4