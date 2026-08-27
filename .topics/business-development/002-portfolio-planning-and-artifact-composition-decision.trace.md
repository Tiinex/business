# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Business Development](001-business-development-project.trace.md)
  - Origin:
    - [relative](001-business-development-project.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 22:36:00
  - Authors: Anchor; Sigma
  - Why: Preserve the portfolio and planning semantics explicitly agreed during the current Business Development conversation so future Anchor sessions do not need to reconstruct them from chat history.
  - Summary: Tiinex portfolio planning uses Project Initiatives, epic-level Task work packages, meaningful Milestones, and a later portfolio Roadmap while preserving direct Parent lineage semantics and cross-repository work locality.
  - Status: accepted/local

---

# Portfolio Planning And Artifact Composition Decision

## Decision

- State: accepted
- Subject: Tiinex Business portfolio planning, cross-repository work association, roadmap timing, Process timing, and current Handoff carrier hygiene requirements
- Decision: represent Core, Tooling, and Viewer as stable cross-repository `tiinex.project.v1` Initiative anchors in Business. Represent significant deliverable-sized work packages as `tiinex.task.v1` artifacts rather than introducing an Epic schema unless Task semantics later prove insufficient. Concrete Tasks may live in their natural repositories and relate back through explicit qualified references; Parent remains direct continuity ancestry and must not be overloaded for project membership. Use `tiinex.milestone.v1` for meaningful observable outcome markers. Defer the first portfolio `tiinex.schedule.v1` Roadmap until the Initiative work-package landscape is visible; add per-Initiative schedules only when real sequencing complexity warrants them, and do not assume schedule-to-schedule composition is already semantically complete. Defer reusable Process artifacts until repeated real artifact sequences provide evidence for definition/run/step/deviation semantics.

## Basis

- Current repository Discovery shows dense historical Tooling/Handoff/continuity work, a more coherent Docs semantic surface, and a newly condensed Business surface; a roadmap authored before work-package condensation would mostly restate scaffolding.
- Existing Project, Task, Milestone, and Schedule schemas already cover the intended planning layers without requiring a new Epic or Roadmap schema today.
- Cross-repository work is a first-class requirement: repository location, organizational association, and direct lineage ancestry answer different questions and should remain distinct.
- Process should be learned from actual repeated behavior so multiple roles can follow one reusable method instead of duplicating procedural instructions inside Roles.
- Current Handoff carrier inspection confirms repeated embedded `TIINEX-RECIPIENT-V2-FACTS` JSON across visible carrier artifacts. Human-readable carrier artifacts should not be polluted by duplicated transport-private machine projections. Fixed-width carrier/lineage labels such as `001` must also be preserved and regression-tested even though the current inspected package did not reproduce a prefix-loss defect.

## Consequences

- Business now carries Project roots for Tiinex Business Development, Tiinex Core, Tiinex Tooling, and Tiinex Viewer plus epic-level Task work packages derived from current Discovery.
- Epic Tasks created while their Project parents remain local/unpublished use explicit Related Project references rather than fabricating a `browse + git` Parent Origin. Parent lineage may be introduced later only when truthful qualified ancestry can be represented or the schema contract is corrected for local parent truth.
- Tooling work must include Recipient-V2 carrier artifact purity and fixed-width prefix preservation in the portable Handoff/cold-start work package.
- Operating Monitoring/Workspace composition remains a design target, not an assumed capability, until Axiom and Loom qualify schema and runtime gaps.
- Roadmap and Process artifacts are intentionally not created in this tranche.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Business Development](001-business-development-project.trace.md)
  - Value: p1lrm5eQklSARfZ7Gkgxdu1qQRlT2ivmvLe-wo6TwPA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:WYnUyyMTfwSZamc-2YvlEkqHtsVKPbslEQsPvlr_1Ns
