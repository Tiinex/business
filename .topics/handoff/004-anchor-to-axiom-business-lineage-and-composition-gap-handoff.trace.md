# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.discovery.research.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/discovery/research/tiinex.discovery.research.v1.schema.md)
  - Created At: 2026-08-26 22:36:00
  - Trace: [Current Repository Frontier And Portfolio Synthesis](../business-development/003-current-repository-frontier-and-portfolio-synthesis-research.trace.md)
  - Origin:
    - [relative](../business-development/003-current-repository-frontier-and-portfolio-synthesis-research.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-08-26 22:49:00
  - Authors: Anchor; Sigma
  - Why: Route newly discovered schema-semantic blockers to Axiom before Anchor finalizes the same-lineage continuation Handoff, Roadmap, or operating-overview composition.
  - Summary: Anchor-to-Axiom semantic review of local Parent Origin truth, Project/Task association, Roadmap composition, operating-overview schema composition, and transport-metadata artifact boundaries.
  - Status: active/local

---

# Tiinex Business Development — Axiom semantic gap review

## Handoff Parties

- Purpose: Resolve the schema-semantic gaps exposed while materializing the professional Tiinex Business portfolio so Anchor can resume with truthful lineage, cross-repository planning, and a valid continuation Handoff.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-anchor-role.trace.md)
- To: Axiom
- To Kind: role
- To Reference: [Axiom Role](../roles/001-axiom-role.trace.md)

## Transfers

- local-parent-origin-semantics
  - Transfer Kind: work
  - Description: Reconcile Root/descendant Parent Origin semantics for a truthful local/unpublished Parent. Current exact Task/Handoff validation requires `browse + git` whenever Parent exists, while `browse + git` is defined as the portable archive permalink and should be commit-pinned when available. The new local Business Projects therefore cannot be truthful Task parents without either fabricating publication evidence or failing exact validation.
  - Boundary: Do not solve this by inventing a GitHub permalink for unpublished material. Determine the correct semantic/schema contract for local Parent recovery and portable Handoff qualification, including whether an additional origin label/conditional rule is warranted.

- project-task-association-semantics
  - Transfer Kind: work
  - Description: Review the current portfolio choice to model Core, Tooling, and Viewer as Project Initiatives and significant deliverable-sized work packages as Tasks. Epic Tasks currently use explicit Related Project references because truthful local Parent ancestry is blocked. Determine whether current Project/Task/Relation semantics are sufficient for cross-repository Initiative association without overloading Parent.
  - Boundary: Do not introduce `epic.v1` merely for vocabulary. Preserve Parent as direct continuity ancestry and keep repository location, organizational association, and lineage distinct.

- roadmap-and-schedule-composition-semantics
  - Transfer Kind: work
  - Description: Review the plan to defer Roadmap until epic review, then use Milestones for observable outcomes and a portfolio Schedule for ordering/timing. Determine what is semantically required if per-Initiative schedules later exist and a portfolio Roadmap needs to reference or summarize them.
  - Boundary: Do not author the Roadmap or dates in this Axiom tranche. Return semantic requirements/gaps only.

- operating-overview-composition-semantics
  - Transfer Kind: work
  - Description: Qualify whether `tiinex.discovery.monitoring.v1`, `tiinex.workspace.v1`, Project/Relation semantics, and existing artifact types can represent one shared operating overview where Monitoring says what is watched and Workspace says how Tooling/Viewer navigate it.
  - Boundary: Do not assume desired composition is already valid. Identify missing relation, lifecycle, status, or execution semantics explicitly.

- carrier-artifact-purity-semantics
  - Transfer Kind: work
  - Description: Review the semantic boundary exposed by the current recipient-v2 package: every visible carrier artifact embeds repeated `TIINEX-RECIPIENT-V2-FACTS` JSON transport data. State whether such transport-private machine projection belongs inside human-readable Tiinex artifacts or should be represented once outside semantic artifact bodies / derived by Tooling.
  - Boundary: Axiom owns semantic disposition only; Loom owns implementation changes and fresh-recipient qualification.

- practitioner-baseline-and-role-versioning-semantics
  - Transfer Kind: work
  - Description: Define a provider-neutral shared Role baseline for continuous Tiinex improvement, provisionally named `Tiinex Practitioner`: observe meaningful friction, hidden-context dependence, repeated manual/native workarounds, human/LLM asymmetry, schema gaps, Tooling gaps, and opportunities to improve the working method; surface durable improvement evidence without expanding the specialized Role's authority. Define how Anchor, Axiom, Loom, Sigma, and future Roles specialize this baseline without using `Parent` as inheritance.
  - Boundary: Preserve `Parent` for version continuity of the same Role identity. Use an explicit typed non-parent relation or equivalent schema-supported specialization mechanism for Practitioner inheritance. Avoid legal/employment implications and avoid turning every minor annoyance into artifact noise.

