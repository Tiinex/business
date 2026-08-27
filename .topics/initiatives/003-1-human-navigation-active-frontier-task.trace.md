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
  - Summary: Human Navigation And Active Frontier Experience
  - Status: draft/local

---

# Human Navigation And Active Frontier Experience

## Objective

Give a human a clear way to enter Tiinex, understand what is current versus historical, move across Initiatives/workspaces/lineages, and reach the active frontier without learning internal repository archaeology.

## Done Criteria

- Viewer can present declared current/historical boundaries and active Initiative/work-package context.
- Navigation follows qualified artifact relations and workspace entrypoints rather than hidden UI state.
- A person can move from portfolio-level context to relevant cross-repository work and back without losing provenance.
- Historical dogfood remains inspectable without dominating the default current experience.

## Scope

- Do not invent active state from UI heuristics when artifacts disagree.
- Do not require every Tooling capability to be exposed at once.
- Keep the underlying artifact/permalink path visible enough for recovery.

## Dependencies

- Tooling Discovery/frontier epic.
- Business Initiatives and later operating overview.
- Site historical cutoff decision.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Viewer](003-viewer-project.trace.md)
  - Value: XDkhY9nCj-07BBfSmD-4x3UdUMulAmdvu6lIp-52odM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: T3s3NMUnenMUImx2FNCPozbJH-HLCewU9CA4vISE5uM
