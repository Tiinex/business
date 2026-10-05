# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-05 01:26:02
  - Trace: [015-make-local-and-latest-linked-builds-portable-npm-flows-task.trace.md](015-make-local-and-latest-linked-builds-portable-npm-flows-task.trace.md)
  - Origin:
    - [relative](015-make-local-and-latest-linked-builds-portable-npm-flows-task.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-10-05 01:26:16
  - Authors: Anchor; Sigma
  - Why: Close the final linked-build regressions through the normal human-recipient Handoff flow before stable Major.
  - Summary: Transfer the portable Local/Latest linked-build repair, including optional unpublished content-source handling, to Sigma for real-host acceptance.
  - Status: ready/local

---

# Anchor To Sigma Portable Linked Build Repair Acceptance Handoff

## Handoff Parties

- Purpose: transfer the repaired Local/Latest portable npm build flows to Sigma for one real VS Code task-discovery/build acceptance
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)

## Transfers

- portable-linked-build-acceptance
  - Transfer Kind: work-and-responsibility
  - Description: confirm all three linked-build tasks are independently discoverable, Local composes the local Tiinex surface, and Latest uses published latest dependencies/content sources without being blocked by optional unpublished content packages
  - Controlling Artifact: [Make Local And Latest Linked Builds Portable NPM Flows](015-make-local-and-latest-linked-builds-portable-npm-flows-task.trace.md)
  - Boundary: real-host acceptance only; Sigma is not asked to debug implementation

## Required Context

- controlling-task
  - Material: portable Local/Latest linked-build repair Task
  - Material Reference: [Portable linked-build repair](015-make-local-and-latest-linked-builds-portable-npm-flows-task.trace.md)
  - Purpose: exact regressions, dependency/content-source boundary, candidate contract, and acceptance evidence
  - Availability: available
- applicability-relation
  - Material: exact current applicability Relation
  - Material Reference: [Portable linked-build repair applicability](015-1-portable-linked-build-repair-acceptance-grounding-applicability-relation.trace.md)
  - Purpose: selected grounding/recipient guidance
  - Availability: available
- current-vscode-workspace
  - Material: exact repaired VS Code Workspace
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: package scripts, dependency-mode implementation, and VS Code task definitions under acceptance
  - Availability: available

## Reference Context

- prior-final-acceptance
  - Material: preceding final VS Code pre-Major acceptance
  - Material Reference: [Final VS Code Pre-Major Acceptance](014-final-vscode-pre-major-acceptance-task.trace.md)
  - Purpose: retain all previously accepted candidate behavior while repairing only build portability and Latest content-source availability handling
  - Availability: available

## Sigma Acceptance Surface

1. Use normal Incoming/Replace and reload the linked extension/workspace as usual.
2. Open VS Code task discovery and search for `Build`.
3. Confirm all three are independently present:
   - `Tiinex: Build linked extension`
   - `Tiinex: Build linked extension (Local)`
   - `Tiinex: Build linked extension (Latest)`
4. Run Local. It should compose the complete local Tiinex dependency/content-source surface and then execute the existing `dev:build` build.
5. Run Latest. Required package dependencies should use npm `@latest`. Registered content sources that have a published latest should use it; currently unpublished optional content sources may be reported as omitted and must not cause npm E404 to abort the build.
6. Latest must not silently retain a Local content-source link when that content source is omitted as unpublished.
7. The neutral Build task should retain its prior behavior and must not implicitly switch dependency mode.

Return a compact pass/fail observation or silent video. Do not debug implementation.

## Retained Responsibilities

- anchor-repair
  - Retained By: Anchor
  - Responsibility: repair any implementation issue returned by Sigma
  - Boundary: Sigma provides observation only

## Exclusions And Dependencies

- remote-mutation
  - Kind: excluded-scope
  - Description: commit, push, publication, release, deployment, and other remote writes are not authorized
  - Responsible Party Or Role: separately authorized operator after acceptance
- next-major-audit-remediation
  - Kind: excluded-scope
  - Description: grounding/audit continuation begins only after stable-Major acceptance
  - Responsible Party Or Role: future bounded Anchor work

## Completion Expectation

- Signal Kind: disposition
- Signal Meaning: report whether all three tasks are visible, Local builds from the local Tiinex composition, and Latest builds from published latest material without optional unpublished content-source E404 failure
- Return To: Anchor
- Return To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: an omitted unpublished content source has a published equivalent, Latest is allowed to use Local bytes as fallback, this Handoff authorizes remote mutation, or this Handoff itself creates the stable Major
- Must Not Be Used To Claim: stable-Major acceptance before Sigma returns disposition

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [015-make-local-and-latest-linked-builds-portable-npm-flows-task.trace.md](015-make-local-and-latest-linked-builds-portable-npm-flows-task.trace.md)
  - Value: arLyKrZ3g2TBsSLPhYPwjkLCswnEE9ASW_eFAj_g4xE

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: LSovKt7jANenUqnXzKCLimTC1LLnimwsMnMGYzLJzEw