- role-version-retention-semantics
  - Transfer Kind: work
  - Description: Qualify the intended Role lifecycle: a materially evolved Role version continues the previous Role version through normal Parent lineage; active workspaces may retain only the current leaf when predecessors are recoverable through immutable adapter-backed provenance such as commit-pinned Git permalinks.
  - Boundary: Working-set reduction must not destroy recoverability. Current local/uncommitted Business material must not be treated as Git-preserved until a real commit/published adapter state exists.

- handoff-closure-workspace-hygiene
  - Transfer Kind: work
  - Description: Review the current Business `.topics/.cache` directory as predecessor-Handoff closure residue. It contains copied Anchor/Sigma Role material and Site decisions required by the older Business Handoff, while the current Business Roles and new Axiom Handoff no longer require those copies. Define the semantic boundary between durable workspace artifacts and Handoff/package closure so transport recovery does not create a parallel hidden artifact hierarchy inside `.topics`.
  - Boundary: Do not simply delete `.cache` while historical Handoff references still depend on it. Define a recoverable migration/repair path first; Loom may then implement any package-manufacture or closure-storage changes.

- business-lineage-repair-target
  - Transfer Kind: work
  - Description: State the semantic target for Anchor's repair round after the local Parent fix: Initiative Projects should become meaningful intermediate nodes with their epic Tasks as descendants; Business Development work packages should descend from the Business Development Project; accepted Decision/Research/Handoff artifacts should follow the actual continuity that produced them rather than remain accidental roots; future Role revisions should continue their prior Role version while specialization remains a non-parent relation.
  - Boundary: Do not force hierarchy where direct continuity is not true. The goal is fewer accidental roots and truthful leaves, not a visually tidy tree at the cost of semantics.

- stabilization-commit-gate-semantics
  - Transfer Kind: work
  - Description: Review the accepted stabilization quality gate for the current Business Development tranche: semantic repair first, Tooling implementation/qualification where required, Anchor graph repair and final Discovery/audit, then a real Sigma-controlled Git durability checkpoint; only after that checkpoint may current working-set reduction rely on commit-pinned or equivalent adapter-backed predecessor recovery.
  - Boundary: Do not infer that a commit, push, merge, or publication already exists. Preserve adapter neutrality and distinguish semantic stabilization from later cleanup/retention.

## Required Context

- business-development-project
  - Material: current Tiinex Business Development Project
  - Material Reference: [Tiinex Business Development](../business-development/001-business-development-project.trace.md)
  - Purpose: ground the project boundary and current tranche
  - Availability: available

- portfolio-planning-decision
  - Material: accepted portfolio planning and artifact-composition decision
  - Material Reference: [Portfolio Planning And Artifact Composition Decision](../business-development/002-portfolio-planning-and-artifact-composition-decision.trace.md)
  - Purpose: preserve the agreed Initiative/Task/Milestone/Roadmap/Process model and current carrier hygiene direction
  - Availability: available

- repository-frontier-research
  - Material: Discovery synthesis that produced the current portfolio
  - Material Reference: [Current Repository Frontier And Portfolio Synthesis](../business-development/003-current-repository-frontier-and-portfolio-synthesis-research.trace.md)
  - Purpose: preserve evidence and known limitations behind the epic breakdown
  - Availability: available

- core-initiative
  - Material: current Tiinex Core Project
  - Material Reference: [Tiinex Core](../initiatives/001-core-project.trace.md)
  - Purpose: ground the semantic Initiative that will own accepted schema/model changes
  - Availability: available

- tooling-initiative
  - Material: current Tiinex Tooling Project
  - Material Reference: [Tiinex Tooling](../initiatives/002-tooling-project.trace.md)
  - Purpose: ground the consuming implementation Initiative and its Handoff/Discovery work packages
  - Availability: available

- axiom-role
  - Material: current canonical Business Axiom Role
  - Material Reference: [Axiom Role](../roles/001-axiom-role.trace.md)
  - Purpose: constrain semantic authority and prevent scope expansion into Tooling implementation
  - Availability: available

- anchor-role
  - Material: current canonical Business Anchor Role
  - Material Reference: [Anchor Role](../roles/001-anchor-role.trace.md)
  - Purpose: preserve the returning review/architecture boundary
  - Availability: available

- sigma-role
  - Material: current canonical Business Sigma Role
  - Material Reference: [Sigma Role](../roles/001-sigma-role.trace.md)
  - Purpose: preserve Sigma human participation and acceptance boundaries
  - Availability: available

