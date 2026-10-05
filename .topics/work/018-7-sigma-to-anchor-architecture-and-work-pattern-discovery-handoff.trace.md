# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-05 13:22:47
  - Trace: [018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Origin:
    - [relative](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-10-05 17:54:53
  - Authors: Sigma; Anchor
  - Why: Preserve Sigma observations, external audit blockers, and Discovery-derived design constraints as recoverable work authority before implementation resumes.
  - Summary: Transfer bounded architecture/process discovery findings and the high-confidence implementation plan to Anchor without implying acceptance or cleanup authority.
  - Status: ready/local

---

# Sigma To Anchor Architecture And Work-Pattern Discovery Handoff

## Handoff Parties

- Purpose: transfer the bounded architecture/process discovery and planning responsibility raised during the grounding-reliability acceptance exercise without implying acceptance, closure, or cleanup authority
- From: Sigma
- From Kind: role
- From Reference: [Sigma Role](../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Transfers

- architecture-and-work-pattern-discovery
  - Transfer Kind: work-and-responsibility
  - Description: reconcile the supplied audit/retro findings and Sigma observations into one high-confidence implementation plan for Role qualification truth, Process representation/decomposition, Workspace-local work-area structure/reduction, and Core/CLI/Runtime ownership boundaries
  - Controlling Artifact: [Recover Post-023 Authority And Lineage Closure Batch](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Boundary: discovery/planning and only the smallest later repairs justified by separately qualified authority; no Task closure, Sigma acceptance claim, real hygiene cleanup, broad work migration, remote mutation, or speculative repository split

## Required Context

- controlling-recovery-task
  - Material: exact controlling Task
  - Material Reference: [Recover Post-023 Authority And Lineage Closure Batch](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Purpose: preserve the current grounding/recovery acceptance boundary and nonterminal lifecycle
  - Availability: available
- work-lifecycle-process
  - Material: Tiinex Work Lifecycle
  - Material Reference: [Tiinex Work Lifecycle](../processes/work-lifecycle/001-tiinex-work-lifecycle-process.trace.md)
  - Purpose: current authority for ownership, placement, execution, follow-up, reduction, and short-frontier semantics
  - Availability: available
- lineage-structure-decision
  - Material: Business Lineage Structure Decision
  - Material Reference: [Business Lineage Structure](../decisions/001-business-lineage-structure-decision.trace.md)
  - Purpose: current authority separating Parent semantics, filename dimensions, Workspace placement, and current leaf projection
  - Availability: available
- project-task-topology-decision
  - Material: Project/Task/Spawn topology Decision
  - Material Reference: [Project, Task, And Spawn Topology](../decisions/001-1-project-task-and-spawn-topology-decision.trace.md)
  - Purpose: preserve Project-vs-Task semantics independently of repository folders
  - Availability: available
- current-business-workspace
  - Material: exact current Business Workspace
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: current Process, Role, Decision, and work-frontier material
  - Availability: available
- current-core-workspace
  - Material: exact current Core Workspace
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: current host-neutral mechanics, bootstrap, grounding, lineage and transitional CLI compatibility implementation
  - Availability: available
- current-native-workspace
  - Material: exact current Native Workspace
  - Material Reference: [Native Workspace](native::.topics/.workspaces/tiinex-native.workspace.md)
  - Purpose: current first-party schema/content and Workspace Scaffold authority
  - Availability: available
- current-cli-workspace
  - Material: exact current CLI Workspace
  - Material Reference: [CLI Workspace](cli::.topics/.workspaces/tiinex-cli.workspace.md)
  - Purpose: current dedicated command-line host boundary over Core
  - Availability: available
- current-runtime-native-workspace
  - Material: exact current Runtime Native Workspace
  - Material Reference: [Runtime Native Workspace](runtime-native::.topics/.workspaces/tiinex-runtime-native.workspace.md)
  - Purpose: current intentionally minimal headless runtime frontier
  - Availability: available

## Reference Context

- latest-grounding-acceptance-handoff
  - Material: current Sigma acceptance Handoff
  - Material Reference: [Grounding Reliability Acceptance](018-6-anchor-to-sigma-grounding-reliability-acceptance-handoff.trace.md)
  - Purpose: preserve that acceptance remains a separate unresolved gate
  - Availability: available

## Current Discovery

### Role qualification truth

- External audit evidence identifies an authority-critical inconsistency: current canonical Role validation and Core grounding can accept different serializations of `Assignment Modes`.
- The current Role schema declares `Assignment Modes` the only machine-authoritative current holder-assignment representation and requires canonical token serialization/order.
- Grounding must consume one qualified Role projection rather than reparsing raw authority-bearing Markdown with a tolerant second rule set.
- The historical/current Sigma Role must not be rewritten merely for cosmetic audit green; any mutation follows after the qualification owner and repair boundary are explicit.

### Process representation and decomposition

- Current reusable Process roots and steps are authored as `tiinex.topic.v1`; no dedicated `tiinex.process.v1` schema exists in the carried Docs/Native schema authority.
- Process Scaffold gives a strong directory convention (`.topics/processes/<process-handle>/`, process root plus steps/branches), but schema typing remains Topic-based.
- `session-grounding-and-continuity` in both Business/Native and `human-mediated-external-execution` are represented by one Process artifact only.
- A one-artifact process is valid only when the process is genuinely atomic. Grounding is no longer atomic in practice: entry boundary, required material, process applicability, carried-source preference, host adaptation, readiness disposition, and checkpointing are already explicit distinct steps in prose and repeatedly exercised by cold-start/retro dogfood.
- Therefore Process decomposition/typing is a real design question, not a Viewer-only issue.

### Work placement and visual work health

- Current Work Lifecycle already says Business owns organizational why/priority/acceptance/disposition while implementation truth belongs in the natural Workspace.
- It also requires terminal/superseded history to reduce and unresolved work to preserve a short explicit frontier rather than leave long historical execution lineages looking current.
- Current Work Scaffold establishes only `.topics/work` and has no Work-area directory convention, unlike the Process Scaffold.
- Current Reduction Scaffold likewise establishes only `.topics/reductions` and does not define how one completed Work area should be reduced/discovered as a scoped unit.
- This mismatch explains why correct semantic guidance can still produce visually long flat work journals and invites improvisation.
- Directory scope must improve human/disaster-recovery pattern recognition without becoming semantic Parent authority or a fake Project taxonomy.

### Core / CLI / Runtime ownership

- Core architecture already declares host-neutral mechanics plus carrier/tooling bootstrap runtime as Core-owned and final ordinary CLI host UX as not Core-owned.
- Core still carries roughly 4.8k lines of `src/tooling/portable/adapters/cli/*` plus the transitional `tools/tiinex-portable.mjs` compatibility entrypoint.
- The dedicated CLI repository already depends one-way on `@tiinex/core`, but currently exposes only a small secure-transport host surface.
- Runtime Native is intentionally minimal and exports no runtime contract until a new bounded task qualifies one.
- Therefore the next decision is not “move CLI because a CLI repo exists”. First classify each Core `cli.*` responsibility as host-neutral operation/input-output contract vs ordinary terminal host UX. Preserve dependency direction `CLI -> Core`; do not create `Core -> CLI`.
- No new repository is justified by current evidence. New repositories remain allowed only if classification reveals a domain that cannot be owned cleanly by existing Core/CLI/Runtime Native/Interop boundaries without a cycle.

## High-confidence Plan

1. **P0 — Reconcile Role authority qualification.** Establish one canonical Role qualification projection for `Assignment Modes`; make grounding consume it; add current Business Role composition tests; only then disposition the Sigma Role serialization and re-run the acceptance gate.
2. **P1 — Specify Process semantics before Tooling.** Decide whether reusable Process deserves a dedicated schema or whether `topic.v1` remains intentional. Define when a Process may be one artifact versus when durable step decomposition is required. Apply the rule first to grounding/continuity because it is demonstrably multi-step.
3. **P1 — Specify Work-area and Reduction-area structure.** Extend durable Process/Decision/Scaffold authority so `.topics/work/<work-area>/` (exact handle rule to be decided) can scope one bounded execution surface without replacing semantic Parent/Project authority. Define start/frontier/terminal-reduction conventions and corresponding `.topics/reductions/...` discovery behavior. Keep Markdown sufficient for no-Tooling emergency grounding.
4. **P1 — Align Work Lifecycle and Roles.** Review canonical Role material for stale assumptions about Business-as-workbench and specialist write scope. Make the general work process explicitly support control-plane Business coordination with execution-plane Workspace-local work and Handoff/Return boundaries.
5. **P1 — Classify CLI extraction boundary.** Inventory Core `cli.*` modules into host-neutral contracts vs terminal-host UX. Move only terminal host ownership to CLI while preserving Core-owned carrier/tooling bootstrap mechanics and one-way dependency `CLI -> Core`. Keep Runtime Native empty until a separate execution-model contract exists.
6. **P1/P2 — Tooling/scaffold implementation after authority.** Update scaffolds, authoring/qualification, Viewer/CLI projections, and migration planning only after the above Markdown/schema/Decision authority is accepted. Do not migrate existing work trees yet.
7. **P2 — Migration rehearsal before cleanup.** Use deterministic Move/Normalize/rebase planning plus required locking/journal/crash-recovery safety before broad canonical work/process/hygiene migration. Rehearse on disposable copies first.
8. **Verification gates.** Re-run Core/Native, Role authority parity, cold grounding, specialist Handoff/Return dogfood, current VS Code verification, and human pattern-readability review before any broad migration or Task closure.

## Retained Responsibilities

- sigma-acceptance
  - Retained By: Sigma
  - Responsibility: human accept/block disposition for the grounding/recovery checkpoint after the authority-critical Role qualification inconsistency is reconciled
  - Boundary: this discovery Handoff does not manufacture acceptance
- anchor-orchestration
  - Retained By: Anchor
  - Responsibility: keep future implementation in bounded Workspace-owned work and reconcile specialist Returns without turning Business into duplicate implementation truth
  - Boundary: no inferred cleanup or remote-write authority

## Exclusions And Dependencies

- real-work-tree-migration
  - Kind: excluded-scope
  - Description: do not restructure existing Business/Core/Native work trees merely because the target convention is clearer
  - Responsible Party Or Role: later explicitly qualified migration work after schema/scaffold/tooling authority and safety gates
- process-migration
  - Kind: excluded-scope
  - Description: do not rewrite existing Process artifacts or directories before the Process representation/decomposition decision qualifies
  - Responsible Party Or Role: later bounded Docs/Native/Business work according to semantic ownership
- speculative-repository-split
  - Kind: excluded-scope
  - Description: do not create repositories merely to make the dependency diagram look symmetric
  - Responsible Party Or Role: later architecture work only if classification proves an ownership domain missing from existing repositories
- remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release, deployment, or other remote write
  - Responsible Party Or Role: separately authorized operator

## Completion Expectation

- Signal Kind: result
- Signal Meaning: Anchor continues from this discovery with P0 Role qualification reconciliation first, then durable Process/Work/CLI boundary authority before implementation/migration; return blockers and plan changes through normal Handoff discipline
- Return To: Sigma
- Return To Reference: [Sigma Role](../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Sigma accepted Task 018, Process schema direction is already decided, work directories may be migrated now, CLI extraction is approved in a specific file-by-file form, a new repository is required, hygiene cleanup is authorized, or remote mutation is authorized
- Must Not Be Used To Claim: Task closure, final Process taxonomy, final dependency graph, migration completion, or acceptance of the external audit disposition by Sigma

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Value: 7g55_HJ1fGhCLlR-o11oSeyefoUdu4dmxF90oujTy68

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: V_AxjXuMhgcs9UHPjxuShfO87_-fh1KeCJ4jVKKam-s