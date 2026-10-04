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
  - Created At: 2026-10-04 20:59:12
  - Authors: Anchor; Sigma
  - Why: Eliminate Core/VS Code carrier-dimension mismatch when a newer same-prefix Major already exists locally.
  - Summary: Make explicit Handoff Package Major allocation advance from the highest observed same-prefix Major while preserving the selected Parent carrier dimension.
  - Status: ready/local

---

# Align Handoff Package Carrier Major Allocation With Observed Same-Prefix Frontier

## Objective

Correct Core's Handoff Package carrier Major allocation so an explicit Major request advances from the highest already allocated Major observed for the same carrier prefix, rather than deriving the next Major only from the selected Parent carrier dimension.

The user-visible contract is outer-carrier naming/allocation only. If `tiinex-020...` already exists locally for prefix `tiinex`, the next explicit Major is `tiinex-021...` even when the selected Parent carrier belongs to an older Major lineage.

## Observed Regression

VS Code correctly projected `021` because a local `020` carrier already existed. Core manufacture returned `019` from the selected Parent lineage, causing a shared carrier-dimension contract mismatch.

The regression was isolated to Core's Package V1 manufacture CLI path used for a Workspace-selected Handoff Package carrier with both:

- an explicit qualified Package Parent; and
- an explicit Major request.

The equivalent Handoff-route manufacture path already used the highest observed same-prefix Major frontier.

## Candidate Change

For the affected Core manufacture branch:

- qualify the selected Parent carrier as before;
- preserve the Parent carrier dimension as `parentDimension`;
- use Core's existing same-prefix Major allocation projection over the supplied observed carrier filenames;
- allocate `highest observed same-prefix Major + 1`;
- retain fail-closed prefix conflict and allocation ambiguity behavior;
- preserve existing provenance describing the observed frontier and Parent carrier.

## Acceptance Evidence

A real Core CLI manufacture was executed with:

- carrier prefix: `tiinex`;
- selected Parent dimension: `018-1-1-1-1-1-1-1`;
- observed local carrier names including Major `019` and `020` for prefix `tiinex`;
- explicit Major request.

Core produced `tiinex-021.handoff-package.zip` with:

- status: ready;
- carrier dimension: `021`;
- Parent dimension preserved as `018-1-1-1-1-1-1-1`;
- Package inspection: valid;
- physical roundtrip: passed;
- zero findings.

## Scope

- Core outer Handoff Package carrier Major allocation for the affected explicit-Major + Parent manufacture path.
- Preserve parity with the already-correct same-prefix Major allocation rule used elsewhere in Core.
- Transfer the candidate to Sigma for the smallest real VS Code confirmation that a locally existing `020` causes the next Major to manufacture as `021` without carrier-dimension mismatch.

## Dependencies

- Existing Core carrier Major allocation projection and filename parsing.
- The previously accepted VS Code workflow repair candidate and its Package V1 parent carrier.
- Existing Tiinex grounding/recipient-transfer discipline for Anchor -> Sigma acceptance.

## Done Criteria

- Core allocates the next explicit Major from the highest observed Major for the same prefix plus one.
- A selected older Parent carrier remains the semantic carrier Parent and its dimension remains recorded as `parentDimension`; it does not cap or reset the observed Major frontier.
- Other prefixes do not affect allocation.
- Core CLI manufactures `021` when Parent is older and `020` is already observed for prefix `tiinex`.
- Package inspection and physical roundtrip remain valid with zero findings.
- Sigma can confirm the real VS Code Major workflow without debugging implementation.

## Boundaries

- This Task does not change Tiinex artifact lineage, artifact filenames, artifact Parent ancestry, or artifact semantic ownership.
- This Task does not change Handoff Package V1 internal archive topology, Workspace materialization topology, Handoff route topology, or carrier Parent semantics.
- This Task does not change Workspace identity/discovery, Replace, Initialize Workspace, Local/Latest switching, or linked-extension build behavior.
- Carrier filename/dimension allocation is transport lineage only and must not be interpreted as semantic artifact Parent authority.
- No commit, push, publication, release, or other remote mutation is authorized by this Task.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Ogz1NQNwFRfcd7AwaQQ9hJIXkbYC5qGD8fqvEyzsqnE