- practitioner-baseline-role
  - Material: accepted Tiinex Practitioner baseline Role
  - Material Reference: [Tiinex Practitioner Role](../roles/001-practitioner-role.trace.md)
  - Purpose: ground the provider-neutral improvement behavior that specialized roles may later relate to without Parent inheritance
  - Availability: available

- stabilization-quality-gate
  - Material: accepted stabilization commit and working-set retention decision
  - Material Reference: [Stabilization Commit And Working-Set Retention Decision](../business-development/004-stabilization-commit-and-working-set-retention-decision.trace.md)
  - Purpose: ground the agreed review/commit/cleanup sequence and adapter-neutral recoverability boundary
  - Availability: available

## Reference Context

- draft-anchor-continuation
  - Material: current draft same-lineage Anchor continuation Handoff blocked by the local Parent Origin contract
  - Material Reference: [Draft Anchor continuation](../continuity/001-1-anchor-to-anchor-business-development-continuation-handoff.trace.md)
  - Purpose: reproduce the concrete validation problem without treating the invalid draft as accepted carrier truth
  - Availability: available

- epic-work-packages
  - Material: current epic-level Tasks under Business Development and the three Initiatives
  - Material Reference: [Tiinex Business Development](../business-development/001-business-development-project.trace.md)
  - Purpose: inspect real examples of local Project association and the decision not to fabricate Parent publication evidence
  - Availability: available

- carried-docs-workspace
  - Material: current full-source tiinex/docs workspace
  - Purpose: canonical schema and policy material for exact semantic review, including Root Parent Origin and Role/Relation contracts
  - Availability: available

- carried-site-workspace
  - Material: current full-source tiinex/site workspace
  - Purpose: historical dogfood, original Role material, Tooling implementation context, and prior semantic decisions/feedback
  - Availability: available

## Retained Responsibilities

- anchor-review-and-portfolio-coherence
  - Retained By: Anchor
  - Responsibility: review Axiom disposition against the current Business architecture, update accepted Business decisions/tasks as warranted, and route implementation changes to Loom
  - Boundary: Axiom semantic findings do not independently authorize Tooling implementation or product acceptance

- sigma-human-acceptance
  - Retained By: Sigma
  - Responsibility: decide whether the resulting operating/planning model remains understandable, useful, and aligned with the intended Tiinex direction
  - Boundary: Axiom should not infer human/business intent where current artifacts remain ambiguous

## Exclusions And Dependencies

- no-tooling-implementation
  - Kind: excluded-scope
  - Description: do not implement recipient-v2, prefix, CLI, Viewer, or package-manufacture changes in this Axiom tranche

- no-roadmap-authoring
  - Kind: excluded-scope
  - Description: do not create Roadmap/Schedule or Milestone artifacts before returning the semantic composition requirements to Anchor

- no-process-authoring
  - Kind: excluded-scope
  - Description: Process remains intentionally later-phase and evidence-derived; only note implications if the reviewed semantics materially constrain future Process design

- exact-schema-authority
  - Kind: unresolved-dependency
  - Description: use current qualified Docs schema material and preserve uncertainty where exact current authority or runtime capability cannot be proven from carried material

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return a bounded Axiom disposition that states the accepted/rejected semantic changes or gaps for local Parent Origin, Project/Task association, truthful Business lineage repair, Practitioner baseline and Role specialization/versioning, stabilization commit/retention semantics, Roadmap composition, operating overview composition, carrier artifact purity, and Handoff closure/workspace hygiene; include exact schema artifacts/decisions changed when warranted and leave Tooling implementation to a later Loom transfer
- Return To: Anchor

## Interpretation Limits

- Does Not Mean: Axiom owns Tooling implementation, the Roadmap should now be authored, the current draft Anchor Handoff is valid, or every historical schema problem is in scope.
- Must Not Be Used To Claim: publication, remote Git state, legal/company status, holder identity beyond explicit participation, implementation completion, Viewer acceptance, or sponsor/funding commitments.
- Authority Limits: Axiom may reconcile canonical schema semantics within this bounded transfer; Anchor retains cross-role architecture/review; Loom retains shared Tooling implementation; Sigma retains human structural judgment and acceptance.
- Transport Limits: carried workspace/package bytes are working context and evidence, not publication authority. Transport projections must not silently become canonical artifact semantics.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Current Repository Frontier And Portfolio Synthesis](../business-development/003-current-repository-frontier-and-portfolio-synthesis-research.trace.md)
  - Value: 3LVrnQtt9EIhbKyJ3r-N4FeMsCm8nQqsbDHTouyvuYg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:HVaJMFFjqTuV3euzdRzJXhQ6QlV06GDQTk-ZgttRBwY
