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
  - Created At: 2026-10-05 13:22:47
  - Authors: Anchor; Sigma
  - Why: Avoid state loss while the current A/B/C closure batch is partially verified and before broader verification or Sigma acceptance.
  - Summary: Preserve the exact in-progress content-source, Native authority, and deterministic-lineage closure state for successor Anchor recovery.
  - Status: ready/local

---

# Recover Post-023 Authority And Lineage Closure Batch

## Objective

Preserve the exact in-progress post-023 closure state so a successor Anchor can resume without reconstructing the work from conversation history.

This recovery checkpoint captures three already-started tracks:

- content-source selection boundary;
- Docs/Native schema authority and local-first verification;
- deterministic lineage maintenance projection/apply plus real Business dogfood.

## Recovered State

### A. Content-source selection boundary

Core now distinguishes carriage from activation:

- a carried Workspace is not automatically an active reusable content source;
- automatic content-source selection requires package declaration through `tiinex.contentSource`;
- explicit content-source selection remains allowed without that declaration;
- installed discovery traverses dependency graphs but only activates declared reusable content packages.

Focused verification already passed:

- content/catalog bootstrap group: 10/10;
- focused content-selection subset: 5/5.

### B. Docs / Native authority closure

A qualified successor Decision now states:

- Docs remains canonical semantic/schema contract authority;
- Native `.topics/.schemas` is the maintained first-party distribution snapshot plus co-located schema-specific companions;
- Core owns generic schema/runtime/sync mechanics;
- carried Workspace membership does not imply active content-source selection;
- local unpublished sync checks preserve existing qualified immutable publication provenance when bytes remain exact.

Native verification already passed:

- Native local-first package tests: 5/5;
- focused schema-sync tests: 4/4;
- schema snapshot check: 109 schema contracts, no stale canonical copies after sync repair.

### C. Deterministic lineage maintenance

Core now contains executable projection/apply work for the previously paused lineage project, including:

- Move;
- Prepend / ordered insertion chain;
- Directory namespace qualification and Normalize Directory;
- fail-closed unsupported arbitrary reorder;
- exact projected-plan fingerprint verification;
- input-drift and target-collision blocking;
- public Node apply export and CLI operation wiring.

Focused projection/apply verification passed 12/12.

A real dogfood application was executed against Business process directories. The resulting Business tree is intentionally carried by this recovery package so the exact applied state is not lost.

## Observed Non-Blocking Debt

A post-dogfood Business audit reports one error on:

`.topics/roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md`

with code `party.role.assignmentModes.invalid`.

That Role artifact is byte-identical to the 023 baseline, so the finding is pre-existing validation debt and is not evidence that the lineage dogfood corrupted Business state. Do not rewrite that historical Role merely to make the dogfood audit green without first qualifying the correct repair boundary.

## Scope

- Preserve the current Business/Core/Native bytes exactly except transient runtime/install state.
- Continue qualification of the three tracks above from this checkpoint.
- Resolve whether the Business dogfood result itself is acceptable before further lineage mutation.
- Run broader verification only after the current state is safely recoverable.

## Dependencies

- Major 023 stable carrier baseline.
- [Deterministic Lineage Maintenance](../initiatives/004-deterministic-lineage-maintenance-project.trace.md)
- [Grounding And Continuity Readiness](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- Native schema authority/extraction project and successor authority Decision carried in the Native Workspace.

## Done Criteria

- Recovery package contains the exact current Business/Core/Native state and inherits all unchanged Workspaces from 023.
- A successor Anchor can re-ground from the package and recover A/B/C without conversation archaeology.
- No transient `node_modules` or `.tiinex` runtime cache is treated as durable project state.
- Remaining work after recovery is explicit rather than inferred.

## Boundaries

- This Task is a recovery checkpoint, not Sigma acceptance.
- Do not perform remote mutation.
- Do not reopen stabilized VS Code workflow unless a concrete compatibility regression is observed.
- Do not treat the pre-existing Sigma Role validation finding as lineage-dogfood corruption.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 7g55_HJ1fGhCLlR-o11oSeyefoUdu4dmxF90oujTy68