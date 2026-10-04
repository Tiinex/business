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
  - Created At: 2026-10-04 22:09:08
  - Authors: Anchor; Sigma
  - Why: Restore one coherent Core/host boundary before promoting the repaired workflow to a stable Major.
  - Summary: Close explicit-Core manufacture ambiguity, Outgoing source duplication, Handoff preview, and routed-Major host contract seams before stable Major.
  - Status: ready/local

---

# Close VS Code Core/Host Boundary Regressions Before Stable Major

## Objective

Close the remaining VS Code regressions at the Core/host boundary without reopening accepted Workspace, artifact-lineage, carrier-lineage, or Package V1 semantics.

The candidate restores one coherent rule: the host observes environment/source facts and Core owns semantic qualification, allocation, and manufacture decisions.

## Observed Regressions

1. During Outgoing manufacture an explicitly selected Incoming Core Workspace was materialized as `selected-core-runtime`, while the same VS Code window also contained a different/open Local Core root. Generic host runtime discovery then treated both as competing Core implementations and blocked with `tiinex.core-source-runtime.ambiguous`, even though source selection had already explicitly chosen one Core for manufacture.
2. Outgoing Workspace selection could present Local and Incoming versions of the same Workspace identity as simultaneously selected. For a Parent-backed Outgoing, the carried Parent Workspaces should be the baseline and Local sources should be explicit replacements.
3. Handoff navigation was not consistently preview-first. Some Handoff paths, including route/file projections, still opened raw Markdown even though the built-in VS Code Markdown Preview is the intended read-first presentation.
4. Routed Handoff + Parent + Major host wiring did not forward the same observed same-prefix carrier filenames that pointerless manufacture already forwarded. That left the same Core allocation invariant with two host contracts.

## Candidate Changes

### Explicit selected Core authority

- Generic host discovery remains fail-closed when it independently discovers more than one physical Core implementation.
- Package manufacture receives a separate explicit-selected-Core runtime boundary.
- When the operator/source plan has already selected a Core Workspace, that selected root is the manufacture runtime.
- Other open Core roots are environment facts only for that operation and are not competing runtime candidates or content roots.
- Non-Core open roots and registered dependency-mode content roots remain available to the selected Core runtime.

### Outgoing source selection

- A Parent-backed Outgoing starts with the Parent-carried Incoming Workspaces selected.
- Local Workspaces begin as alternatives, not implicit co-selections.
- Selecting a Local or Incoming alternative for one Workspace identity deselects the other source for that same identity.
- If Local and embedded Incoming bytes are byte-identical, embedded Incoming remains the deterministic winner.
- Changed Local material can explicitly replace the carried source.

### Handoff Markdown presentation

- Handoff artifact and Handoff file paths prefer VS Code's built-in `markdown.showPreview` command.
- If preview cannot be opened, navigation falls back to exact Markdown source.
- Ordinary non-Handoff Markdown remains source-first.

### Routed Major filesystem facts

- VS Code always forwards the observed carrier filename set for an explicit Major request, including when a Package Parent exists.
- VS Code does not calculate the semantic Major from those names; Core continues to own allocation.
- Pointerless and routed Parent manufacture therefore share the same filesystem-fact contract.

## Acceptance Evidence

Anchor executed focused host/runtime acceptance against the candidate:

- Generic host discovery with two distinct Core roots remained blocked as ambiguous.
- The explicit-selected-Core boundary selected the requested Core snapshot while excluding other Core roots from content composition and retaining non-Core content roots.
- The real VS Code package builder manufactured a pointerless package using an Incoming embedded Core snapshot while a different Local Core was open; no Core ambiguity occurred.
- Source-selection tests confirmed explicit Local/Incoming replacement exclusivity and byte-identical embedded preference.
- A routed Handoff + Package Parent + explicit Major manufacture was run with a locally observed `tiinex-022...` filename; Core allocated and manufactured `tiinex-023-anchor-to-sigma.handoff-package.zip`.
- Modified TypeScript files transpiled without syntax diagnostics.

## Parallel Audit Feedback

A parallel Anchor audit independently identified Core ↔ VS Code boundary-contract duplication as the concentrated technical-debt area, including the mismatch where pointerless manufacture forwarded observed filenames while routed Parent manufacture did not. This Task uses that feedback only to tighten the current boundary contract; broad `artifactTree.ts`, operator-tree, Core duplication, and full test-harness migration work are deferred to the next Major.

## Scope

- VS Code host/runtime composition for explicit Core selection.
- Outgoing Workspace source-selection defaults and exclusivity.
- Handoff read-first Markdown Preview routing.
- Routed Major filesystem-fact parity with pointerless manufacture.
- Focused regression coverage for those boundaries.

## Dependencies

- [Grounding And Continuity Readiness](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- [Finish Handoff Package Transport And VS Code Presentation Polish](007-finish-handoff-transport-and-vscode-presentation-polish-task.trace.md)
- Current carried Core, Native, Business, and VS Code Workspaces.

## Done Criteria

- Explicit selected Core manufacture succeeds even when another Core checkout is open, while generic unselected multi-Core discovery still blocks.
- Parent-backed Outgoing selection begins with Incoming sources and maintains at most one selected source per Workspace identity.
- Byte-identical embedded Incoming material wins deterministically; changed Local material remains an explicit replacement option.
- Handoff clicks from semantic and file projections open built-in Markdown Preview first.
- Routed Parent + Major forwards observed filenames and Core alone allocates the next Major.
- Ordinary Outgoing Pack and Files projection no longer fail because `selected-core-runtime` competes with an open Local Core.
- Sigma can confirm the real Extension Host behavior without debugging source.

## Boundaries

- No Core product semantics are changed by this Task.
- No artifact parser, artifact lineage, semantic Parent ancestry, Workspace identity, carrier lineage model, or Package V1 topology is changed.
- The broader audit findings about duplicated parsing, operator-tree concentration, Core primitive duplication, and test-harness migration remain next-Major work.
- No commit, push, publication, release, or other remote mutation is authorized.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: KfsUro27pVH6q7i9o17FcPffMAa0chlCd63ObNlYPMg