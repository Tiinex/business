# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-05 00:57:54
  - Trace: [014-final-vscode-pre-major-acceptance-task.trace.md](014-final-vscode-pre-major-acceptance-task.trace.md)
  - Origin:
    - [relative](014-final-vscode-pre-major-acceptance-task.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-10-05 00:57:55
  - Authors: Anchor; Sigma
  - Why: Let Sigma perform the final operator acceptance without becoming the debugger before an explicit stable-Major checkpoint.
  - Summary: Transfer the final combined VS Code/Core pre-Major acceptance candidate to Sigma through the normal recoverable recipient flow.
  - Status: ready/local

---

# Anchor To Sigma Final VS Code Pre-Major Acceptance Handoff

## Handoff Parties

- Purpose: transfer the one bounded final VS Code/Core pre-Major acceptance Task to Sigma
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)

## Transfers

- final-vscode-pre-major-acceptance
  - Transfer Kind: work-and-responsibility
  - Description: exercise the combined final operator candidate and return pass/fail observations without debugging implementation
  - Controlling Artifact: [Final VS Code Pre-Major Acceptance](014-final-vscode-pre-major-acceptance-task.trace.md)
  - Boundary: acceptance observation only

## Required Context

- controlling-acceptance-task
  - Material: current bounded acceptance Task
  - Material Reference: [Final VS Code Pre-Major Acceptance](014-final-vscode-pre-major-acceptance-task.trace.md)
  - Purpose: exact acceptance frontier and completion boundary
  - Availability: available
- source-preset-task
  - Material: five-mode Parent source-preset implementation Task
  - Material Reference: [Finish Outgoing Parent Source Presets Before Stable Major](012-finish-outgoing-parent-source-presets-before-stable-major-task.trace.md)
  - Purpose: exact five-mode interaction and no-Parent boundary
  - Availability: available
- operator-convenience-task
  - Material: dirty-workspace/build-shortcut/package-Guided-Entry implementation Task
  - Material Reference: [Finish Dirty Workspace Controls, Build Shortcuts, And Package Guided Entry Before Stable Major](013-finish-dirty-workspace-controls-build-shortcuts-and-package-guided-entry-before-stable-major-task.trace.md)
  - Purpose: exact dirty Replace, reset, build shortcut, and recipient-entry behavior under acceptance
  - Availability: available
- applicability-relation
  - Material: exact applicability Relation for this acceptance
  - Material Reference: [Final VS Code pre-Major acceptance applicability](014-1-final-vscode-pre-major-acceptance-grounding-applicability-relation.trace.md)
  - Purpose: selected grounding/recipient guidance
  - Availability: available
- current-vscode-workspace
  - Material: exact current VS Code Workspace carried by this package
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: current host/UI candidate bytes under acceptance
  - Availability: available
- current-core-workspace
  - Material: exact current Core Workspace carried by this package
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: qualified pointerless/routed Guided Entry transport projection under acceptance
  - Availability: available

## Reference Context

- readiness-project
  - Material: Grounding And Continuity Readiness Project
  - Material Reference: [Grounding And Continuity Readiness](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Purpose: organizational lineage for this final checkpoint and next-Major continuation
  - Availability: available

## Sigma Acceptance Surface

1. Use the normal Incoming/Replace flow, Switch/build/reload normally.
2. Parent-backed Outgoing: use the dedicated `Source preset` button and confirm `Incoming only -> None -> Prefer Local -> Prefer Incoming -> Local only -> Incoming only`, with one source per Workspace identity.
3. Dirty Replace: make one Git Workspace dirty, choose Replace, and confirm `Discard local changes` is the final dirty-resolution choice and cleans to committed HEAD before Replace proceeds.
4. Global reset: make multiple Git Workspaces dirty, run `Tiinex: Reset All Dirty Workspaces`, confirm No is active/default and Yes is below it; choose Yes and confirm dirty repos become clean while ignored files remain.
5. Build shortcuts: confirm the existing `Tiinex: Build linked extension` still works. Confirm Local runs Switch all to Local before `dev:build` and is default test; Latest runs Switch all to Latest before `dev:build` and is default build. Link/Unlink stays unchanged.
6. Transport package row: confirm `Guided Entry` is available on a pointerless Workspace carrier and on this routed Handoff carrier. For the routed carrier, Start should retain the carried Continue From route while adding Start Entry intent.
7. Handoff Pointer row: confirm `Copy Transport Text` remains available for the exact route. The routed package row itself should use Guided Entry rather than a duplicate raw-copy action.

Return a compact pass/fail observation or silent video. Do not debug implementation.

## Retained Responsibilities

- anchor-repair
  - Retained By: Anchor
  - Responsibility: diagnose and repair any implementation issue returned by Sigma
  - Boundary: Sigma provides observations, not source isolation or patches

## Exclusions And Dependencies

- remote-mutation
  - Kind: excluded-scope
  - Description: commit, push, publication, release, deployment, and other remote writes are not authorized by this Handoff
  - Responsible Party Or Role: separately authorized operator after acceptance
- next-major-audit-remediation
  - Kind: excluded-scope
  - Description: Core↔host contract consolidation, test-baseline restoration, source-shape test migration, and broader audit work begin only after the stable checkpoint
  - Responsible Party Or Role: future bounded Anchor work

## Completion Expectation

- Signal Kind: disposition
- Signal Meaning: report whether the bounded final acceptance Task passes or which concrete user-visible behavior blocks it
- Return To: Anchor
- Return To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: package-level Guided Entry changes the selected Handoff route, pointer-level Copy Transport becomes obsolete, this Handoff authorizes remote mutation, or this package itself creates the stable Major
- Must Not Be Used To Claim: stable-Major acceptance before Sigma returns disposition
- Transport Limits: normal delivery is one Handoff Package plus Tooling-projected recipient entry/routing surfaces

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [014-final-vscode-pre-major-acceptance-task.trace.md](014-final-vscode-pre-major-acceptance-task.trace.md)
  - Value: AQnxxwQWFKI-_Fii7Pt42mMcMser-RRQLuLc8NeEZJk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: QmhwjQuraYyrKSszWQbUeVA4ZqgI9Tu4PfuBBhxGXJM