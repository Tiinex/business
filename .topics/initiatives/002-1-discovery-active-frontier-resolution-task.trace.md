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
  - Summary: Discovery And Active Frontier Resolution
  - Status: draft/local

---

# Discovery And Active Frontier Resolution

## Objective

Make Tiinex Discovery reliably identify current, historical, root, leaf, cross-repository, monitored, and reactivated work so humans and LLMs can orient without treating every technical graph leaf as active.

## Done Criteria

- Discovery can distinguish declared historical/read-only corpora from current frontiers without rewriting history.
- Cross-repository references and Initiative associations can be resolved from qualified material.
- A fresh LLM can discover what exists and select the appropriate Tooling operation without GitHub-first or native-archaeology detours.
- Viewer and CLI can consume the same frontier semantics through shared implementation where appropriate.

## Scope

- Do not infer current work solely from filename order or graph-leaf state.
- Do not require hidden conversation memory or provider identity.
- Schema gaps should be surfaced rather than guessed around.

## Dependencies

- Site/Docs/Business cutoff and coordination decisions.
- Current search-lineage/resolve-lineage behavior.
- Operating Overview epic and Axiom schema findings.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Tooling](002-tooling-project.trace.md)
  - Value: 0zVe7vLWB7VMnz_nU766CpSRIadi72v6t8oX4sxuCxY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Tig87EpJGvKaLJPUQeD7Wfxb3zz_YDgWNni_RqSOt7E
