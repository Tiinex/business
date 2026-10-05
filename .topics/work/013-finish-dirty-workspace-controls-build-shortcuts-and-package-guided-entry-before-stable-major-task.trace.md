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
  - Created At: 2026-10-05 00:57:26
  - Authors: Anchor; Sigma
  - Why: Close the remaining operator conveniences before the stable Major without reopening accepted carrier, Workspace, or package topology behavior.
  - Summary: Finish dirty Replace/reset controls, Local/Latest build shortcuts, and package-level Guided Entry for pointerless and routed carriers while retaining pointer-level raw transport.
  - Status: ready/local

---

# Finish Dirty Workspace Controls, Build Shortcuts, And Package Guided Entry Before Stable Major

## Objective

Close the remaining operator-facing VS Code work before the stable Major without reopening accepted Workspace, Replace, carrier-lineage, Major-allocation, or Package V1 topology behavior.

This Task combines four bounded conveniences that belong to the current operator workflow:

- add an explicit destructive `Discard local changes` option to dirty Replace;
- add one safe global `Reset All Dirty Workspaces` Git command;
- add Local/Latest linked-build shortcut tasks without changing the existing linked build mechanics;
- restore one package-level `Guided Entry` recipient action for both pointerless Workspace carriers and qualified routed Handoff carriers while retaining exact `Copy Transport Text` on individual Handoff Pointer rows.

The five-mode Parent-backed Outgoing source preset remains governed by Task 012 and is carried unchanged into the same final acceptance session.

## Dirty Replace

When Incoming Replace reaches a dirty Git Workspace, the precondition picker keeps the existing non-destructive choices and adds `Discard local changes` as the final option.

Discard means:

- reset tracked material to committed `HEAD`;
- remove untracked non-ignored material;
- preserve ignored material;
- continue Replace only after the repository verifies clean.

No branch change, commit, push, or Tiinex semantic mutation is implied by this choice.

## Reset All Dirty Workspaces

Expose `Tiinex: Reset All Dirty Workspaces` as a global VS Code command over Git repositories already known through VS Code's Git surface.

The command:

1. inspects only those repositories;
2. selects only dirty roots;
3. shows a confirmation picker with `No` active/default and `Yes` below it;
4. performs no mutation when `No` or Esc is chosen;
5. when `Yes` is chosen, applies the same verified discard primitive to every dirty Git Workspace.

The command performs no commit, push, publication, branch change, package operation, or Tiinex semantic qualification.

## Linked-build shortcuts

Keep the existing `Tiinex: Build linked extension` task mechanics intact: it remains `dev:build` after the existing `Tiinex: npm install` dependency.

Add two shortcut tasks:

- `Tiinex: Build linked extension (Local)`
  - pre-task: `Tiinex: Switch all to Local`
  - then `dev:build`
  - default `test` task
- `Tiinex: Build linked extension (Latest)`
  - pre-task: `Tiinex: Switch all to Latest`
  - then `dev:build`
  - default `build` task

Link/Unlink tasks are unchanged. The Switch-all tasks continue to own full dependency-chain switching/install behavior; the shortcuts do not invent a second linking mechanism.

## Package Guided Entry And Pointer Transport

The Transport tree distinguishes two recipient surfaces:

### Package row

`Guided Entry` is the normal package-level recipient action for both:

- pointerless Workspace carriers; and
- qualified routed Handoff carriers.

For a routed Handoff carrier, Core qualifies the selected Handoff route and preserves its exact Start + Continue From transport shell. Guided Entry then adds the selected reusable Entry / Custom session intent above that unchanged routing authority.

If a package carries multiple qualified Handoff routes, package-level Guided Entry requires an explicit route choice before rendering Entry transport text.

The routed package row does not need a separate `Copy Transport Text` action once Guided Entry is available there.

### Handoff Pointer row

`Copy Transport Text` remains available on each Handoff Pointer/route row as the exact low-level transport projection for that qualified route.

This preserves an explicit raw-routing capability without duplicating it on the package row.

## Core / Host Ownership

- Core owns whether a carrier is eligible for Guided Entry, exact Handoff route qualification, and composition of Entry intent with qualified transport text.
- VS Code owns package/pointer action presentation, route-choice UI when more than one qualified route exists, clipboard delivery, Git UX, and build-task convenience.
- VS Code does not reconstruct Handoff Start/Continue From semantics.

## Acceptance Evidence

Anchor verified the candidate with focused behavior checks:

- the five Task-012 source presets still project exactly: Incoming only, None, Prefer Local, Prefer Incoming, Local only;
- `Reset All Dirty Workspaces` defaults to No and Yes mutates only dirty Git roots;
- the shared real discard primitive restored tracked bytes to `HEAD`, removed untracked non-ignored material, preserved ignored material, and left the repository clean;
- the original linked-build task retains its `dev:build` + `Tiinex: npm install` mechanics, while Local/Latest shortcuts own only the requested Switch-all pre-task plus `dev:build`;
- the latest routed Anchor→Sigma package produced a ready Core Guided Entry catalog and a ready Start rendering that preserved the exact carried Continue From pointer;
- an existing pointerless Workspace carrier still produced ready Guided Entry Start text;
- VS Code package menus expose Guided Entry for pointerless and routed package rows, hide package-level raw Copy Transport Text, and retain Copy Transport Text on Handoff Pointer rows;
- the modified VS Code source tree passed the available TypeScript syntax/unresolved-name gate.

## Scope

- VS Code dirty Incoming Replace precondition UX.
- VS Code global Git reset convenience over already-known Git repositories.
- VS Code repository-local Local/Latest linked-build shortcut composition.
- Core Guided Entry transport projection for already-qualified pointerless Workspace and routed Handoff carriers.
- VS Code Transport package/pointer action presentation for Guided Entry versus exact raw route transport.
- Preserve the already-carried Task-012 five-mode Parent source preset implementation for the same final acceptance session.

## Dependencies

- [Finish Outgoing Parent Source Presets Before Stable Major](012-finish-outgoing-parent-source-presets-before-stable-major-task.trace.md)
- Current carried Core Workspace.
- Current carried VS Code Workspace.
- Native reusable Entry/content material already composed into the active runtime.

## Done Criteria

- Dirty Replace exposes Discard as its final dirty-resolution choice and verifies the repository clean before Replace continues.
- Reset All Dirty Workspaces defaults to No and Yes cleans all dirty VS Code-known Git repositories to committed HEAD while preserving ignored files.
- Existing `Tiinex: Build linked extension` mechanics remain unchanged.
- Local and Latest build shortcuts perform the corresponding Switch-all task before `dev:build`, with Local default-test and Latest default-build grouping.
- Task-012 five-mode Parent source presets remain intact.
- Package-level Guided Entry works for pointerless and qualified routed Handoff carriers.
- Multi-route Guided Entry requires exact route selection.
- Handoff Pointer rows retain exact Copy Transport Text.
- Package-level routed Copy Transport Text is not separately exposed.
- No carrier lineage, Major allocation, Workspace identity, Replace model, or Package V1 topology change is introduced.

## Boundaries

- This Task extends Core Guided Entry transport projection only enough to accept already-qualified routed Handoff carriers; it does not weaken Handoff qualification or create new Handoff authority.
- No commit, push, publication, release, deployment, or other remote mutation is authorized.
- Broader Core↔host contract consolidation and test-baseline/audit remediation remain next-Major work.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: ylF7nMMFoEoGB8E7rYl6HEUg5IPA8ELbgNaOuI7Gn8Y