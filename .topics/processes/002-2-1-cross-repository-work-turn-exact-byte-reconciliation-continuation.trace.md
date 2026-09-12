# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-12 00:03:46
  - Trace: [002-2-cross-repository-work-turn-reconciliation-major-human-gate-continuation.trace.md](002-2-cross-repository-work-turn-reconciliation-major-human-gate-continuation.trace.md)
  - Origin:
    - [relative](002-2-cross-repository-work-turn-reconciliation-major-human-gate-continuation.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-12 09:04:53
  - Authors: Anchor
  - Why: Docs Major 005 integration demonstrated that deterministic ZIP timestamps and equal-size changed artifacts can defeat mtime/size copy heuristics; Core reconciliation correctly caught the stale candidate before recovery manufacture.
  - Summary: Require exact-byte base/incoming/current/reconciled proof and forbid timestamp/size copy heuristics from standing in for source identity during specialist-return integration.
  - Status: ready/local

---

# Cross-Repository Work Turn — Exact-Byte Reconciliation Continuation

## Current Read

Return integration must be decided from exact qualified source identity, not filesystem freshness heuristics. Deterministic carriers deliberately normalize timestamps, and changed artifacts may retain the same byte length. A merge helper that trusts `mtime`, archive timestamp, or size can therefore silently preserve stale bytes even when a specialist return is otherwise conflict-free.

## Exact-Byte Reconciliation Rule

For every concurrent specialist return:

- establish the exact delegated **base**, returned **incoming**, and accepted **current** source frontiers;
- build the candidate **reconciled** frontier from explicit selected bytes, not timestamp/size-based copy heuristics;
- prove the candidate with shared Core source-frontier reconciliation before recovery manufacture when that gate is available;
- require every automatically accepted incoming-only and current-only path to survive with exact bytes;
- require explicit disposition for conflict/deletion candidates;
- fail closed when the reconciled frontier fingerprint does not match the mechanically expected result;
- treat normalized ZIP timestamps, equal byte sizes, directory mtimes, copy-tool skip decisions, and extraction order as non-authoritative implementation details.

A content copy may be implemented by exact archive-byte materialization, digest-aware copy, explicit changed-path copy, or another qualified mechanism. The process requirement is exact source identity, not one particular filesystem command.

## Demonstrated Failure Mode

During Docs Major 005 integration, the Root schema and dependent Transport Envelope integrity bytes changed while deterministic archive timestamps remained normalized. A timestamp/size-oriented overlay preserved stale Transport Envelope integrity bytes even though the intended incoming frontier was conflict-free. Core reconciliation rejected the candidate as `reconciled-frontier-mismatch`, exposing the stale byte before recovery manufacture.

The correction was to rebuild the candidate from exact incoming bytes and rerun reconciliation. The corrected Docs proof became `manufacture-ready` with four incoming-only paths, zero conflicts, and zero mismatches. Core Major 007 similarly reconciled with fifteen incoming-only paths and zero conflicts/mismatches.

This incident is a process/tooling-success signal: the reconciliation gate, not the copy command, owns mechanical preservation confidence.

## Recovery Discipline

- Never infer that a complete incoming Workspace can replace the accepted current Workspace without reconciliation.
- Never infer that a copy command actually transferred changed bytes merely because it returned success.
- Recovery manufacture should consume or independently re-prove exact source identity after reconciliation.
- Same exact Carrier Dimension with divergent package bytes remains a hard failure.
- Historical source is not rewritten merely to normalize representation.

## Defect-To-Improvement Rule

If a merge/recovery incident exposes a reusable blind spot, update the narrow durable owner rather than retaining a personal Anchor workaround. This continuation is the Business process correction for the demonstrated mtime/size merge hazard; Core owns the mechanical reconciliation gate itself.

## Interpretation Limits

This process does not grant Tooling semantic merge authority, authorize deletion, replace repository-owner review, or make filesystem paths/timestamps semantic truth. It defines the minimum mechanical evidence required before Anchor may rely on a concurrent source union.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [002-2-cross-repository-work-turn-reconciliation-major-human-gate-continuation.trace.md](002-2-cross-repository-work-turn-reconciliation-major-human-gate-continuation.trace.md)
  - Value: Iki4WHrUDupW1YcqT34MyBzwAzSQeIBYGJSxynO4t9Y

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: wmzNCH-EPTKqmhdLEbGm0fop5d8dftmZYPGAu66b34g