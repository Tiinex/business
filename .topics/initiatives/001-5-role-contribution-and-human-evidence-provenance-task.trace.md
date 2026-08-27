# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Core](001-core-project.trace.md)
  - Origin:
    - [relative](001-core-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-27 12:55:00
  - Authors: Anchor; Sigma
  - Why: Preserve human and AI role contributions as inspectable provenance before downstream synthesis condenses away who observed, judged, challenged, or supplied the evidence that changed the work.
  - Summary: Epic work package for first-class role contribution and human evidence provenance across Tiinex artifacts, Discovery, review, and future Process learning.
  - Status: accepted/local

---

# Role Contribution And Human Evidence Provenance

## Objective

Make material role contributions inspectable as first-class provenance so Tiinex can show not only the final AI-condensed result, but also which human or AI role observed, supplied evidence, challenged assumptions, prioritized, accepted, or otherwise caused meaningful changes in the work.

## Done Criteria

- Material human feedback, screenshots, observations, acceptance signals, and structural judgment can be preserved without requiring verbatim conversation capture.
- Downstream syntheses retain explicit contribution/source links rather than silently replacing the originating role signal.
- Discovery can answer which role materially contributed to a decision, finding, task, or change without inferring identity or authority from conversation context.
- Sigma behavior is teachable from real artifact examples, including observation, prioritization, bias-probing, friction reporting, and human acceptance boundaries.
- Equivalent contribution provenance is available to AI roles when their observations or reviews materially change the work.
- Future Process derivation can distinguish prescribed role instructions from observed role behavior and can learn from both without conflating them.
- Artifactization has a meaningful-signal threshold so routine conversation does not become provenance noise.

## Scope

- Feedback/evidence/contribution semantics, attribution boundaries, screenshot or host-observation references, Discovery projection, and cross-role synthesis provenance.
- Preserve the distinction between contributor provenance and authority: contribution does not automatically prove holder identity, approval, delegation, ownership, or decision rights.
- Support humans and LLMs through the same readable semantic model where practical rather than maintaining separate hidden attribution systems.
- Coordinate with Viewer/Tooling only where projection, capture, or navigation support is required.

## Dependencies

- [Sigma Contribution Provenance Is Underrepresented](../business-development/007-sigma-contribution-provenance-feedback.trace.md)
- Current Role and Practitioner semantics.
- Existing Feedback, Evidence, Relation, Decision, Task, and Discovery schema families.
- Later Process work should consume the resulting real contribution corpus rather than define this epic's semantics in advance.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Core](001-core-project.trace.md)
  - Value: iPnUakoUgOJxovtSJtf3TEcAIJrfOv7NTah1MIagOMU

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:uB8gu6EuYUjpeclSB7U_I71c9EfRrUnq1SGGNqznDKw
