# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-11 12:38:12
  - Trace: [001-stream-day-parallel-major-001-orchestration.trace.md](../001-stream-day-parallel-major-001-orchestration.trace.md)
  - Origin:
    - [relative](../001-stream-day-parallel-major-001-orchestration.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-11 12:46:15
  - Authors: Anchor
  - Why: Sigma asked how far the refactor is from a worthy PoC replacement and explicitly wants valuable monolith behavior preserved rather than forgotten during decomposition.
  - Summary: Reconcile retained PoC product value against the refactored App/Site/Verse path before retirement or parity claims.
  - Status: ready/local

---

# Viewer Carrier Major 001 — PoC Replacement Re-Baseline

## Objective

Establish a truthful current product-contract delta between the historical Viewer PoC and the refactored App/Site/Verse architecture before any claim that the PoC can be retired or that missing behavior is intentionally gone.

## Done Criteria

- Start from the carried local Site PoC product-contract inventory, Viewer parity lineage and current App parity ledger rather than remote-first rediscovery.
- Reconcile the historical user loops across ingress/workspaces, read/navigation, actions/authoring, persistence/recovery, source/history, export/publication and truthful presentation.
- Classify each discovered PoC product value as `KEEP`, `CHANGED INTENTIONALLY`, `DROP WITH REASON`, or `UNKNOWN` with exact current-source evidence and owner boundary.
- Distinguish "implemented somewhere" from "proven in the refactored product path"; a partial ledger state remains partial until current integration evidence exists.
- Identify which retained values already have current implementation/tests, which require later implementation Majors, and which are blocked by missing historical evidence.
- Use an explicit targeted historical source read only when the carried local evidence cannot resolve a real unknown; remote lookup does not become the default discovery path.
- Produce a bounded next-Major sequence and an explicit PoC retirement gate; do not retire the PoC in this Major unless all required product values and Sigma acceptance evidence are actually qualified.

## Scope

Product-contract discovery/reconciliation only. Current App/Site/Verse source may be read and locally exercised for evidence, but broad implementation, visual redesign, release/deployment and unrelated feature work are outside this Major.

## Initial Local Evidence

- `site::.topics/viewer/001-1-poc-product-contract-inventory-discovery.trace.md` and its seven product-contract groups.
- Site Viewer parity Tasks/Decision/Reduction through current human authoring/Handoff package work.
- `app::src/parity/poc.parityLedger.js` and current scenario definitions/tests.
- Current App source surfaces for Workspace lifecycle, Feed/Tree/Lineage, authoring, Time Portal, publication and export.
- Current `verse-native` frontier, including any still-empty extraction/export boundary that prevents honest replacement claims.

## Safety Invariants

- Exact PoC implementation details are evidence, not automatic requirements; preserve product value, not monolith accidents.
- Missing behavior stays `UNKNOWN` until evidence supports KEEP/CHANGE/DROP.
- Do not infer semantic authority from Site/App placement or parity labels.
- Do not use a successful unit/acceptance test as a substitute for Sigma browser/product acceptance where the contract is experiential.
- Carrier Major 001 scope is this re-baseline; implementation findings become explicit next-Major candidates rather than silently expanding the current Major.

## Dependencies

- Current audited Anchor full recovery and local-first materialization.
- Carried Site, App, Core, Docs, verse-native and Business Workspaces.
- Historical PoC source only if a specific unresolved product-contract question cannot be answered from carried evidence.
- Sigma retains the final human decision to retire the old PoC.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-stream-day-parallel-major-001-orchestration.trace.md](../001-stream-day-parallel-major-001-orchestration.trace.md)
  - Value: XVBIK1Q4XsLJQCqk_bq8MYdQKtMcwCt_2zSdwyHtSKQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: wz1PGnrabH3tF_luOd9jUI6KJLopuZHtqa3RzYyNLHg