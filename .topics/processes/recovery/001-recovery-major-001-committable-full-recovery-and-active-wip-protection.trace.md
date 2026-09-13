# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-13 15:02:02
  - Trace: [014-1-1-1-anchor-full-recovery-grounding-transport-closed-fresh-succession.trace.md](../../initiatives/refactor/orchestration/handoffs/014-1-1-1-anchor-full-recovery-grounding-transport-closed-fresh-succession.trace.md)
  - Origin:
    - [relative](../../initiatives/refactor/orchestration/handoffs/014-1-1-1-anchor-full-recovery-grounding-transport-closed-fresh-succession.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-13 16:11:30
  - Authors: Anchor
  - Why: The latest Full Recovery was qualified yet landing it over the active VS Code checkout staged destructive rollback/deletion scope; Anchor must guarantee stable committable Recovery before Sigma receives it.
  - Summary: Make Full Recovery stable and committable without silently deleting or reverting newer local WIP.
  - Status: ready/local

---

# Recovery Major 001 — Committable Full Recovery And Active-WIP Protection

## Objective
Make Full Recovery a trustworthy restart/checkpoint surface that can be handed to Sigma as stable and committable without silently deleting or reverting newer local work, while preserving the distinction between accepted Recovery state and unaccepted local WIP.

## Reproduced Evidence
- The prior accepted Full Recovery and the later fresh-successor Full Recovery carry byte-identical `extension-vscode` Workspace snapshots: 262 files, 0 additions/removals/changes between those two Recovery carriers.
- The latest qualified VS Code candidate carries 290 files relative to that Recovery snapshot: 28 current-only files and 36 changed files.
- Landing the Full Recovery onto the active Windows checkout therefore staged a large rollback surface, including `.topics` deletions, instead of failing closed or requiring an explicit reconciliation decision.
- This means the observed deletion surface is not proven to be Reduction physically pruning the Recovery snapshot; the stronger reproduced failure is that a stable accepted Recovery can be applied destructively over a checkout containing newer WIP without an adequate divergence/preflight guard.

## Scope
- Audit the host-neutral Recovery/landing/reconcile path that permits accepted Recovery snapshots to overwrite, delete, or revert current-only/divergent target checkout state.
- Define and implement a fail-closed preflight for Full Recovery landing when the target contains current-only or divergent work that is not proven safe to replace.
- Preserve accepted Recovery snapshot semantics: do not silently absorb unaccepted WIP into Master Recovery merely to avoid deletions.
- Reuse existing compare/reconcile semantics where possible; do not invent parallel merge semantics.
- Make the safe operator outcomes explicit: exact-safe landing, explicit reconciliation, or stop with a precise blocker.
- Add a Recovery acceptance audit that materializes the manufactured carrier and verifies intended Workspace bytes, unexplained removal count, and committable/restart suitability before Anchor labels it `Master Recovery` for Sigma.
- Preserve historical provenance; Reduction/current-attention projection must never imply physical source pruning unless explicitly authorized by its owning semantics.

## Dependencies
- Current accepted Full Recovery lineage and exact carried Workspace snapshots.
- Existing compare/reconcile semantics and landing/preflight behavior in shared Tooling.
- Reproduced Windows evidence that applying the accepted Recovery over a newer active checkout staged rollback/deletion scope.
- Latest qualified VS Code candidate used only as comparative evidence; its unaccepted WIP must not be promoted into Recovery.

## Acceptance Evidence
- Reproduce the active-WIP conflict with a fixture or exact equivalent: Recovery snapshot A plus target checkout B where B contains current-only and modified files.
- Default Recovery landing does not silently delete/revert B-only/divergent work.
- Exact-safe targets remain green and do not gain unnecessary prompts or blockers.
- A divergent target gets a deterministic fail-closed/reconcile-required result that identifies current-only/changed scope before mutation.
- No implementation auto-promotes unaccepted WIP into accepted Recovery.
- Full Recovery manufacture/acceptance has an Anchor-consumable coarse audit proving the carried Workspace set can be re-materialized without unexplained deletions relative to its declared accepted basis.
- Broad relevant Core/Tooling validation passes on exact candidate bytes.

## Exclusions
- Do not repair VS Code feature code or artifact hygiene debt in this Major.
- Do not mass-rewrite `.topics` history.
- Do not redefine canonical schema semantics; route any required semantic/schema change to Axiom.
- Do not weaken exact-byte reconciliation or fail-closed authority boundaries.

## Done Criteria
- One qualified Loom → Anchor return carrying the bounded Tooling/recovery implementation and evidence.
- Direct return uses the explicitly reserved non-Major package sibling index 1.
- Anchor can use the returned mechanics to manufacture a new Full Recovery and audit it as stable + committable before exposing it to Sigma.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [014-1-1-1-anchor-full-recovery-grounding-transport-closed-fresh-succession.trace.md](../../initiatives/refactor/orchestration/handoffs/014-1-1-1-anchor-full-recovery-grounding-transport-closed-fresh-succession.trace.md)
  - Value: SckhswSreuTsSYO_k_01olLfJsKhqC5VgnXK-lFHa_M

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: -_YX-EmvHd9U_9qEosRUJkRhZVOx-w4-r-LdCiBhudQ