# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-10-05 19:21:14
  - Trace: [001-2-entry-what-where-and-workspace-work-area-structure.trace.md](001-2-entry-what-where-and-workspace-work-area-structure.trace.md)
  - Origin:
    - [relative](001-2-entry-what-where-and-workspace-work-area-structure.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-10-05 20:16:26
  - Authors: Anchor; Sigma
  - Why: Align new grounding/process work with the stronger typed Process pattern already present in Business instead of representing executable steps as generic Topics.
  - Summary: Use Topic roots, Transition Definition executable positions, and Relation topology edges as the default reusable Process representation.
  - Status: ready/local

---

## Decision

- State: accepted
- Subject: Typed reusable Process topology for process roots, executable positions, and branch/composition edges
- Decision: Tiinex reusable Process material uses a Topic artifact for the process identity/root unless and until a dedicated Process root schema is separately justified. Durable executable process positions use `tiinex.transition.definition.v1`. Durable branch, outcome, loop, composition, or sub-process topology edges use `tiinex.relation.v1` when the relation is semantically material. Child Topics are not the default representation for executable steps merely because they are stored under a process directory.

## Basis

- Existing Business processes such as Development And Acceptance and Accepted Change Landing already use this typed pattern successfully: Topic root, Transition Definition positions, and Relation branch/composition edges.
- `tiinex.transition.definition.v1` explicitly owns reusable bounded transformation semantics, applicability, input/output roles, lifecycle effects, continuity effects, placement intent, and interpretation limits; those are stronger semantics than a generic Topic provides for an executable process position.
- `tiinex.relation.v1` explicitly separates process topology edges from Tiinex continuity Parent, which prevents branch/composition meaning from being smuggled through filename or directory structure.
- A generic Topic remains appropriate for the reusable process identity/root while the current process model does not require a dedicated `tiinex.process.v1` contract.
- Human-readable process directories and filename lineage remain navigation/discovery aids; artifact schema and explicit relations remain semantic truth.

## Consequences

- Native Session Grounding And Continuity will receive a typed successor topology whose process identity remains Topic-based and whose durable steps are Transition Definitions.
- OpenAI ChatGPT continuity/source-discipline will receive the same typed successor topology in `interop-openai`; OpenAI-specific semantics remain owned there.
- Existing Topic-based step artifacts created during the preceding P1 checkpoint remain historical candidate material and are not rewritten in place. The corrected typed topology is represented through successor artifacts.
- Process Scaffold guidance must explicitly recommend Transition Definitions for executable positions and Relations for durable topology edges, while allowing one-artifact atomic processes and explanatory/supporting Topics when those semantics are truthful.
- A dedicated `tiinex.process.v1` is not created merely to improve naming aesthetics. It should be proposed only if the Topic root cannot express required reusable process identity/applicability/composition semantics without duplicated or hidden authority.
- No existing Business/Native/OpenAI process tree is broadly migrated by this Decision. Broader convergence remains separate migration work.

## Review Conditions

- Review if Process roots require machine-authoritative semantics not owned cleanly by Topic plus Transition/Relation.
- Review if Transition Definition becomes too execution-oriented for a durable process position or if another qualified schema supersedes it.
- Review if real process dogfood shows that explicit Relation artifacts are either insufficient or unnecessarily materialized for common branch/composition cases.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-entry-what-where-and-workspace-work-area-structure.trace.md](001-2-entry-what-where-and-workspace-work-area-structure.trace.md)
  - Value: rvEKaBdQ8YjpfmiD6bOibLvBOVXTYIOzJ4PtR5lB67w

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: llDJHT3sx41lT3DqgHRsk4zrUH3ccE_C4CfENzo9ePo