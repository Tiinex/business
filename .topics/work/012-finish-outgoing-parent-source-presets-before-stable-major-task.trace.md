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
  - Created At: 2026-10-04 23:57:20
  - Authors: Anchor; Sigma
  - Why: Give Sigma fast deterministic source-selection presets without changing Workspace identity, carrier semantics, or no-Parent behavior.
  - Summary: Add a deterministic five-mode Parent source preset cycle to VS Code Outgoing selection while preserving ordinary no-Parent Local selection behavior.
  - Status: ready/local

---

# Finish Outgoing Parent Source Presets Before Stable Major

## Objective

Finish the final VS Code Outgoing source-selection polish before the stable Major by giving Parent-backed Outgoing selection a deterministic five-mode source preset cycle while leaving the ordinary no-Parent/local-only QuickPick behavior untouched.

## Requested Interaction

When an Outgoing context has a Parent carrier, source selection starts from the Parent-carried Incoming baseline and exposes one `Source preset` QuickPick button. Each press cycles deterministically through:

1. `Incoming only` — select every Workspace carried by the Parent; all Local alternatives are unselected.
2. `None` — select no Workspace sources so the operator can build a custom selection manually.
3. `Prefer Local` — select Local wherever a Local Workspace exists, plus Parent Incoming only for Workspace identities missing locally.
4. `Prefer Incoming` — select Parent Incoming wherever carried, plus Local only for Workspace identities absent from the Parent.
5. `Local only` — select every qualified Local Workspace and no Parent Incoming source.
6. The next press returns to `Incoming only`.

At all times a Workspace identity remains exclusive: Local and Incoming cannot remain selected simultaneously for the same identity.

## No-Parent Boundary

If there is no Parent carrier, no source-preset button is activated. The picker remains the ordinary Local Workspace multi-select surface and VS Code's built-in checkbox/select-all behavior remains unchanged.

## Candidate Change

- Reuse the pure Outgoing source-preset projection already present in `src/core/sourceSelection.ts`.
- Wire that projection into the Outgoing QuickPick only when a Parent carrier is present.
- Show the current preset and next preset in the button tooltip.
- If the operator manually edits the selection into a custom state, the button reports `Custom` and the next press returns to `Incoming only` before continuing through the five-mode cycle.
- Keep individual checkbox selection and the existing exclusive-source resolver intact.
- Remove the old Outgoing-only byte-identical normalization on picker initialization; Guided Entry embedded-wins deduplication remains a separate Core behavior and is not changed by this Task.

## Acceptance Evidence

Anchor verified the five source projections directly with overlapping Local/Parent sources plus Local-only and Incoming-only identities:

- `Incoming only` -> Parent Incoming `core`, `docs`, `remote`.
- `None` -> empty selection.
- `Prefer Local` -> Local `core`, Local `docs`, Local-only identity, Incoming-only `remote`.
- `Prefer Incoming` -> Incoming `core`, Incoming `docs`, Incoming `remote`, Local-only identity.
- `Local only` -> Local `core`, Local `docs`, Local-only identity.

Each projection round-trips through preset detection to the same mode. The QuickPick wiring is Parent-gated, preserves `canSelectMany`, and cycles the declared mode order.

## Scope

- VS Code Outgoing Parent source-selection presentation/interaction only.
- Pure deterministic preset projection and QuickPick wiring only.
- Durable Task/Handoff continuity for Sigma acceptance.

## Dependencies

- [Finish Outgoing Select-All And Retire Redundant Git Operator UI](011-finish-outgoing-select-all-and-retire-redundant-git-operator-ui-task.trace.md)
- Current carried VS Code Workspace.
- Current Parent carrier source set.

## Done Criteria

- Parent-backed Outgoing selection exposes the five-mode preset cycle in the declared order.
- The initial Parent-backed baseline remains `Incoming only` when there is no prior explicit Outgoing selection.
- `Prefer Local` and `Prefer Incoming` preserve complete Workspace coverage by filling only the missing side.
- `Local only` and `Incoming only` remain strict source-only modes.
- `None` permits fully manual selection.
- No Workspace identity can remain double-selected.
- No-Parent/local-only Outgoing selection retains the ordinary VS Code multi-select/select-all behavior.
- Replace, Initialize, Guided Entry, Git staging, carrier lineage, Major allocation, package topology, and Core semantics do not change.

## Boundaries

- No remote mutation is authorized by this Task.
- Do not begin the broader Core↔host boundary/test-baseline audit remediation in this pre-Major Task.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 63xpMO-7hYGc33UTApxctUENo9f6liR5nkRvA2-lQ1o