# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Trace: [001-processes.trace.md](../../001-processes.trace.md)
  - Origin:
    - [relative](../../001-processes.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-09 15:06:50
  - Authors: Anchor
  - Why: Turn-2 recovery exposed a recurring runtime failure mode that should not depend on Sigma's conversational memory.
  - Summary: Fail-closed successor procedure when execution runtime integrity becomes untrustworthy.
  - Status: ready/local

---

# Emergency Runtime Handoff

## Purpose

Preserve current work and transfer responsibility when the execution runtime is no longer trustworthy enough for safe mutation or qualification.

## Trigger Discipline

Distinguish product/test failure, tool-specific failure and runtime-integrity failure. A single ordinary test failure or transient tool error is not sufficient. Repeated unrelated failures on trivial operations across execution tools are strong evidence that runtime integrity is no longer trustworthy.

## Procedure

- Stop new implementation and destructive work.
- Do not manufacture claims that cannot be verified.
- Identify the latest durable source/checkpoint/Handoff and surface already-created recovery material when needed.
- Record what was last verified, what was only reported, what may exist only in failed runtime state, and what was not changed.
- If qualified Tooling still functions, manufacture the normal successor Handoff.
- If Tooling itself cannot execute reliably, do not label an ordinary ZIP as a qualified Handoff; provide explicit recovery transport instead.
- The successor re-grounds source and verifies carried bytes before substantial mutation, then creates the first current durable checkpoint/Handoff.
- Runtime failure alone does not change semantic Parent, path allocation, carrier major or package version.

## Grounding Gap Review

After successor grounding, route any exposed durable gap to the narrowest owning Role, Process, semantic authority or Tooling surface rather than adding duplicate prose everywhere.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-processes.trace.md](../../001-processes.trace.md)
  - Value: -dIbKFmhRYlDVjL-4TkCoeb6KCK-5wH6l4U8zsPgj8s

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: O6p3oZrZkk4AYDrxWMxwmjgfegZ_O9VYGQbY7oAeO7I