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
  - Created At: 2026-10-04 20:08:53
  - Authors: Anchor; Sigma
  - Why: The same physical Local Core was being treated as multiple implementations across linked/multi-root host coordinates.
  - Summary: Collapse equivalent Core host paths to one physical runtime source and restore Incoming qualified matches, Replace, Initialize, and Outgoing Pack.
  - Status: ready/local

---

# Eliminate VS Code Core Alias Ambiguity In Standard Workflow

## Objective

Restore the ordinary Incoming qualified-match, Replace, Initialize, Outgoing New, and Pack flow when Local dependency mode and the multi-root VS Code host expose the same physical Core checkout through more than one host path.

## Root Cause

The host treated path-string uniqueness as Core implementation uniqueness. In linked/multi-root development the same physical Core can be present through the dependency-mode path, an open Workspace path, and a junction/symlink/casing variant. That produced `tiinex.core-source-runtime.ambiguous`, which then caused Incoming delta projection to degrade exact local matches to unavailable, Replace to lose automatic identity mapping, and Outgoing New/Pack to block.

## Candidate Changes

- Canonicalize candidate Core roots to physical filesystem identity before deciding source ambiguity; Windows comparison is case-insensitive.
- Preserve fail-closed ambiguity when two genuinely different physical Core checkouts are present.
- Use `prepareHostCoreRuntime` for Incoming qualified-match/delta projection instead of a separate bundled runtime.
- Do not silently convert a shared host-runtime qualification failure into a full set of innocent-looking unavailable Workspace deltas.
- Use the shared Host Core runtime for the Outgoing manufacture fallback so Local mode, open Workspace roots, and content-source composition remain consistent.
- Keep `Switch all to Local`, `Switch all to Latest`, and `Build linked extension` task contracts unchanged from the preceding candidate.

## Anchor Machine Acceptance

- Same physical Core via direct path plus symlink alias resolves to one runtime.
- Two physically distinct Core checkouts still produce `tiinex.core-source-runtime.ambiguous`.
- A real carried `app` Workspace extracted from the incoming carrier compares `exact` against its identical local root and therefore qualifies for the green `qualified match` UI state.
- Replace auto-discovers and qualifies that already-open `app` Workspace without a folder prompt.
- Initialize remains ready under the aliased Local Core for no Git, Git without origin, and Git with origin.
- VS Code host Outgoing manufacture succeeds for `app`, `core`, `interop-openai`, and `native` while the same Core is also exposed through an alias; Core orientation reports ready, bootstrap valid, and zero findings.
- The produced host carrier passes ZIP integrity and Core re-orientation.

## Dependencies

- [Grounding And Continuity Readiness](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- [Restore VS Code Workspace Workflow After Content Composition Cutover](004-restore-vscode-workspace-workflow-after-content-composition-cutover-task.trace.md)
- Current carried VS Code/Core/Native/OpenAI Interop Workspaces.

## Scope

- VS Code host runtime physical-source identity.
- Incoming exact-match/qualified-match projection.
- Replace automatic mapping.
- Initialize under Local composition.
- Outgoing New/Pack under Local composition.
- Durable regression coverage for the alias boundary.

## Done Criteria

- Already-merged exact Workspaces render as qualified matches instead of unavailable when Local Core is reachable through equivalent host paths.
- Replace does not ask for a folder when an exact qualified open Workspace is already available.
- Initialize remains valid for all three supported source forms.
- Outgoing New/Pack does not fail merely because the same Core checkout has multiple host coordinates.
- Real distinct Core implementations still fail closed as ambiguous.
- Sigma needs only the smallest real Windows/Extension Host observation and is not the debugger.

## Manual Merge Boundary

This progression changes only two Workspaces relative to its parent carrier:

1. `business` — Task/Handoff lineage for the acceptance transfer.
2. `vscode` — product/runtime and regression-test changes.

All other Workspaces are inherited unchanged for full recovery and do not need manual merge for this candidate.

## Boundaries

- Physical-path canonicalization does not make repository identity authoritative for Workspace identity.
- No Core, Native, or Interop product source change is part of this repair.
- No commit, push, publication, release, or remote mutation is authorized.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 7ZRumXJhc55fXzmTB1h4ZhVqWdeZOWysDkFIFrmZT_M