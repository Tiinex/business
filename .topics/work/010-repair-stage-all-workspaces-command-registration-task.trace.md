# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-10-04 02:20:00
  - Trace: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Origin:
    - [relative](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-04 22:58:46
  - Authors: Anchor; Sigma
  - Why: Close the final observed compile-time wiring defect without reopening accepted staging or Guided Entry semantics.
  - Summary: Repair the missing VS Code import that blocked the linked-extension build for Stage All Workspaces.
  - Status: ready/local

---

# Repair Stage All Workspaces Command Registration Before Stable Major

## Objective

Repair the final VS Code command-wiring defect discovered by Sigma during the real linked-extension build acceptance without reopening the accepted Guided Entry, packaging, Workspace, carrier, or host-boundary behavior.

## Observed Defect

The candidate registered `tiinex.stageAllWorkspaces` in `src/extension.ts` and implemented/exported `stageAllWorkspacesCommand()` from `src/commit.ts`, but `extension.ts` did not import that exported symbol. The real `Tiinex: Build linked extension` therefore failed TypeScript compilation with `TS2304: Cannot find name 'stageAllWorkspacesCommand'` before the operator could execute the command.

## Candidate Change

- Add `stageAllWorkspacesCommand` to the existing named import from `./commit` in `src/extension.ts`.
- Do not change the command implementation, Git behavior, command identifier, package contribution, Build linked extension task, Guided Entry deduplication, Core semantics, packaging, carrier lineage, Replace, Initialize, or Outgoing behavior.

## Acceptance Evidence

Anchor verified the repaired candidate at the TypeScript symbol boundary: `src/extension.ts` now imports the exact exported `stageAllWorkspacesCommand` symbol from `src/commit.ts`, and a TypeScript semantic diagnostic check no longer reports that symbol as unresolved.

The current container still does not substitute for Sigma's actual Windows linked-extension build because the full local VS Code dependency install is not available here. The remaining real-host acceptance is intentionally one build plus one Stage All execution.

## Scope

- VS Code command registration/import wiring only.
- Durable Task/Handoff continuity for Sigma acceptance.

## Dependencies

- [Finish Workspace Staging And Guided Entry Deduplication Before Stable Major](009-finish-workspace-staging-and-guided-entry-deduplication-task.trace.md)
- Current carried VS Code Workspace candidate.

## Done Criteria

- `Tiinex: Build linked extension` compiles past the previous `TS2304` error.
- `Tiinex: Stage All Workspaces` is available and executes the already-accepted staging implementation.
- The command opens no review/commit/push form and performs no commit or push.
- No unrelated workflow behavior changes.

## Boundaries

- No Core source change.
- No Guided Entry semantic change.
- No package/carrier/Workspace lineage change.
- No remote mutation is authorized by this Task.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: ku3HQx5pun22FM0kiclMfNHVMx8PL0Se5h3Q0te5K3U