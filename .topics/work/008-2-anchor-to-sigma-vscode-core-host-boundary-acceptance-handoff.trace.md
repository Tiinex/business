# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-04 22:09:08
  - Trace: [008-close-vscode-core-host-boundary-regressions-task.trace.md](008-close-vscode-core-host-boundary-regressions-task.trace.md)
  - Origin:
    - [relative](008-close-vscode-core-host-boundary-regressions-task.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-10-04 22:10:25
  - Authors: Anchor; Sigma
  - Why: Verify the remaining boundary-contract fixes without making Sigma debug implementation.
  - Summary: Transfer the final real-host acceptance of the repaired VS Code Core/host boundary before stable Major.
  - Status: ready/local

---

# Anchor To Sigma VS Code Core Host Boundary Acceptance Handoff

## Handoff Parties

- Purpose: transfer the final real VS Code acceptance of the repaired Core/host boundary before the stable Major
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)
- Notes: Sigma remains an ordinary recipient and is not expected to debug implementation

## Transfers

- vscode-core-host-boundary-acceptance
  - Transfer Kind: work-and-responsibility
  - Description: confirm the remaining real Extension Host UX and packaging behavior after the Core/host boundary repair, then return a compact disposition
  - Controlling Artifact: [Close VS Code Core Host Boundary Regressions](008-close-vscode-core-host-boundary-regressions-task.trace.md)
  - Boundary: observation/acceptance only; implementation repair remains with Anchor

## Required Context

- controlling-task
  - Material: current boundary-repair Task
  - Material Reference: [Close VS Code Core Host Boundary Regressions](008-close-vscode-core-host-boundary-regressions-task.trace.md)
  - Purpose: exact regressions, candidate changes, machine evidence, and boundaries
  - Availability: available

- grounding-applicability
  - Material: exact applicability Relation for this Task
  - Material Reference: [VS Code Core Host Boundary Acceptance Guidance Applicability](008-1-vscode-core-host-boundary-acceptance-guidance-applicability-relation.trace.md)
  - Purpose: explicit grounding/recipient guidance selection
  - Availability: available

- current-vscode-workspace
  - Material: exact repaired VS Code Workspace carried by this package
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: explicit selected-Core runtime, Outgoing source exclusivity, Handoff preview, and routed Major host-wiring changes
  - Availability: available

- current-core-workspace
  - Material: exact current Core Workspace carried by this package
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: unchanged semantic authority consumed by the repaired host boundary
  - Availability: available

- portable-grounding-process
  - Material: Portable Session Grounding And Continuity
  - Material Reference: [Portable grounding process](native::.topics/.processes/session-grounding-and-continuity/001-session-grounding-and-continuity-process.trace.md)
  - Purpose: recipient and recovery discipline
  - Availability: available

- tiinex-grounding-profile
  - Material: Tiinex Session Grounding And Continuity Profile
  - Material Reference: [Tiinex grounding profile](../processes/session-grounding-and-continuity/001-session-grounding-and-continuity-process.trace.md)
  - Purpose: Anchor/Sigma acceptance boundary
  - Availability: available

- chatgpt-host-adaptation
  - Material: ChatGPT Session Continuity And Source Discipline
  - Material Reference: [ChatGPT continuity process](interop-openai::.topics/.processes/chatgpt-session-continuity/001-chatgpt-session-continuity-and-source-discipline-process.trace.md)
  - Purpose: one-Package delivery and current-host continuity
  - Availability: available

## Reference Context

- readiness-project
  - Material: Grounding And Continuity Readiness Project
  - Material Reference: [Grounding And Continuity Readiness](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Purpose: organizational lineage for the repaired grounding/host workflow and the next stable-Major continuation
  - Availability: available

- prior-polish-task
  - Material: prior final transport polish Task
  - Material Reference: [Finish Handoff Package Transport And VS Code Presentation Polish](007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md)
  - Purpose: prior accepted transport/presentation fixes retained as context, not reopened by this boundary repair
  - Availability: available

## Sigma Acceptance Surface

1. Merge only the Workspaces listed beside the delivered Handoff Package.
2. Run `Tiinex: Switch all to Local`, then the unchanged `Tiinex: Build linked extension`, then restart/reload the extension.
3. Create an Outgoing from the carried Parent. Incoming Parent Workspaces should be selected by default; Local alternatives should not be co-selected automatically.
4. Select one changed Local Workspace as a replacement. The same Workspace identity must not remain selected from both Local and Incoming sources. A byte-identical Local/Incoming pair should keep Embedded/Incoming.
5. Click a Handoff from both normal semantic navigation and, if convenient, the Files projection. It should open VS Code Markdown Preview first; source remains available through normal VS Code Markdown controls/fallback.
6. Pack the normal multi-Workspace Outgoing. `selected-core-runtime` must not conflict with an open Local Core. Files projection/preview should be usable after the pack boundary is available.
7. If testing an explicit Major with an existing higher same-prefix carrier filename, VS Code should pass the observed filename facts and Core should determine the next Major consistently.

Return pass/fail/observation only. A video is sufficient for a failure. Do not debug source.

## Retained Responsibilities

- anchor-debug-and-repair
  - Retained By: Anchor
  - Responsibility: diagnose and repair any implementation or contract issue returned by Sigma
  - Boundary: Sigma provides the observation, not source isolation or patches

## Exclusions And Dependencies

- remote-mutation
  - Kind: excluded-scope
  - Description: commit, push, publication, release, deployment, and other remote writes are not authorized by this Handoff
  - Responsible Party Or Role: separately authorized operator after acceptance

- broad-audit-refactoring
  - Kind: excluded-scope
  - Description: artifactTree parser ownership, operatorTrees decomposition, Core primitive deduplication, and full test-harness migration are deferred to the next Major
  - Responsible Party Or Role: next bounded Anchor work after stable checkpoint

## Completion Expectation

- Signal Kind: disposition
- Signal Meaning: report whether Parent-default source selection, exclusive replacement, Handoff Preview, Files/Pack, explicit selected-Core manufacture, and routed Major behavior are correct in the real Extension Host
- Return To: Anchor
- Return To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- Notes: a failure returns to Anchor for repair; Sigma is not a debugger

## Interpretation Limits

- Does Not Mean: audit feedback is semantic authority, broad technical debt is resolved, machine evidence substitutes for real-host acceptance, or this progression is automatically the stable Major
- Must Not Be Used To Claim: remote-write authority, publication readiness, or closure of deferred next-Major audit work
- Authority Limits: Core remains semantic authority; VS Code supplies UI, filesystem, Git, user-interaction, and environment facts
- Transport Limits: normal delivery is one Handoff Package plus exact Tooling routing text

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [008-close-vscode-core-host-boundary-regressions-task.trace.md](008-close-vscode-core-host-boundary-regressions-task.trace.md)
  - Value: KfsUro27pVH6q7i9o17FcPffMAa0chlCd63ObNlYPMg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: MaQojI5_g7tPbzO7dZe8a_8gH67yHzK1hy3dVMTdr_Q