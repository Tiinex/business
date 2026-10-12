# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-10-05 19:21:14
  - Trace: [001-2-entry-what-where-and-workspace-work-area-structure.trace.md](001-2-entry-what-where-and-workspace-work-area-structure.trace.md)
  - Origin:
    - [relative](001-2-entry-what-where-and-workspace-work-area-structure.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-10-11 22:57:01
  - Authors: ChatGPT (analysis session; canonical Role holder unverified)
  - Why: Human candidate for Sigma audit; not an accepted Tiinex Decision
  - Summary: Provisional Work Frontier Reduction And Transport Convention
  - Status: draft/local

---

# Work Frontier, Reduction And Transport Convention — Provisional

This is a candidate refinement to the existing Business Work Area Decision, prepared from a qualified read-only carrier and user-supplied observations. It is **not** a landed Tiinex Decision or permission to modify remote sources. Sigma must review the exact text and owner before acceptance.

## Decision

- State: provisional; pending Sigma review and acceptance
- Subject: work-frontier topology, local filename dimensions, Handoff placement, and Reduction defaults for future Tiinex work
- Decision: Use one descriptive `.topics/work/<bounded-task-handle>/` directory for each durable, bounded execution Task frontier in its natural owning Workspace. Its initial `001-...task.trace.md` is directly anchored by a truthful, qualified Parent to the governing Business Project, except where a separately qualified direct continuation or domain-native exception applies. Within that directory, further Task, Handoff, Evidence, Feedback, Decision and Return artifacts normally continue the immediately causal prior artifact through a declared Parent rather than becoming unrelated siblings for every new model turn. Create siblings for genuinely parallel, separately scoped or independent work; do not invent false causality just to produce a straight chain. Do not add a subdirectory for each subtask by default. Numeric dimensions are local to each directory; semantic Parent may cross a directory or Workspace boundary without inheriting its filename dimensions.
- Handoff Placement: An ordinary execution Handoff belongs in the owning `work/<task-handle>/` lineage at its actual transfer boundary, not in a general `handoffs/` collection. An independent Handoff only belongs elsewhere when a qualified owner and real semantics require it. A participant transfer is represented using qualified Handoff semantics and the canonical Handoff Package; passing a package onward without a new Handoff does not change the original route. A checkpoint without responsibility transfer must not invent a Handoff.
- Reduction Placement: The default is a flat `.topics/reductions/` area with a growing qualified Reduction continuity chain (`001`, `001-1`, `001-1-1`, ...), which may itself be consolidated according to qualified retention/recovery rules. Multiple independent Reduction chains (`002`, `003`, ...) are allowed when semantically warranted. Do not create subject subdirectories as the default. Preserve exact source evidence and integrity/recovery obligations; a directory move or local-dimension reset is never itself proof of reduced history, completion or authority.
- Clean Start: Preserve qualified canonical authority, applicable process and role material, and current explicit obligations. Prefer qualification and Reduction of historical execution tracks over broad cosmetic migration when exact historical material is recoverable. Begin genuinely resumed or new work with an explicitly grounded current Task frontier rather than reactivating old `ready/local` chronology. Schemas retain their independent Root-led ancestry; development work on schemas remains accountable through qualified organizational work ancestry.

## Basis

- Parent-backward traversal is the lowest-cost cold-start recovery path. Flat same-parent model turns obscure the causal history and prevent line-length/branching observations used to judge lineage health.
- The accepted prior Business Decisions already require Workspace-local Work Areas and qualified cross-Workspace Project/Task ancestry. This refinement narrows the defaults for Reduction placement and Handoffs without making path names semantic authority.
- Observed carried Core `.topics/work/001-deterministic-lineage-maintenance-projection-and-apply-task.trace.md` has ten direct numbered children, including Evidence and Handoffs. This is a concrete candidate for a historical Reduction, not permission to falsify its ancestry.
- Historic Native `.topics/handoffs/` mixes transfers across several work contexts. Its current Tooling-to-Sigma `020` return remains a separate human acceptance gate and must not be disrupted by cleanup.

## Consequences

- New Tiinex work uses one Task-local Work Area and a truthful qualified Business Parent; branching follows actual distinct scope/causality rather than authoring-turn numbering.
- Current Native Scaffold remains a structural capability, not an automatically applicable lineage policy. Qualified Business Process/Decision grounding and active Task authority govern actual application.
- Existing What/Where Entry discovery and typed Process topology remain intact; this candidate does not turn filename/Parent order into executable Process applicability.
- Existing historical path references remain valid source material until exact qualification and separate authorized Reduction/Move. Existing accepted files are not rewritten merely to make examples symmetric.
- On an actual transfer, the Handoff and receiving Role/capacity are separately qualified and carried through canonical Tooling-manufactured Handoff Package; no loose markdown file substitutes for a transfer carrier.

## Review Conditions

- Sigma reviews this proposed default and determines whether it should be accepted and which source or successor artifact owns the landed rule.
- Verify no conflicting applicable schema/Process contract, and distinguish `work/` execution topology from reusable Process topology.
- Test one fresh Task → Handoff → Evidence → Feedback → Return → Decision continuation and a genuine sibling subtask; ensure Parent traveral recovers work without side exploration.
- Verify directory-local dimensions under cross-Workspace Parent and no invented upstream acceptance/currentness.
- Verify lifecycle, archive/retention and canonical Handoff Package transport in a blind cold start with no conversational hinting.
- Do not authorize publication, migration, deletion, or remote mutation through this provisional record.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-entry-what-where-and-workspace-work-area-structure.trace.md](001-2-entry-what-where-and-workspace-work-area-structure.trace.md)
  - Value: rvEKaBdQ8YjpfmiD6bOibLvBOVXTYIOzJ4PtR5lB67w

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: uGcUoO29aFa3wM_hHxFcxuafhVzafMXf5-iFEst-5eE