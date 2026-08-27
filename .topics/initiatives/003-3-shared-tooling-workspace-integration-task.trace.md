# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Viewer](003-viewer-project.trace.md)
  - Origin:
    - [relative](003-viewer-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Shared Tooling And Workspace Integration
  - Status: draft/local

---

# Shared Tooling And Workspace Integration

## Objective

Integrate Viewer with shared Tooling/runtime mechanics for workspace opening, discovery, validation, navigation, and bounded actions so Viewer does not maintain a divergent semantic engine.

## Done Criteria

- Viewer workspace behavior consumes shared qualified mechanics where available.
- Workspace entrypoints and host capability boundaries are explicit and inspectable.
- Viewer-specific adapters remain presentation/integration layers rather than semantic forks.
- Missing Tooling/schema capabilities surface as bounded gaps instead of silent UI workarounds.

## Scope

- Tooling-first does not mean poor human UX; it means shared semantics are stabilized before presentation-specific divergence.
- Do not couple portable core to browser-only state.
- Do not treat Viewer success as proof of CLI/LLM behavior.

## Dependencies

- Tooling shared-runtime epic.
- Workspace schema and operating-overview gap analysis.
- Current Site/reference implementation.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Viewer](003-viewer-project.trace.md)
  - Value: XDkhY9nCj-07BBfSmD-4x3UdUMulAmdvu6lIp-52odM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: YZngT_sw-aYAlUelFBC0wu1-u5xy6P-NAgdMCVV1kVc
