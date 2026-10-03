# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Trace: [001-processes.trace.md](../../processes/001-processes.trace.md)
  - Origin:
    - [relative](../../processes/001-processes.trace.md)
- Current
  - Current Schema: [tiinex.reduction.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/reduction/tiinex.reduction.v1.schema.md)
  - Created At: 2026-10-03 19:32:55
  - Authors: Anchor; Sigma
  - Why: Keep process navigation scalable without exposing pre-convention development layout as current structure.
  - Summary: Reduce the old flat Business process catalogue into per-process directories while preserving exact immutable recovery.
  - Status: ready/local

---

# Business Process Directory Convergence Reduction

## Source Context

- Source: `Tiinex/business@e6739663336519dd52afd1e038287bca4859d77a`, where the Business process catalog contained nineteen process artifacts directly beneath `.topics/processes/`.
- Exact Recovery: the immutable commit above preserves the old flat catalog bytes, including process root Git blob `2d18624ca9ea68938fdae1688fc15de9f57d3be1` and all eighteen process-definition/step artifacts moved by this convergence.
- Reduced Structure: the former flat Development And Acceptance, Accepted Change Landing, Human-Mediated External Execution, and Bounded Generative Visual Source Production files.
- Current Structural Target: one Workspace-local process catalog artifact directly beneath `.topics/processes/`, with each reusable process owning `.topics/processes/<process-handle>/`.

## Carry-Forward State

- `.topics/processes/001-processes.trace.md` remains the Business-local process catalog root and real Parent of direct Business process-definition roots where that ancestry is truthful.
- `development-and-acceptance/` owns the Development And Acceptance definition and its process topology.
- `accepted-change-landing/` owns the reusable Accepted Change Landing process and its topology.
- `human-mediated-external-execution/` owns the bounded external-execution process.
- `bounded-generative-visual-source-production/` owns the generative source/freeze/derive/review process.
- `work-lifecycle/` is the new reusable outer Tiinex Work Lifecycle and follows the same directory convention.
- Docs keeps its own Workspace-local process root plus `schema-development/`, preserving local schema-process authority rather than moving Docs process semantics into Business.
- Process directory placement expresses process ownership/navigation only. It does not manufacture Parent ancestry, execution occurrence, process applicability, acceptance, currentness, or completion.

## Loss And Uncertainty

- No old process bytes are intended to remain current at their flat Business coordinates; exact pre-convergence bytes remain recoverable from the immutable source commit.
- Numeric lineage filenames are intentionally retained inside each process directory to avoid inventing a second filename-renaming migration while directory ownership is sufficient for navigation.
- A generic process executor is deliberately not introduced. A qualified Entry or work boundary may ground an applicable Process, while real work lineage remains execution truth.
- Process applicability remains semantic and must not be inferred merely from catalog membership or directory proximity.

## Validation

- The Core reference-safe relocation projection qualified before apply with 18 moved artifacts, 13 relative reference rewrites, 14 Parent-integrity updates, 18 self reseals, and zero findings.
- Local old Business process bytes were verified Git-blob-identical to `Tiinex/business@e6739663336519dd52afd1e038287bca4859d77a` before mutation.
- After the process-root semantics were updated, a Parent-first Core projection deterministically refreshed 25 descendant Parent-integrity/self-integrity values.
- The current process structure is subject to final Business/Native/Core inspect and regression qualification before carriage.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-processes.trace.md](../../processes/001-processes.trace.md)
  - Value: 894_R-4DZE3RsHODoloOXj00yq9YAvOSDFA_3iwmBgc

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: X_E_XqsIYI4Nhj47KbelVn0HJJRdtVG8PdxxcItpwQQ