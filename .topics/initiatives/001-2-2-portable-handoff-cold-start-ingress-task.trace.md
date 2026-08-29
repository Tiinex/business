# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Tooling](001-2-tooling-project.trace.md)
  - Origin:
    - [relative](001-2-tooling-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Portable Handoff, Cold-Start And LLM Ingress
  - Status: draft/local

---

# Portable Handoff, Cold-Start And LLM Ingress

## Objective

Make Tiinex continuation reliably cold-startable from one qualified Handoff carrier so a new Anchor can recover current organizational truth without hidden pre-context or gradual workspace loss.

## Done Criteria

- A qualified Handoff gives a cold recipient one unambiguous route into current work and preserves the semantic Parent lineage already present in source artifacts.
- Stable-major carrier creation requires complete qualified `tiinex-business`, `tiinex-docs`, and `tiinex-site` Workspace snapshots together; a major containing only a subset is not accepted as the Tiinex foundation recovery point.
- Carrier lineage remains a human progress/recovery projection and never replaces artifact Parent lineage.
- Fixed-width/dimension prefixes survive manufacture and round-trip qualification.
- The next stable foundation major is created only after Business, Docs, and Site are mutually current enough for Sigma to accept the foundation and cold-start qualification succeeds.

## Scope

- Handoff manufacture, cold-start routing, workspace completeness, fixed-width carrier lineage, and recovery qualification.
- Do not use a Handoff to reconstruct semantic work that should already exist as source artifacts.
- Do not declare a stable major merely because generic packaging succeeds; the Tiinex-specific three-workspace gate is an additional acceptance requirement.

## Dependencies

- Current recipient-v2 carrier implementation and bootstrap runtime.
- Historical cold-start/Handoff dogfood and fresh-recipient qualification.
- Axiom review where transport changes touch schema semantics.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Tooling](001-2-tooling-project.trace.md)
  - Value: r9jB8WC2FVPxtL4hQGcU0buUznxvGHkwK-mT_SdGQ3I

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 98V3eH4kzG9fScCFCBOzyD6xvfentpTb22NweodQYb4
