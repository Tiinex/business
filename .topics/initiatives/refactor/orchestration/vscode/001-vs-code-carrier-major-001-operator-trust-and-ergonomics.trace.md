# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-11 12:38:12
  - Trace: [001-stream-day-parallel-major-001-orchestration.trace.md](../001-stream-day-parallel-major-001-orchestration.trace.md)
  - Origin:
    - [relative](../001-stream-day-parallel-major-001-orchestration.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-11 12:43:13
  - Authors: Anchor
  - Why: Sigma supplied current operator feedback and will drive the VS Code lane semi-independently while Anchor retains shared-boundary and Major-closure coordination.
  - Summary: Bound the VS Code Major 001 safety, workflow and finish tranche under Sigma/Kodax dogfood.
  - Status: ready/local

---

# VS Code Carrier Major 001 — Operator Trust And Ergonomics

## Objective

Make the current `extension-vscode` operator workflow safe enough to dogfood without overwrite anxiety and ergonomic enough that Sigma can drive repeated Handoff/receive/land cycles, while preserving shared Tiinex semantics and explicit human acceptance gates.

## Done Criteria

- Pack output uses the canonical projected carrier filename, never silently overwrites an existing ZIP, and has real Windows-host evidence before acceptance.
- Real Handoff artifact authoring is understood and tested end-to-end; extension-local UI consumes shared authoring/package logic where available and returns any missing shared primitive instead of inventing private semantics.
- Incoming Handoff pointers can be intentionally selected/copied into Outgoing for forwarding without changing their semantic authority or implying recipient acceptance.
- Auto staging behaves predictably and is tested before auto commit/push become default workflow assumptions.
- The commit workflow no longer requires unnecessary manual staging solely to obtain a useful generated commit message; auto commit/push are tested only after staging and message generation are trustworthy.
- The extension uses the current Tiinex primary brand asset once exact source bytes are available from the organization branding source.
- Display options collapse into one scalable control that exposes icon + text + toggle state rather than consuming one toolbar button per option.
- README reaches VS Code Marketplace-quality clarity; Sigma receives a deterministic GIF capture runbook after UI behavior stabilizes.
- Incoming Workspace rows that are byte-identical to Local show a green qualified match state directly and do not offer Merge/Replace actions that cannot change state.
- Attach Handoff is reproduced and either qualified or repaired before acceptance.
- Major closure includes explicit Sigma Windows observation; technical PASS alone is not human acceptance.

## Scope

`Tiinex/extension-vscode` implementation, tests, operator UX and its consumption of already-qualified shared Core/Docs contracts. Core/Docs/Site changes are not silently taken over by this lane.

## Ordering

1. Safety: Pack naming/no-overwrite, identical-workspace action suppression, Attach Handoff, auto staging.
2. Workflow: Handoff authoring, pointer forwarding, commit-message/stage/commit/push ergonomics.
3. Finish: display-options menu, branding, README/GIF capture plan.

## Safety Invariants

- Existing output files are never silently replaced.
- Package/Workspace/Handoff semantics come from shared qualified contracts, not filename/UI inference.
- User video/Windows observations are evidence/feedback, not automatic acceptance.
- New defects may reorder work inside this Major when safety-critical, but unrelated feature expansion is deferred to the next carrier Major.
- Auto commit/push remain opt-in/tested behavior until the preceding local workflow is qualified.

## Dependencies

- Current complete `extension-vscode` Workspace from the audited Anchor recovery.
- Current Core and Docs Workspaces for package/authoring/lineage contracts.
- Current Business Workspace for Kodax Role, this Major scope and Sigma/Anchor gates.
- Site may be consulted as read-only comparison context when shared human authoring/package behavior must be reconciled.
- Exact Tiinex primary logo bytes are not currently part of the sixteen-Workspace recovery; branding closure waits for an exact qualified asset source rather than copying a guessed image.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-stream-day-parallel-major-001-orchestration.trace.md](../001-stream-day-parallel-major-001-orchestration.trace.md)
  - Value: XVBIK1Q4XsLJQCqk_bq8MYdQKtMcwCt_2zSdwyHtSKQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: X6UqB50cTIcfgzXPh3UWJYac2PtLPpiwBcCfYIinCjM