# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/8f568f14658a48500e2fa4d0d72a58620eaae759/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-31 01:28:53
  - Trace: [002-cross-repository-work-turn-process.trace.md](002-cross-repository-work-turn-process.trace.md)
  - Origin:
    - [relative](002-cross-repository-work-turn-process.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-12 00:03:46
  - Authors: Anchor
  - Why: Recent specialist-return and Sigma-test failures exposed durable process gaps that belong in Business process authority rather than Anchor memory.
  - Summary: Continue the cross-repository process with base/incoming/current reconciliation, fixed-Major discipline, local-first recovery, human-gate carriage and defect-to-owner evolution.
  - Status: ready/local

---

# Cross-Repository Work Turn — Reconciliation, Major, Recovery And Human-Gate Continuation

## Current Read

Cross-repository work remains bounded by explicit Tasks/Handoffs and repository ownership. This continuation adds the integration, recovery, Major-scope, and human-gate rules demonstrated by later multi-role work without changing artifact Parent semantics.

## Return Reconciliation Rule

A specialist return is a candidate relative to the exact source frontier it received. Before integration when the accepted frontier may have advanced, compare **base / incoming / current** or preserve equivalent qualified evidence.

- incoming-only source may be accepted when it belongs to the delegated return;
- current-only source must not disappear merely because the incoming Workspace snapshot is complete;
- same-result concurrent change is not a conflict;
- conflicting overlap requires explicit owner/Anchor disposition;
- intentional deletion must be explicit and may not be inferred from absence in a child snapshot;
- complete incoming Workspace replacement is not a substitute for reconciliation.

Automatic byte union may help detect candidates; it is not semantic merge authority.

## Major Discipline

- A Major is a bounded operational scope/checkpoint declared by controlling work authority.
- Adjacent useful work does not silently join an active Major.
- New work is excluded, separately delegated, or explicitly re-scoped.
- Carrier Major numbers and artifact filename lineage remain separate projections.
- Completion means the declared scope is coherently closed or explicitly returned with a bounded blocker; turn count, lineage length or carrier movement alone is not completion.

## Recovery Discipline

- Anchor maintains an exact qualified recoverable integration frontier while child lanes are active.
- Prefer qualified local/carried source before remote reconstruction; fallback must be explicit and auditable.
- Every accepted return updates recovery through reconciliation, not wholesale Workspace replacement.
- Same exact Carrier Dimension with divergent package bytes is a hard process/tooling failure signal.

## Human Gate Rule

When Sigma or another declared human must test/accept a dependency-sensitive result:

- deliver sufficient complete selected source/context in one qualified carrier;
- give one clear front-door action and expected result;
- identify what not to debug or mutate;
- do not require the human to reconstruct dependencies, follow broken lineage just to discover the test procedure, or guess among multiple plausible launch paths;
- machine PASS remains separate from human acceptance.

## Defect-To-Improvement Loop

Every repeated workaround, successor teaching burden, process mismatch, Tooling blind spot, authority confusion, repository-boundary drift or human-test friction should be classified to the narrowest durable owner: Semantics/Docs, Anchor Role, Business Process, Grounding/Required Context, Tooling/Core, repository-local implementation, human-gate design, or transient recovery.

Fix and qualify the owning layer. Do not keep the workaround only in Anchor memory or repeat the same warning in every Handoff.

## Interpretation Limits

This process does not grant semantic merge authority, cross-repository implementation ownership, automatic Role binding, human acceptance, publication/release permission, or authority to rewrite historical artifacts merely for cleaner presentation.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [002-cross-repository-work-turn-process.trace.md](002-cross-repository-work-turn-process.trace.md)
  - Value: _1dsgMDIFUHpMSI-bcLTn14-3QKm6CfIsorPDruQ2ZM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Iki4WHrUDupW1YcqT34MyBzwAzSQeIBYGJSxynO4t9Y