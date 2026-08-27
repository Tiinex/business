# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 21:31:12
  - Trace: [Active Tiinex Portfolio Coordination Boundary Decision](001-active-portfolio-coordination-boundary-decision.trace.md)
  - Origin:
    - [relative](001-active-portfolio-coordination-boundary-decision.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-08-26 22:42:00
  - Authors: Anchor; Sigma
  - Why: Preserve the completed Business Development portfolio-structuring tranche and let a fresh Anchor continue from durable Roles, Initiatives, epic work packages, decisions, and Discovery evidence rather than reconstructing this conversation.
  - Summary: Anchor-to-Anchor continuation for Tiinex Business Development after role consolidation, historical cutoff decisions, Initiative materialization, epic-level portfolio breakdown, and Handoff carrier defect discovery.
  - Status: active/local

---

# Tiinex Business Development — Anchor continuation

## Handoff Parties

- Purpose: Continue Tiinex Business Development from the newly condensed Business portfolio surface, preserving Sigma participation, cross-repository Discovery findings, current full-source workspaces, and the decision to build Milestones/Roadmap only after epic review.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-anchor-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role](../roles/001-anchor-role.trace.md)

## Transfers

- portfolio-epic-review-and-refinement
  - Transfer Kind: work
  - Description: Review the materialized Core, Tooling, Viewer, and Business Development epic-level Tasks against current Discovery. Adjust, merge, split, or reprioritize only when new evidence shows a better bounded deliverable structure.
  - Boundary: Do not create implementation subtasks merely to populate the portfolio. Epic Tasks should remain meaningful work packages; concrete execution belongs in the natural repository and may bind back through qualified references.

- milestone-and-roadmap-preparation
  - Transfer Kind: work
  - Description: After epic review, identify meaningful observable Milestones across and within Initiatives, then design the first portfolio Roadmap as a Schedule. Consider per-Initiative schedules only when actual sequencing complexity warrants them.
  - Boundary: Do not author roadmap dates or nested schedule composition from aesthetics. Preserve the distinction between plan, execution lineage, and evidence.

- operating-overview-schema-and-tooling-gap-discovery
  - Transfer Kind: work
  - Description: Qualify whether Discovery Monitoring, Workspace entrypoints, Project relations, and current Tooling can support one shared operating overview for Sigma, other humans, LLMs, Tooling, and Viewer.
  - Boundary: Treat Monitoring + Workspace + Project composition as a desired architecture, not an existing guaranteed capability. Route semantic gaps to Axiom and implementation gaps to Loom.

- portable-handoff-carrier-hygiene
  - Transfer Kind: work
  - Description: Preserve and route the observed Handoff carrier defects: repeated embedded `TIINEX-RECIPIENT-V2-FACTS` JSON in every visible carrier artifact is unacceptable artifact pollution; fixed-width lineage/carrier labels such as `001` must be preserved and regression-tested even though prefix loss was not reproduced in the received package.
  - Boundary: Do not manually patch generated packages as the product fix. Changes belong in Tooling and require fresh-recipient/cold-start qualification.

- process-last-discipline
  - Transfer Kind: responsibility
  - Description: Keep reusable Process artifacts deferred until enough real artifact sequences exist to extract repeatable behavior, including definition/run/step/deviation and Parent-versus-membership semantics.
  - Boundary: Roles may reference future Processes, but do not duplicate speculative procedures into Roles or create Process artifacts merely to complete a taxonomy.

## Required Context

- active-portfolio-coordination-decision
  - Material: current Business coordination and Handoff-parent decision
  - Material Reference: [Active Tiinex Portfolio Coordination Boundary Decision](001-active-portfolio-coordination-boundary-decision.trace.md)
  - Purpose: preserve the current Business frontier, cross-repository anchor model, and continuation boundary
  - Availability: available

- business-development-project
  - Material: current Tiinex Business Development Project
  - Material Reference: [Tiinex Business Development](../business-development/001-business-development-project.trace.md)
  - Purpose: ground the meta-project that owns professional operating structure, sustainability, public trust, overview, and later process adoption
  - Availability: available

- portfolio-planning-decision
  - Material: accepted planning and artifact-composition decision
  - Material Reference: [Portfolio Planning And Artifact Composition Decision](../business-development/002-portfolio-planning-and-artifact-composition-decision.trace.md)
  - Purpose: preserve Initiative/epic/Milestone/Roadmap/Process ordering and Parent-versus-membership semantics
  - Availability: available

- repository-frontier-research
  - Material: current cross-repository Discovery synthesis used to derive the portfolio
  - Material Reference: [Current Repository Frontier And Portfolio Synthesis](../business-development/003-current-repository-frontier-and-portfolio-synthesis-research.trace.md)
  - Purpose: preserve why the current Initiative and epic boundaries were selected and which gaps remain provisional
  - Availability: available

- core-initiative
  - Material: current Tiinex Core Initiative Project
  - Material Reference: [Tiinex Core](../initiatives/001-core-project.trace.md)
  - Purpose: ground the semantic/schema Initiative and its epic work packages
  - Availability: available

