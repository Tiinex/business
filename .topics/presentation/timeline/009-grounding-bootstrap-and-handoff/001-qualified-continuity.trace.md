# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:48
  - Trace: [001-1-1-playthings-separates-the-experiment.trace.md](../008-the-playthings-experiment/001-1-1-playthings-separates-the-experiment.trace.md)
  - Origin:
    - [relative](../008-the-playthings-experiment/001-1-1-playthings-separates-the-experiment.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:48
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: Maturing explicit transfer and qualification with fixed source anchors.
  - Status: approved-for-publication

---

# A carrier is useful only if a recipient can orient and continue

The practical pieces eventually converged on a more explicit arrangement: portable artifacts with typed relations, Workspaces as bounded contexts, Handoff as transfer semantics, a Package as carrier/discovery boundary, and bootstrap tooling to inspect what has actually been supplied. This is a **convergence chapter**: some components existed in May or June, while the maintained Handoff and Package contracts emerged later.

## Source artifacts that show the maturation

- [August 22 Handoff schema](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md) — defines responsibility/work transfer separately from packaging.
- [September 1 Handoff Package schema](https://github.com/Tiinex/docs/blob/25cb94d68a46d8670d437869e67c4555e74b2f26/.topics/.schemas/coordination/handoff/package/tiinex.handoff.package.v1.schema.md) — defines a receiver-facing carrier; does not duplicate the Handoff itself.
- [September 18 cold-consumer bootstrap recovery code](https://github.com/Tiinex/core/blob/7a4c0e1eab27559eef417cf5eb1c15d47483d199/src/tooling/portable/handoff/bootstrapRecovery.js) — a bounded implementation milestone.

## Recipient walkthrough

A recipient gets material with a declared entry. They must inspect the actual qualified source, identify what the carrier contains, distinguish current tasks from historical artifacts, find any selected Handoff route and its participants, and report whether they can safely act. Merely extracting ZIP bytes does not confer authority or truth.

## The outcome to examine

Can another supported host or model recover enough to continue a bounded task **without the originating conversation**? And can it say what it could not recover? That is the testable value proposition; every successful test is specific to its setup and constraints.

The next three entries deepen this chapter: transport vs grounding, testing limits, and ordinary continuation.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-playthings-separates-the-experiment.trace.md](../008-the-playthings-experiment/001-1-1-playthings-separates-the-experiment.trace.md)
  - Value: nFvY3z-c2nOtU3wQxnAQ4FRgKb7LKuaWa_3ZJ5e1evI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Qu3WL9dYGn060RzwtCrTmO5IEib7icuv6yXt83-jbp0
