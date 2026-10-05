# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-03 19:28:10
  - Trace: [001-1-1-classify-owner-placement-and-applicable-process.trace.md](001-1-1-classify-owner-placement-and-applicable-process.trace.md)
  - Origin:
    - [relative](001-1-1-classify-owner-placement-and-applicable-process.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-03 19:28:11
  - Authors: Anchor; Sigma
  - Why: Provide one deterministic stage in the reusable Tiinex Work Lifecycle.
  - Summary: Create the smallest authoritative current work artifact in its natural Workspace.
  - Status: ready/local

---

# Create Bounded Work

## Objective

Create the smallest authoritative work artifact that can own the current frontier.

## Rules

- Author in the natural owning Workspace and qualified Scaffold placement.
- Use the artifact schema appropriate to the work kind. Project owns a real coordinated outcome; Task owns bounded executable work; Task children are the default subtask mechanism when no independent Project boundary exists.
- Declare real Parent continuity and typed relations where the schema supports them; directory placement and filename shape must not manufacture lineage.
- For Tiinex-specific development work that crosses a repository boundary, require the intended upstream Business Project Parent to be qualified and immutable/published before the child is authored. Supply exact Parent bytes plus commit-pinned recovery when materializing the child.
- If the required cross-repository Parent is new and not yet published, author/checkpoint the upstream spawn boundary and STOP. The truthful interrupted state is `spawn intended; child not materialized`, not a parentless child awaiting later cleanup.
- A Workspace-qualified selector such as `business::path` is runtime resolution input only and must not be serialized as durable replacement for immutable external Parent recovery.
- Related Project/Task relations may support coordination but do not replace Parent where direct continuation is intended.
- Record acceptance criteria or desired outcome at the authority boundary that can actually judge them.

## Exit Condition

One bounded current artifact owns the work and can be grounded independently of chat history.

## Next Artifact

- [Execute Through Applicable Process](001-1-1-1-1-execute-through-applicable-process.trace.md)

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-classify-owner-placement-and-applicable-process.trace.md](001-1-1-classify-owner-placement-and-applicable-process.trace.md)
  - Value: zpFuquFCTQkDi_HRC3e7YY8b8YXSexSkUtroQSMZQBQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: pU54KnXhcRwGe7ZBMVf8QNZKTlkl2JWulRqWtnNCpVc