- tooling-initiative
  - Material: current Tiinex Tooling Initiative Project
  - Material Reference: [Tiinex Tooling](../initiatives/002-tooling-project.trace.md)
  - Purpose: ground the Tooling Initiative, including Discovery, Handoff, integrity, authoring, and shared-runtime epics
  - Availability: available

- viewer-initiative
  - Material: current Tiinex Viewer Initiative Project
  - Material Reference: [Tiinex Viewer](../initiatives/003-viewer-project.trace.md)
  - Purpose: ground the human-facing Viewer Initiative and its current epic work packages
  - Availability: available

- anchor-role
  - Material: current canonical Business Anchor Role
  - Material Reference: [Anchor Role](../roles/001-anchor-role.trace.md)
  - Purpose: ground the successor Anchor boundary
  - Availability: available

- sigma-role
  - Material: current canonical Business Sigma Role
  - Material Reference: [Sigma Role](../roles/001-sigma-role.trace.md)
  - Purpose: ground Sigma human participation, judgment, priority, and acceptance boundaries
  - Availability: available

## Reference Context

- epic-work-packages
  - Material: all current `*-task.trace.md` epic work packages in `business-development/` and `initiatives/`
  - Material Reference: [Business Development Project](../business-development/001-business-development-project.trace.md)
  - Purpose: use Tooling Discovery from the Project/Business workspace rather than copying eighteen task bodies into this Handoff
  - Availability: available

- docs-current-workspace
  - Material: carried current tiinex/docs full-source workspace including the documentation authority/history boundary decision
  - Purpose: provide current schema/policy authority and historical development evidence for Axiom/Anchor review
  - Availability: available

- site-current-workspace
  - Material: carried current tiinex/site full-source workspace including the historical artifact corpus cutoff decision
  - Purpose: preserve implementation source and historical dogfood while preventing arbitrary old leaves from becoming default continuation targets
  - Availability: available

## Retained Responsibilities

- sigma-human-judgment
  - Retained By: Sigma
  - Responsibility: decide human priorities, acceptable tradeoffs, funding/sustainability intent, public-project intent, and whether proposed portfolio or roadmap changes still match the desired Tiinex direction
  - Boundary: Anchor, Axiom, and Loom should surface evidence and alternatives rather than infer Sigma intent from historical scaffolding

- anchor-cross-role-coherence
  - Retained By: Anchor
  - Responsibility: preserve cross-role architecture, continuity, bounded artifactization, and review; route semantic work to Axiom and shared Tooling work to Loom when warranted
  - Boundary: Anchor does not acquire universal schema, implementation, human acceptance, publication, or legal authority

## Exclusions And Dependencies

- no-subtask-population
  - Kind: excluded-scope
  - Description: do not create detailed implementation subtasks until a bounded epic is actually selected for execution in its natural repository

- no-roadmap-before-epic-review
  - Kind: unresolved-dependency
  - Description: Milestone and Roadmap work depends on reviewing the current epic inventory against qualified Discovery and deciding which outcomes are meaningful

- no-process-before-observed-evidence
  - Kind: unresolved-dependency
  - Description: Process authoring depends on repeated real artifact behavior and Core semantic qualification; current Process ideas remain design direction only

- unpublished-parent-origin-gap
  - Kind: unresolved-dependency
  - Description: current exact Task validation requires a `browse + git` Parent Origin when Parent is declared. Because the new Business Projects are local/unpublished, epic Tasks intentionally use explicit Related Project references instead of fabricating publication evidence. Preserve this as a Core/Tooling schema-capability gap for later repair.

- publication-not-implied
  - Kind: excluded-scope
  - Description: local working snapshots and Handoff carriage do not prove GitHub publication, commit identity, legal organization state, or authorization to write remotely

## Completion Expectation

- Signal Kind: return
- Signal Meaning: continue until a coherent bounded tranche reaches a reviewable checkpoint; preserve resulting durable artifacts and return a Tooling-manufactured Handoff package that continues this decision lineage and carries full-source Business, Docs, and Site workspaces
- Return To: Anchor

## Interpretation Limits

- Does Not Mean: every epic is equally urgent, the roadmap already exists, Process semantics are complete, Monitoring/Workspace composition works today, Site history has been deleted, or Handoff carrier defects have been repaired.
- Must Not Be Used To Claim: legal company status, tax treatment, sponsor commitments, publication, remote Git state, holder identity beyond explicit participation, product acceptance, schema authority outside qualified material, or completion of the transferred work.
- Authority Limits: Sigma retains human structural judgment and acceptance; Anchor coordinates architecture/continuity; Axiom owns schema-semantic reconciliation within transferred scope; Loom owns bounded shared Tooling implementation and qualification.
- Transport Limits: Handoff package carriage provides recoverable working context but does not make transport-private metadata semantic truth. Human-readable carrier artifacts should remain semantically clean.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Active Tiinex Portfolio Coordination Boundary Decision](001-active-portfolio-coordination-boundary-decision.trace.md)
  - Value: k9BfNtThdKxDYV-qs5hZ_3bevbm9jFwl5G_tk0-iQsw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:VJtr_wMXa2z_-JCLDxsuvDr0VbLYSJ9t1BMvIf8nIwg
