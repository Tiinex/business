# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 15:34:51
  - Trace: [004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md](../../handoffs/004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md)
  - Origin:
    - [relative](../../handoffs/004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 15:42:51
  - Authors: Anchor
  - Why: Continue today's Viewer objective under the corrected Carrier Major boundary without rewriting earlier misnumbered transport history.
  - Summary: Delegate bounded local-first Viewer PoC product-contract reconciliation to Kodax under Carrier Major 002.
  - Status: ready/local

---

# Anchor to Kodax — Viewer Carrier Major 002 PoC Replacement Reconciliation

## Handoff Parties

- Purpose: complete the current local-first Viewer PoC replacement re-baseline as a bounded technical reconciliation so Anchor can plan later implementation Majors without silently dropping useful PoC behavior.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-kodax-role.trace.md)

## Transfers

- poc-contract-reconciliation
  - Transfer Kind: work-and-responsibility
  - Description: reconcile the seven preserved PoC product-contract groups against the current refactored App/Site/Verse/Provider path using carried local material first. Classify each retained user-visible value as KEEP, CHANGED INTENTIONALLY, DROP WITH REASON, or UNKNOWN with exact source evidence.
  - Controlling Artifact: [Viewer re-baseline discovery](../viewer/001-1-viewer-major-001-local-re-baseline-starting-discovery.trace.md)
  - Boundary: historical implementation accidents and exact monolith styling are evidence, not automatic requirements.
- parity-ledger-disposition
  - Transfer Kind: work
  - Description: review the current App PoC parity ledger scenario-by-scenario and distinguish implementation gap, composition gap, browser/manual evidence gap, intentionally changed behavior, or stale ledger state. Do not upgrade any scenario beyond its evidence.
  - Boundary: code presence or unit tests alone are not Sigma product acceptance.
- next-major-plan
  - Transfer Kind: work
  - Description: return the smallest ordered Viewer implementation/qualification Major sequence needed to reach a truthful PoC retirement gate, including any targeted historical source read that remains genuinely necessary.
  - Boundary: do not silently expand this reconciliation into broad product implementation.

## Required Context

- app-workspace
  - Material: Complete current App Workspace.
  - Material Reference: [App Workspace](app::.topics/.workspaces/tiinex-app.workspace.md)
  - Purpose: Current Viewer/application implementation and PoC parity ledger.
  - Availability: available
- site-workspace
  - Material: Complete current Site Workspace including preserved PoC product-contract inventory and Viewer parity lineage.
  - Material Reference: [Site Workspace](site::.topics/.workspaces/tiinex-site.workspace.md)
  - Purpose: Historical product-contract evidence and current host composition.
  - Availability: available
- verse-native-workspace
  - Material: Complete current Native Verse Workspace.
  - Material Reference: [Native Verse Workspace](verse-native::.topics/.workspaces/tiinex-verse-native.workspace.md)
  - Purpose: Exact current extraction/export boundary.
  - Availability: available
- business-workspace
  - Material: Current Business orchestration, role and Viewer Major context.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: Controlling plan and return context.
  - Availability: available
- docs-workspace
  - Material: Current canonical semantic contracts.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: Read-only semantic boundary where product behavior touches canonical meaning.
  - Availability: available

## Reference Context

- prior-viewer-rebaseline
  - Material: [Viewer Carrier Major 001 re-baseline task](../viewer/001-viewer-carrier-major-001-poc-replacement-re-baseline.trace.md) and its local-first discovery child.
  - Purpose: Preserve the already-established product-contract questions and avoid restarting discovery from chat or remote-first assumptions.
  - Availability: available
- stream-day-plan
  - Material: [Stream-Day Parallel Major orchestration](../001-stream-day-parallel-major-001-orchestration.trace.md)
  - Purpose: Preserve the original bounded Viewer objective while correcting the carrier-major transport boundary prospectively.
  - Availability: available

## Retained Responsibilities

- major-scope-and-retirement-gate
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
  - Responsibility: decide the next Viewer Carrier Major sequence and whether evidence is sufficient to approach PoC retirement.
  - Boundary: Kodax returns technical reconciliation; Anchor retains orchestration.
- human-product-acceptance
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-sigma-role.trace.md)
  - Responsibility: browser/product acceptance and final decision that the old PoC can be retired.
  - Boundary: technical reconciliation is not human acceptance.

## Exclusions And Dependencies

- broad-implementation
  - Kind: excluded-scope
  - Description: Do not implement the full remaining Viewer surface in this Handoff; produce a precise evidence-backed delta and next sequence first.
  - Responsible Party Or Role: later explicit Viewer implementation Major.
- remote-first-research
  - Kind: excluded-scope
  - Description: Use carried local evidence first. Targeted historical remote source may be proposed only for a concrete unresolved product-contract question.
  - Responsible Party Or Role: Anchor approval before external recovery when needed.
- release-and-deploy
  - Kind: excluded-scope
  - Description: No deployment, publication, package release, remote push or PoC retirement is authorized.
  - Responsible Party Or Role: explicit later gates.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: Return a bounded technical Evidence/reconciliation artifact plus one normal Handoff to Anchor, with the seven PoC product-contract groups and current parity scenarios dispositioned as far as exact carried evidence allows, explicit UNKNOWNs only where evidence is truly missing, and a small ordered next-Major sequence.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Interpretation Limits

- Does Not Mean: PoC parity, PoC retirement, Native Verse completeness, Sigma acceptance, or authorization for broad implementation.
- Must Not Be Used To Claim: Carrier Major 002 maps to artifact filename 002; Site/App placement creates semantic authority; historical implementation detail is automatically required; or a partial ledger entry is a proven defect.
- Authority Limits: bounded Viewer technical reconciliation only.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md](../../handoffs/004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md)
  - Value: 0j4-TtEoAW-aqCwb78kARR1WFGcUXZmsJ4TfpapN4x8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: -Ll5saPjMnoeu1bzgE3FeFsv012Fw7ZYzR027YbRqag