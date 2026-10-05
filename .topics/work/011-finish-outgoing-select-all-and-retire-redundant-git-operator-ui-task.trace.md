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
  - Created At: 2026-10-04 23:24:04
  - Authors: Anchor; Sigma
  - Why: Close the final user-visible VS Code polish before stable Major without reopening accepted Core or packaging behavior.
  - Summary: Make Outgoing Select All prefer explicit Local sources while retaining Incoming only where Local is absent, and remove the redundant multi-repository review/commit/push command and form.
  - Status: ready/local

---

# Finish Outgoing Select-All And Retire Redundant Git Operator UI

## Objective

Close the final user-visible VS Code polish before the stable Major by making Outgoing `Select All` preserve Local Workspace sources wherever they exist, retaining Incoming only for Workspace identities with no Local source, and removing the redundant multi-repository Stage/Review/Commit/Push command and its review form.

## Observed Behavior

Sigma verified that `Tiinex: Stage All Workspaces` now performs the desired direct multi-repository staging behavior. Two small UX deviations remained:

- In `Select Outgoing Workspaces`, using VS Code's Select All control selected both Local and Incoming candidates and the exclusive-source resolver then preferred byte-identical Incoming for identities that also had Local, so Local selections disappeared immediately.
- The older `Tiinex: Stage, Review, Commit & Push Repositories` command and its dedicated form were still exposed even though the existing post-stage automation already owns that complete workflow and Stage All now covers the desired manual staging primitive.

## Candidate Changes

- Keep Outgoing source selection exclusive per Workspace identity.
- Treat the source newly selected by the operator as the winner before the byte-identical Incoming fallback. This means Select All yields Local where Local exists and leaves Incoming selected only where there is no Local candidate.
- Keep the separate Guided Entry rule unchanged: byte-identical carried/embedded Entry deduplication remains a Core projection where embedded wins deterministically.
- Remove the `tiinex.stageCommitPushMany` command contribution and registration.
- Remove the dedicated multi-repository Git review-form implementation used only by that command.
- Keep `Tiinex: Stage All Workspaces` and the existing automatic post-stage Git workflow unchanged.

## Acceptance Evidence

Anchor verified the Outgoing selection resolver directly with a Parent-style Incoming baseline:

- Local + Incoming are available for `core` and `docs`.
- Incoming-only is available for `remote`.
- Selecting all candidates resolves to Local `core`, Local `docs`, and Incoming `remote`.
- Explicitly selecting Incoming while Local is already selected switches that one identity to Incoming, proving explicit operator intent still wins.

Anchor also verified command-surface cleanup:

- `tiinex.stageAllWorkspaces` remains contributed.
- `tiinex.stageCommitPushMany` is no longer contributed or registered.
- the dedicated review-form module is removed.
- the retained Stage All primitive still performs real `git add -A` across two Git repositories and leaves no unstaged changes.

## Scope

- VS Code Outgoing source-selection presentation/interaction only.
- VS Code Git command surface cleanup only.
- Durable Task/Handoff continuity for Sigma acceptance.

## Dependencies

- [Repair Stage All Workspaces Command Registration Before Stable Major](010-repair-stage-all-workspaces-command-registration-task.trace.md)
- Current carried Core Workspace with Guided Entry byte-identical deduplication already accepted as candidate behavior.
- Current carried VS Code Workspace.

## Done Criteria

- Outgoing Select All selects Local for every Workspace identity with a qualified Local source.
- Incoming remains selected for identities that have no Local source.
- A Workspace identity cannot remain double-selected.
- Explicitly selecting the alternate source switches only that identity.
- `Tiinex: Stage All Workspaces` remains available and stages all changes without review/commit/push UI.
- `Tiinex: Stage, Review, Commit & Push Repositories` and its dedicated form are absent.
- No Core, packaging, carrier, Replace, Initialize, Guided Entry, or Major-allocation behavior changes.

## Boundaries

- No remote mutation is authorized by this Task.
- Do not refactor the broader Core↔host boundary or verification debt in this pre-Major polish Task; that is next-Major work informed by the separate audit.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 6l-nyo-jhLMa8EQ3XSZwdzQHObdZ24N88Izy4JvjWFo