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
  - Created At: 2026-10-05 09:37:04
  - Authors: Anchor; Sigma
  - Why: Prevent platform-limit state loss while continuing the consolidation work already started after the 022 audit.
  - Summary: Preserve the post-022 closure batch: Core verification is green, VS Code verification migration is in progress, and contract/semantic cleanup remains the next frontier.
  - Status: ready/local

---

# Restore Truthful Verification And Close Started Architecture Cleanup

## Objective

Preserve and continue the in-progress post-022 closure batch after platform conversation-limit interruption. The batch is intentionally consolidation-first: restore truthful verification, formalize the already-stabilized Core↔host contract, then remove started semantic duplication without reopening stable operator workflows.

## Starting Point

Major 022 is the product baseline. A parallel low-pre-context audit concluded that the active Core↔VS Code regression boundary is substantially healthier, while the remaining red risk has moved to verification debt, broad host-adapter surface, and duplicated artifact semantics in VS Code.

This Task therefore does not reopen the repaired Replace, Initialize, Guided Entry, Handoff Package, carrier allocation, Stage All, Outgoing, or linked-build workflows unless a contract/behavior regression test proves a real defect.

## Completed In This Batch

### Core verification baseline

The previously known-red Core test population was traced primarily to stale test-harness assumptions from the content/schema authority migration rather than to 94 independent product defects.

The Core test harness and affected tests were migrated to the same explicit external content composition that the 022 product path uses:

- Core remains generic mechanics;
- Native is selected as external first-party content authority for test runtime composition;
- tests consume current schema/material bindings instead of old Core-local schema pack paths/permalinks;
- stale generated-transition/native-schema-pack assumptions were removed rather than recreating old product architecture inside tests.

Observed full Core result after migration:

- 422 tests;
- 421 pass;
- 0 fail;
- 1 skip.

This is the new truthful Core baseline and must be preserved.

## In-Progress Work At Recovery

### VS Code verification migration

The carried 022 VS Code harness still contains source-shape assertions that can fail on behavior-preserving refactors. The batch has started migrating those checks toward behavior/contract evidence.

Current modified VS Code surface relative to 022:

- `.vscode/tasks.json`;
- generated `dist/` used by the carried harness;
- `src/core/artifactNavigation.ts`;
- `src/operatorTrees.ts`;
- `test/run.mjs`.

Progress so far:

- the stale Handoff Markdown Preview assertion that required literal `handoff` text inside `openArtifactNode()` was identified as source-shape debt and moved toward helper/behavior-oriented verification;
- subsequent harness runs progressed substantially farther;
- the latest run still stops on a stale assertion around the retired/reduced Git command surface at `test/run.mjs` near the Stage All / Reset Dirty policy checks.

The VS Code verification migration is NOT complete and must be continued before architecture cleanup proceeds.

## Next Frontier

1. Finish VS Code harness migration until the carried harness is green for the 022 product behavior. Prefer executable behavior/contract checks over regex assertions about function bodies.
2. Freeze a Core↔host contract matrix for the already-working manufacture variants: pointerless/routed, Parent/no Parent, Major/no Major, explicit selected Core, Guided Entry, Workspace source exclusivity, and filesystem observation facts.
3. Introduce the smallest host-facing facade needed to express observations, operator selections, environment capabilities, Core decisions/projections/reason codes/receipts without copying portable internal details into each future host.
4. Remove dead or duplicated VS Code artifact semantics only where Core already owns the truth, beginning with legacy `artifactTree.ts` parsing/current-role logic that has no active caller.
5. Only after verification and boundary cleanup are stable, consider decomposing `operatorTrees.ts` or consolidating semantically sensitive Core primitives. Do not DRY for its own sake.

## Acceptance Evidence

- The Core suite was run after migration and observed green at 422 total / 421 pass / 0 fail / 1 skip.
- The prior 022 audit independently observed the same 94 Core failures in 021 and 022 before this batch, supporting the diagnosis of persistent harness debt rather than a new 022 regression population.
- VS Code harness iterations demonstrate that stale source-shape checks are the current blocker; later iterations advance past earlier assertions without evidence of operator workflow regression.

## Scope

- Core test-harness/content-composition migration required for a truthful green baseline.
- VS Code test-harness migration from source-shape assertions toward behavior/contract verification.
- Core↔host contract matrix/facade consolidation already motivated by the stabilized 022 boundary.
- Removal of demonstrably dead/duplicated host semantics where Core already owns the meaning.
- Durable recovery of this exact work state.

## Dependencies

- [Grounding And Continuity Readiness](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- Stable Major 022 product baseline carried as the package Parent.
- Current Core/Native content ownership model and current VS Code host adapter.

## Done Criteria

- Core remains at a truthful green baseline; no test-only reintroduction of old Core-owned schema/content architecture.
- VS Code carried harness is green or every remaining red has an explicitly qualified real product defect rather than source-shape debt.
- The working Core↔host variants are represented in a contract matrix with shared invariant coverage.
- VS Code no longer independently owns artifact semantics already available as Core projection where the old code is dead or safely replaceable.
- Stable operator workflows remain behaviorally unchanged unless a new real defect is proven.
- A subsequent fresh/cold grounding replay can consume the resulting Major without relying on this chat history.

## Boundaries

- Do not reopen five-mode Outgoing UX; Sigma explicitly accepted the simpler Local/Incoming toggle behavior as sufficient.
- Do not broadly rewrite Core or VS Code.
- Do not split `operatorTrees.ts` before the verification/contract boundary is stable.
- Do not consolidate generic-looking Core duplicates unless the primitive is semantically sensitive and ownership is clear.
- No commit, push, publication, release, deployment, or other remote mutation is authorized by this Task.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: dCw5svlotlyXPQ2ugjyioeAoGlbcltabE6GL4ExQwPg