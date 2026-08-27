# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Business Development](001-business-development-project.trace.md)
  - Origin:
    - [relative](001-business-development-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Operating Overview And Monitoring
  - Status: draft/local

---

# Operating Overview And Monitoring

## Objective

Design a shared operating overview that lets Sigma, other humans, LLMs, Tooling, and Viewer locate the Initiatives, current frontiers, watched sources, blockers, resource signals, and relevant cross-repository work without manual archaeology.

## Done Criteria

- Axiom has identified which existing schemas can safely compose the overview and which schema gaps remain.
- Loom has identified which Tooling operations can consume the declared overview without hidden host-specific behavior.
- Monitoring semantics remain distinct from Workspace navigation and from manually maintained status dashboards.
- The overview can point to current work through qualified permalinks/Discovery rather than copying every Task into Business.

## Scope

- Do not assume Monitoring + Workspace + Project composition already works.
- Do not create a second hidden machine-only information model.
- Viewer and LLM/CLI consumers should read the same declared semantic facts through appropriate projections.

## Dependencies

- Initiative and epic inventory.
- Schema-gap discovery for discovery.monitoring, workspace, project, relation, and related contracts.
- Tooling capability discovery.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Business Development](001-business-development-project.trace.md)
  - Value: p1lrm5eQklSARfZ7Gkgxdu1qQRlT2ivmvLe-wo6TwPA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: k5amjJRbSrCcO-iCb6WBFjiGdFv5au4qLFFgHCfyyNI
