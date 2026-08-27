# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 22:36:00
  - Trace: [Portfolio Planning And Artifact Composition Decision](002-portfolio-planning-and-artifact-composition-decision.trace.md)
  - Origin:
    - [relative](002-portfolio-planning-and-artifact-composition-decision.trace.md)
- Current
  - Current Schema: [tiinex.discovery.research.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/discovery/research/tiinex.discovery.research.v1.schema.md)
  - Created At: 2026-08-26 22:36:00
  - Authors: Anchor; Sigma
  - Why: Preserve the Discovery basis used to derive the current Initiative and epic portfolio rather than asking future Anchor sessions to infer it from hundreds of historical artifacts.
  - Summary: Cross-repository Discovery synthesis for the current Tiinex portfolio frontier and epic breakdown.
  - Status: accepted/local

---

# Current Repository Frontier And Portfolio Synthesis

## Research Question

- Question: What current Tiinex Initiative boundaries and deliverable-sized work packages are supported by the carried Business, Docs, and Site material after historical cutoff decisions, and what should remain deferred rather than prematurely modeled?

## Source Field

- In Scope: Tooling-driven inspection and lineage search across the current tiinex/business, tiinex/docs, and tiinex/site workspaces; current Business roles and coordination decisions; qualified schema material; current Handoff carrier inspection.
- Out Of Scope: deleting historical artifacts, treating every graph leaf as active work, inventing product subtasks, setting calendar commitments, publishing repository changes, or claiming legal/company state.

## Method

- Method: use Tiinex Tooling `inspect`, `search-lineage`, `resolve-lineage`, schema guides, and Handoff orientation/audit to identify dense historical themes, current frontiers, semantic gaps, and cross-repository boundaries; then condense repeated themes into Project Initiatives and Task work packages whose completion would represent meaningful deliverables.

## Findings

- Finding: Site remains a large historical/dogfood surface. Current Tooling lineage inspection reports 511 nodes, 177 resolved edges, 291 roots, and 42 missing edges, with major recurring clusters around Handoff/cold-start, Discovery/workspace grounding, lineage integrity/repair, publication/permalink qualification, schema capability, and Viewer integration.
- Finding: Docs is comparatively coherent as semantic authority but still contains historical/educational material and validation debt. Current inspection reports 355 nodes and 323 resolved edges; maintained schemas remain current while development history is governed as historical/read-only unless explicitly reactivated.
- Finding: Business is now the condensed organizational surface. Roles are materialized, historical/cached material is retained, and active portfolio coordination has an explicit decision frontier. The new Project/epic tranche increases Business graph roots because exact Task validation currently requires a `browse + git` Parent Origin when Parent is declared; unpublished local Project ancestry cannot be represented truthfully without fabricating publication evidence.
- Finding: Core, Tooling, and Viewer are supported as distinct cross-repository Initiative boundaries. Tooling has the densest active implementation frontier; Core owns semantic/schema coherence; Viewer is a real human product surface intentionally downstream of shared Tooling qualification while still able to feed human evidence back into Core/Tooling.
- Finding: Current Handoff recipient-v2 carrier artifacts repeat machine JSON facts inside every visible human-readable carrier artifact. This is an observed Tooling design defect for artifact purity. The inspected package preserves `001-*` visible carrier prefixes, so prefix loss remains an unconfirmed regression risk rather than a reproduced defect.

## Synthesis

- Synthesis: use Business Development as the meta-project for professionalizing Tiinex operation; use Core, Tooling, and Viewer as stable Initiative Projects; use epic-level Tasks for significant deliverable-sized work; defer subtasks to the repository/work context where implementation happens. Build Milestones from meaningful observable outcomes after epic review, then author one portfolio Roadmap and only later per-Initiative schedules if needed. Keep Operating Monitoring/Workspace composition provisional pending schema/Tooling qualification. Keep Process last and derive it from real repeated artifact behavior.

## Interpretation Limits

- Limits: this research is a current portfolio synthesis, not proof that every historical artifact has been exhaustively classified, that all proposed epics are equally urgent, that the current schemas are sufficient, or that any roadmap dates, funding outcomes, product acceptance, or publication state have been established.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Portfolio Planning And Artifact Composition Decision](002-portfolio-planning-and-artifact-composition-decision.trace.md)
  - Value: C9jsCzDtShe9z3yTA8SrNSNNTM-MEtO5tdbGf77QyJI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:g43lAHYeTSRqKNRLYPqroqojvU3x7bYYzWT8eUVbjKw
