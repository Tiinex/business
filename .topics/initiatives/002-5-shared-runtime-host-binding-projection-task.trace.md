# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Tooling](002-tooling-project.trace.md)
  - Origin:
    - [relative](002-tooling-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Shared Runtime, Host Binding And Projection
  - Status: draft/local

---

# Shared Runtime, Host Binding And Projection

## Objective

Consolidate reusable Tiinex mechanics behind host-neutral interfaces so CLI, LLM hosts, Viewer, and future integrations share one semantic/runtime core without hiding capability boundaries.

## Done Criteria

- Portable runtime exposes explicit host capability binding and fails closed when required capabilities are unavailable.
- CLI remains a first-class human and LLM consumer.
- Viewer can reuse shared discovery/resolution/validation mechanics without duplicating semantic logic.
- Host-specific adapters remain outside canonical semantics and return explicit evidence/receipts where authority matters.

## Scope

- Do not make one provider, IDE, chat host, or Viewer implementation the architecture center.
- Do not infer host capability from provider name alone.
- Preserve offline/local-first and recoverable operation where feasible.

## Dependencies

- Portable Tooling runtime and host capability model.
- Viewer shared-integration epic.
- Current cold-start and workspace discovery findings.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Tooling](002-tooling-project.trace.md)
  - Value: 0zVe7vLWB7VMnz_nU766CpSRIadi72v6t8oX4sxuCxY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 8UYlbxUzZ6wjLWWmx4VEfywnPCs4Wy1yJBZDi6St7bU
