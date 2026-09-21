# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 18:35:26
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 19:47:22
  - Authors: Anchor
  - Why: Integrated fan-in reached a pre-existing Core operator-context leak that still promotes the Extension Host fixture Workspace into the live top-level Workspace set.
  - Summary: Close the remaining Core operator-context nested-Workspace leakage before another Sigma gate.
  - Status: ready/local

---

# Operator Context Top-Level Workspace Boundary Recovery

## Objective

Close the one remaining integrated blocker before another Sigma gate: Core `project-operator-context` must not promote nested fixture/schema Workspaces beneath an explicit repository root into that root's live top-level Workspace set.

## Done Criteria

- Reproduce the exact integrated failure where the Extension repository root projects `extension-host-acceptance` in addition to the intended top-level `extension-vscode` and `vscode` Workspaces.
- Define the smallest shared-Core source-boundary rule consistent with current operator-context semantics: explicit host root material may expose the qualified Workspace artifacts owned by that root's canonical `.topics` surface, while a nested independent `.topics` Workspace is not silently promoted into the parent root's live Workspace set.
- Preserve support for multiple legitimate Workspace artifacts on the same top-level `.topics/.workspaces` surface.
- Do not delete/move fixtures or add VS Code filtering to hide the symptom.
- Keep the latest Loom endpoint/material-closure fixes intact.
- Add deterministic Core regression coverage proving nested fixture Workspaces remain excluded while legitimate sibling Workspace artifacts on the selected root remain visible.
- Re-run the focused Core regressions and the integrated Extension test that previously failed. The integrated assertion must return exactly the intended top-level Workspace set.
- Return exact Core delta and one Loom-to-Anchor Handoff. No self-promotion to Sigma.

## Scope

Shared Core operator-context/workspace source projection and focused tests only.

## Dependencies

- Integrated Fan-In Operator Context Leakage Evidence.
- Current reconciled Loom Core and Kodax Extension VS Code candidate.
- Existing root-cause recovery Task and specialist Evidence remain controlling context.

## Boundaries

- No Docs semantic mutation.
- No Extension VS Code mutation.
- No fixture deletion or relocation.
- No label/recency/path-guess authority.
- No remote mutation, release, publication or deployment.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md)
  - Value: YQlYnFeSTjmcFkCch0U2il9eZT9mxsE4U9a7NqLMQ_w

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: YupwpGwsNjBDUpwmUVLXgfcEc2DxLGt0EVHFdD5KaAA