# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-08-26 22:49:00
  - Trace: [Tiinex Business Development — Axiom semantic gap review](../handoff/004-anchor-to-axiom-business-lineage-and-composition-gap-handoff.trace.md)
  - Origin:
    - [relative](../handoff/004-anchor-to-axiom-business-lineage-and-composition-gap-handoff.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 23:39:00
  - Authors: Axiom
  - Why: Return the bounded schema-semantic disposition requested by Anchor for the current Tiinex Business lineage and composition gap tranche without claiming Tooling implementation, repository mutation, or publication.
  - Summary: Axiom disposition for local Parent Origin truth, Project/Task association, Schedule composition, operating-overview composition, carrier purity, Practitioner specialization, Role versioning, Handoff closure hygiene, Business lineage repair, and stabilization retention.
  - Status: accepted/local

---

# Axiom Business Lineage And Composition Gap Disposition

## Decision

- State: accepted
- Subject: ten semantic transfers in the qualified Anchor-to-Axiom Business lineage and composition Handoff
- Decision: apply the following bounded dispositions. These decisions define semantic targets and follow-up ownership; they do not claim implementation, Git mutation, push, merge, publication, or Anchor acceptance.

1. **local-parent-origin-semantics**
   - Axiom outcome: accept schema change. A truthful local/unpublished Parent is valid continuity when the Parent target is directly recoverable from the same qualified local workspace/materialization. Root must not force a fabricated forge locator.
   - Rule: `Parent` remains direct continuity ancestry. When Parent exists, at least one truthful origin/recovery locator is required. A qualified `relative` locator is sufficient for same-workspace/local continuity; `browse + git` is required only when that Git/forge recovery claim is actually true. Portable package closure may independently prove exact Parent bytes and must not be reinterpreted as publication evidence.
   - Schema owner / target: `tiinex.root.v1`, Parent Origin contract and validator compilation. Descendants inherit the corrected rule; Task/Handoff must not locally re-impose a forge requirement.
   - Change class: root schema correction plus validator/runtime projection correction.
   - Suggested implementation branch: `loom/root-local-parent-origin`.
   - Implementation evidence target: exact validation fixtures for local relative Parent pass, published commit-pinned Parent pass, unresolved Parent fail, and fabricated/unresolvable forge origin fail; cold-recipient Handoff qualification using local Parent bytes.
   - Follow-up owner: Loom for implementation/qualification; Anchor for Business graph repair after qualification.

2. **project-task-association-semantics**
   - Axiom outcome: accept the current Project Initiative + Task work-package model; reject a new `epic.v1` merely for vocabulary.
   - Rule: Project membership/association and artifact continuity are separate. A Task may use an Initiative Project as Parent only when the Task is actually a direct decomposition/refinement/continuation of that Project artifact. A Task created independently and later associated to a Project must use a typed non-parent relation. Cross-repository location never determines Parent.
   - Schema owner / target: `tiinex.project.v1`, `tiinex.task.v1`, and `tiinex.relation.v1`; canonical association predicate is a typed Project-work-item relation (for example `project work item` / inverse `has work item`) rather than Parent overloading.
   - Change class: semantic clarification; no new schema required. Optional future ergonomic projection fields do not change the relation truth.
   - Suggested implementation branch: none required for semantic correctness; any UI/index projection belongs to Loom later.
   - Implementation evidence target: examples covering true Project-to-Task decomposition, independent cross-repository Task association by Relation, and rejection of path-based Parent inference.
   - Follow-up owner: Anchor for lineage repair; Loom only if Tooling lacks typed relation projection/discovery.

3. **roadmap-and-schedule-composition-semantics**
   - Axiom outcome: keep Roadmap as a `tiinex.schedule.v1` planning shape; do not add a Roadmap schema now. Add explicit schedule-to-schedule composition semantics before portfolio Roadmap composition is treated as canonical.
   - Rule: Milestone owns observable milestone/outcome meaning. Initiative schedules own their local ordering/timing. A portfolio Schedule may summarize/order those schedules but must not silently duplicate or override their local timing truth. Schedule remains a human-readable timing/order structure, not a recurrence engine or proof the plan was executed.
   - Schema owner / target: `tiinex.schedule.v1` with an optional typed composition surface for component Schedule references and composition role such as `summarizes`, `orders`, or `aggregates`; `tiinex.relation.v1` supplies the non-parent graph meaning. `tiinex.milestone.v1` remains milestone owner.
   - Change class: Schedule schema amendment; no new Roadmap schema.
   - Suggested implementation branch: `loom/schedule-composition` after Axiom schema text is landed by the schema-authority workflow.
   - Implementation evidence target: validator/examples for portfolio Schedule referencing component Schedules, no duplicated ownership/status, and no recurrence-engine implication.
   - Follow-up owner: Axiom for exact schema amendment; Loom for Tooling support; Anchor authors Roadmap only after both qualify.

4. **operating-overview-composition-semantics**
   - Axiom outcome: composition is not yet canonically complete. `tiinex.discovery.monitoring.v1` is maintained and can own what/why/cadence/boundary of observation. The carried portable runtime's `tiinex.workspace.v1` is a viewer-local Tiinex/site extension (`viewer-local-v119`) and exposes no exact Artifact Creation Contract; it is therefore insufficient as canonical cross-repository schema authority by itself.
   - Rule: Monitoring owns observation intent, field, cadence/trigger, stop/review condition, and observation boundary. Workspace owns human/Tooling/Viewer navigation, membership/entrypoints, and view composition only; it must not become hidden status, execution, monitoring-result, or project-ownership truth. Project/Relation connect the overview to initiatives and monitored targets.
   - Schema owner / target: promote/qualify a canonical `tiinex.workspace.v1` schema authority (Docs-owned or otherwise explicitly canonical) with exact creation/validation contract and relation-friendly member/entrypoint semantics; preserve `tiinex.discovery.monitoring.v1` as the monitoring owner.
   - Change class: schema-authority gap plus Workspace contract completion.
   - Suggested implementation branch: `axiom/workspace-canonical-contract` for schema authority, followed by `loom/workspace-operating-overview` for Tooling/Viewer support.
   - Implementation evidence target: exact Workspace creation/validation authority; overview example linking Projects and Monitoring without copying their lifecycle/execution state; shared human/LLM navigation qualification.
   - Follow-up owner: Axiom for canonical Workspace contract; Loom for implementation; Anchor for final composition review.

5. **carrier-artifact-purity-semantics**
   - Axiom outcome: reject repeated transport-private `TIINEX-RECIPIENT-V2-FACTS` JSON embedded in every visible human-readable carrier artifact as semantic artifact content.
   - Rule: Handoff semantics are declarative transfer semantics, not ZIP/manifest/transport state. Package topology, byte maps, route projections, and repeated machine transport facts belong in one carrier control/manifest surface or another explicitly transport-owned payload/evidence representation. Human-readable carrier artifacts should contain only the minimal semantic statement and exact references/integrity evidence they actually own. Tooling may derive disposable projections from package truth.
   - Schema owner / target: portable recipient-v2 Handoff carrier/projection contract; `tiinex.handoff.v1` remains unchanged in its transport boundary.
   - Change class: portable carrier projection contract correction, not Handoff semantic expansion.
   - Suggested implementation branch: `loom/recipient-v2-carrier-purity`.
   - Implementation evidence target: fresh-recipient package showing no duplicated opaque facts in visible artifacts, with orientation, route qualification, context audit, byte identity, and roundtrip still passing from explicit package control authority.
   - Follow-up owner: Loom; Anchor reviews cold-start continuity after implementation.

6. **practitioner-baseline-and-role-versioning-semantics**
   - Axiom outcome: accept `Tiinex Practitioner` as a standalone provider-neutral `tiinex.party.role.v1` baseline. Specialized roles are peers, not children in an authority hierarchy.
   - Rule: specialization is a typed non-parent relation (`specializes role` / `incorporates role baseline`), never Parent. The baseline contributes working-method obligations and improvement heuristics but cannot widen a specialized Role's `May Do`, holder state, delegation, or authority. Specialized Role boundaries remain controlling for authority. A standalone `tiinex.relation.v1` artifact is valid immediately; a first-class Role specialization surface should project the same typed relation rather than invent inheritance through Parent.
   - Schema owner / target: `tiinex.party.role.v1` plus `tiinex.relation.v1`. Add an optional Role Specialization/Baseline relation surface if machine-readable incorporation is required across all roles.
   - Change class: Role schema semantic amendment for first-class specialization composition; relation predicate definition.
   - Suggested implementation branch: `axiom/role-baseline-specialization`, followed by Loom only for UI/validator projection support.
   - Implementation evidence target: Practitioner -> Anchor/Axiom/Loom/Sigma examples where specialization is discoverable, Parent is absent for specialization, and baseline cannot grant authority omitted/forbidden by the specialized Role.
   - Follow-up owner: Axiom for schema text; Anchor for Role graph repair; Loom for tooling projection if needed.

7. **role-version-retention-semantics**
   - Axiom outcome: accept Parent lineage for materially evolved versions of the same logical Role identity; reject Parent as role specialization.
   - Rule: a new Role version continues the immediately prior version of that same Role through normal Parent continuity. Stable Role identity should be preserved through the Role's canonical identifier/readable identity, while each version remains its own artifact representation. Working-set leaf retention is allowed only when predecessors are demonstrably recoverable through an immutable qualified adapter or preserved package/materialization; local/uncommitted predecessors are not Git-preserved by assumption.
   - Schema owner / target: `tiinex.party.role.v1` lifecycle/interpretation clarification plus corrected Root local Parent semantics from disposition 1.
   - Change class: Role lifecycle clarification; optional schema amendment to state version continuity explicitly.
   - Suggested implementation branch: `axiom/role-version-continuity` if schema text is amended.
   - Implementation evidence target: two-version Role lineage with stable logical identity, local-parent pre-publication qualification, later commit-pinned recovery, and separate Practitioner specialization Relation.
   - Follow-up owner: Anchor for current Role lineage repair; Axiom only if explicit Role contract language is added.

8. **handoff-closure-workspace-hygiene**
   - Axiom outcome: classify Business `.topics/.cache` predecessor-Handoff copies as transport/closure residue, not intended durable Business domain hierarchy. Do not delete until historical recovery is independently preserved.
   - Rule: closure-only copies should live in Handoff/package material closure, scoped to the owning Workspace/route, not as a parallel hidden hierarchy under the durable workspace. Historical Handoff/package bytes are immutable evidence. Migration must preserve the old package/workspace snapshot or immutable adapter state first; then current working-set copies and superseded Handoffs may be removed together when their historical relative references remain recoverable from the preserved representation. Do not rewrite old Handoff bytes merely to make cleanup convenient.
   - Schema owner / target: portable Handoff material-closure/carrier contract plus Workspace boundary; no new `.cache` semantic schema.
   - Change class: closure-storage/migration rule; possible Tooling implementation change.
   - Suggested implementation branch: `loom/handoff-closure-hygiene` if current manufacture still writes closure residue into source workspaces.
   - Implementation evidence target: old package remains recoverable byte-for-byte; new package resolves required context without source-workspace `.topics/.cache`; context audit explains every detached closure byte; no historical reference is silently broken.
   - Follow-up owner: Loom for package behavior if needed; Anchor performs post-checkpoint cleanup only after recovery proof.

9. **business-lineage-repair-target**
   - Axiom outcome: accept truthful leaf-oriented repair, not cosmetic tree tidying.
   - Rule: Initiative Projects may descend from Business Development only when they were actually produced as direct decomposition/refinement; otherwise relate them. Epic Tasks descend from Initiative Projects when they are direct work decomposition. Business Development work packages follow the same rule. Decision/Research/Handoff artifacts parent to the artifact they actually continue/refine/answer only when that direct continuity is true; otherwise remain roots and use typed relations. Role revisions parent prior versions of the same Role; Practitioner specialization stays non-parent.
   - Schema owner / target: Root Parent semantics; Project/Task/Relation/Role/Handoff/Decision/Research use their existing artifact roles. No graph-wide synthetic parent field is introduced.
   - Change class: data/lineage repair after disposition 1 qualifies.
   - Suggested implementation branch: `anchor/business-lineage-repair` after Root/Tooling fix.
   - Implementation evidence target: final Business Discovery graph, exact validations, no fabricated origin, fewer accidental roots only where direct continuity evidence exists, and explicit relations for association/specialization.
   - Follow-up owner: Anchor.

10. **stabilization-commit-gate-semantics**
   - Axiom outcome: accept the current stabilization gate with an explicit durability distinction: semantic stabilization, Git commit, remote publication, and working-set reduction are separate events.
   - Rule: Axiom disposition first; required Loom implementation/qualification second; Anchor graph repair + final Discovery/audit third; Sigma-controlled repository durability checkpoint fourth. Cleanup follows only when predecessor recovery is demonstrated. A local Git commit qualifies as recovery evidence only while the commit object/repository remains retained and reachable through the configured adapter; a GitHub permalink is evidence only after that remote object actually exists. A preserved qualified package snapshot may provide independent recovery without implying Git publication.
   - Schema owner / target: accepted Business stabilization Decision plus Root Origin/provenance truth; no new schema required.
   - Change class: semantic gate clarification; no repository mutation in this tranche.
   - Suggested implementation branch: none for Axiom disposition; later branches are owned by Loom/Anchor as above.
   - Implementation evidence target: qualified semantic/tooling returns, Anchor final audit, actual Sigma-issued Git receipt if/when performed, and a post-checkpoint retention test resolving predecessor artifacts from the declared adapter/package source.
   - Follow-up owner: Anchor coordinates; Sigma alone decides actual commit/push/merge; Loom only where implementation gaps exist.

## Basis

- Pinned schema authority at Tiinex/docs commit `3988951208eb9a8926e84ab42625d4b42fa00c2d` keeps Parent narrow, provides maintained Task, Project, Schedule, Monitoring, Relation, Party Role, and Handoff schemas, and treats relation edges as non-parent semantics.
- The compiled Workspace runtime projection inherits a Root Parent Origin requirement for `browse + git` whenever Parent exists even though `relative`, `absolute`, and `browse + git` are recognized origin labels. That requirement blocks truthful local ancestry and must be corrected at Root rather than worked around by fabricated publication evidence.
- `tiinex.schedule.v1` already represents human-readable timing/order and explicitly is not a recurrence engine; its current contract does not expose first-class component-Schedule composition.
- `tiinex.discovery.monitoring.v1` already owns recurring observation purpose, cadence/trigger, boundary, and review/stop semantics while explicitly excluding runtime crawler configuration.
- Portable Tooling identifies its bundled `tiinex.workspace.v1` source as a Tiinex/site viewer-local extension and reports exact create authority/renderer unavailable, so canonical shared-Workspace semantics are not yet sufficiently grounded.
- `tiinex.relation.v1` explicitly exists for typed non-parent relations and allows relation instances with independent provenance/state to be durable artifacts.
- `tiinex.handoff.v1` explicitly separates transfer semantics from ZIP/export/package/transport mechanics and does not make delivery proof of acceptance or completion.

## Consequences

- No Axiom claim is made that the current Business repository is merge-ready or publication-ready.
- No Roadmap/date artifact is authored in this tranche.
- No Git commit, push, merge, PR, publication, or remote mutation is asserted.
- Loom receives implementation work only for the Root/validator, carrier-purity, Workspace/overview, Schedule-composition, Role-specialization, or closure-storage gaps that require code/runtime changes.
- Anchor owns the subsequent Business graph repair and final cross-role consolidation review; Sigma remains the human authority for actual repository durability actions.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Business Development — Axiom semantic gap review](../handoff/004-anchor-to-axiom-business-lineage-and-composition-gap-handoff.trace.md)
  - Value: 1yzibo2l_LQQCKfTQYjTuATC4WoK4v9WlkG61awQdP8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:7IrMDIMpUH8qiItmoe4-pUuR8kK6kmSXGSppSucpIA4
