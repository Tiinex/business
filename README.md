# Tiinex Business

Tiinex keeps the context around work readable and portable: why material exists, where it came from, what it depends on, what changed, what may carry forward, and what must not be inferred. This repository is the organizational Workspace for Tiinex. It owns Business-level intent, Project outcomes, Roles, Processes, financing provenance, and cross-Workspace disposition where those concerns belong here.

`.topics/**` is the semantic/provenance authority. This README is a human reception surface and should stay small enough that ordinary Project/Task changes do not require manual synchronization.

## Current orientation

Tiinex completed a broad Major 017 fresh-start cleanup. Historical execution attempts remain recoverable through immutable history and qualified Reductions rather than being presented as current merely because an old leaf still exists.

The current project model is:

```text
Tiinex organization
└─ Project: Tiinex
   ├─ Tiinex Business
   ├─ Tiinex Core
   ├─ Tiinex Tooling
   ├─ Tiinex Viewer
   └─ Tiinex Playthings
```

These Projects represent durable outcome directions, not repository folders. One Project may span several Workspaces and one Workspace may contain work for several Projects. Tasks and Task children remain the normal execution decomposition; a new Project exists only when it owns a meaningful independent purpose/scope/outcome.

Two current transition Projects intentionally remain outside the fresh `006` portfolio ancestry until they finish:

- **Native Schema Authority Extraction** — moving first-party schema authority/companions toward Native without creating duplicate authority or a Core↔Native runtime dependency cycle.
- **Deterministic Lineage Maintenance** — establishing safe host-neutral Move/Prepend/re-dimension mechanics before manual lineage maintenance is normalized.

Their repository root Tasks already carry immutable cross-repository Parent ancestry to their pushed Business Project bytes. They were not reparented again merely for visual symmetry.

## Start here

- **Current executive orientation:** [Tiinex Fresh-Start Executive Grounding](.topics/executive/002-fresh-start-executive-grounding.trace.md)
- **Current umbrella Project:** [Tiinex](.topics/initiatives/006-tiinex-project.trace.md)
- **Project/work topology carry-forward:** [Project/Work Topology Rollout Reduction](.topics/reductions/project/005-project-work-topology-rollout-reduction.trace.md)
- **How new work should flow:** [Tiinex Work Lifecycle](.topics/processes/work-lifecycle/001-tiinex-work-lifecycle-process.trace.md)
- **Reusable Business Processes:** [Processes](.topics/processes/001-processes.trace.md)
- **Responsibility/authority:** [Roles](.topics/roles/001-roles.trace.md)
- **Financing provenance:** [Financing](.topics/financing/001-financing.trace.md)
- **Organization root:** [Tiinex organization](.topics/001-tiinex.trace.md)

For LLM-specific routing and explicit “do not infer” rules, see [`llms.txt`](llms.txt).

## Project, Task, Workspace, and Parent

```text
Project
→ real bounded coordinated outcome

Project → Project
→ subproject when the child has its own outcome boundary

Task
→ bounded executable work

Task → Task
→ ordinary subtask decomposition

Workspace
→ ownership / placement surface
→ not Project identity
```

Parent is semantic continuity ancestry. Folder nesting and filename numbers do not manufacture Parent relationships.

For Tiinex-specific development that crosses repositories, the upstream Project must first have immutable published recovery. Only then is the child Project/Task materialized with exact Parent bytes plus commit-pinned recovery. This deliberately creates a safe two-phase spawn boundary: an interruption leaves either a published spawn intent with no child yet, or a fully parented child — not a parentless implementation artifact waiting for cleanup.

## Current execution frontiers

The topology/spawn repair represented by Business Tasks `005` and `005-2` is completed and reduced. Those source files may remain physically present until a later immutable publication makes destructive cleanup/recovery safe; physical presence does not make them current work.

The explicit next implementation frontier from that Reduction is **Core `001-2 Qualify Lineage Maintenance Projection Contract`**. The Native schema-authority extraction frontier remains separately preserved and should resume only through explicit priority and applicable Process grounding.

The older Public Trust / contribution-governance branch is also deliberately preserved because its challenge/bounty disposition may still require explicit future work. Preservation is not evidence of payout, winner selection, or closure.

## Process boundary

Processes describe reusable ways of working. They are not execution logs and their presence does not prove applicability or completion. New bounded work should normally follow the Work Lifecycle:

```text
need / boundary
→ classify owner + Project/Task shape + placement + applicable Process
→ create bounded work
→ execute through the applicable Process
→ accept / land / verify
→ disposition / reduce
```

Each reusable Process owns its own directory beneath `.topics/processes/`; the Workspace-local process catalog root remains directly beneath that directory. Viewer/Tooling should discover Process material from artifacts rather than a hand-maintained README index.

## Financial and organizational boundaries

Tiinex Business preserves organizational and financial provenance, but it is not itself proof of legal incorporation, employment, representation authority, accounting correctness, cash balance, runway, secured funding, or tax outcomes. A pledge is not received money, an invoice is not payment, and a Project/Task status is not human acceptance unless the governing artifacts explicitly establish those facts.

Implementation detail belongs in the natural owning Workspace. Business should not become a duplicate software issue tracker; it should retain organizational why, Project outcomes, priority/acceptance boundaries where applicable, and concise cross-Workspace disposition.
