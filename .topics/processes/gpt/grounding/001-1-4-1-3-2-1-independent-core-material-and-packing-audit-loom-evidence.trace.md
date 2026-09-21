# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 13:52:53
  - Trace: [001-1-4-1-3-2-anchor-to-loom-independent-core-material-and-packing-audit.trace.md](001-1-4-1-3-2-anchor-to-loom-independent-core-material-and-packing-audit.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-2-anchor-to-loom-independent-core-material-and-packing-audit.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 14:18:27
  - Authors: Loom
  - Why: Return the independent Core-mechanical audit required before Anchor reconciliation and any further implementation.
  - Summary: Source-grounded Loom audit of Core material closure, participant authority, cache representation, references, and failure timing.
  - Status: ready/local

---

# Independent Core Material And Packing Audit — Loom Evidence

## Supported Claim Or Question

- Supported Claim Or Question: whether current Core material closure, Handoff manufacture, participant projection, reference/internal-binding mechanics, cache carriage, and failure timing are mechanically sound enough for Anchor reconciliation before further implementation
- Evidence Role: independent Loom audit evidence that identifies one source-proven participant-authority qualification defect, one fail-timing refactor seam, several non-defects, and semantic questions that must remain with Axiom/Anchor reconciliation
- Review Context: controlling Architecture Recovery Audit Before Further Host Mutation; audit only, no Core mutation

## Provenance

- Known Source: exact Core and Docs Workspace snapshots qualified from the selected Anchor to Loom Handoff carrier, plus the exact selected Business task/Handoff and read-only local execution against those carried Core bytes
- Preservation Basis: this artifact preserves source paths and line ranges, test/probe outcomes, defect/non-defect disposition, and the minimal proposed correction and acceptance surface; exact Core and Docs snapshots remain separately carried source authority
- Provenance Limits: no production files in Core or Docs were changed; the focused Node test command timed out after 180 seconds after ten completed passing subtests, so this evidence does not claim the full Core suite passed; the temporary participant-integrity probe was executed outside the Core Workspace and is summarized here rather than promoted to canonical test source
- Source Artifact: [Controlling Audit Task](001-1-4-1-3-architecture-recovery-audit-before-further-host-mutation.trace.md)

## Evidence Material

- Material: PROVEN DEFECT — `src/tooling/portable/adapters/node/handoff.manufacture.requirements.js:60-134,211-240` labels `resolveNearestQualifiedTaskRecord` as qualified but accepts a Task after only parsing Current Schema plus the presence of continuity/integrity sections; it does not verify Task self-integrity or exact schema contract before `explicitTaskParticipantDeclarations` becomes semantic authority. A read-only probe sealed a valid Task, then changed the participant declaration without resealing it; `validatedC14nV2PrimarySelfDigest` returned `mismatch/digest-mismatch`, while `projectSemanticParticipantManufacturingRequirements` still returned route `state: qualified`, one Sigma declaration, one participant Role requirement, and zero findings. Minimal Core correction: require exact Task schema/self-integrity qualification at the participant-authority source boundary before deriving declarations, and fail closed with a dedicated finding when the current-work Task cannot qualify. NON-DEFECT — manual route participant input cannot itself create participation (`handoff.manufacture.requirements.js:96-113`), exact Role material is independently byte/self-integrity qualified before participant use (`handoff.manufacture.requirements.js:242-286`), and existing regressions confirm carriage/cache inventory alone does not create participant authority. FAIL-TIMING REFACTOR — `src/tooling/portable/adapters/node/handoff.manufacture.js:41-48` starts tooling-bootstrap construction before semantic/material closure is known; workspace enumeration starts before requirement projection, while requirements and semantic participant projection occur around `:180-191`; `src/tooling/portable/handoff/materialClosure.archiveV2.direct.js:14-21` computes closure readiness but still constructs the base export bundle, and the public manufacture facade proceeds into archive upgrade/inspection before final blocked status. This is late/costly failure rather than demonstrated source mutation. Minimal correction: split/hoist blocking selected-Handoff/current-work/material preflight so failed semantic/closure inputs stop before bootstrap archive construction and recipient package assembly. CACHE DISPOSITION — Core already routes bounded Workspace source through generic Material Representation machinery (`src/tooling/portable/handoff/recipientV2.packageV1.build.js:43-68`), consistent with canonical Docs `tiinex.handoff.package.v1` requirements that bounded source use `Material Representation Bindings`; detached route or bounded-parent recovery bytes are separately coalesced into `*-cache.zip` with numbered `.bin` entries and a visible `tiinex.external.payload.v1` descriptor (`recipientV2.packageV1.build.js:132-154`). Canonical Docs explicitly permits bootstrap/cache descriptors under their owning schemas and sets `Derived Inventory Authority: none`; therefore cache presence is not itself a semantic-authority defect. It is an inspectability debt: textual detached bytes are not directly human-readable at the carrier surface. A safe Core refactor may preserve exact bytes while using stable safe source-shaped archive entry names/media extensions or equivalent visible text projection; replacing detached parent recovery with a bounded Workspace Representation requires Axiom/Docs disposition if it would widen the representation's exact bounded scope. REFERENCE/BINDING NON-DEFECT — Core maintains separate semantic/reference text and internal exact Workspace/path binding; explicit endpoint Role bindings use `targetWorkspaceId`/`targetPath` and cross-check a workspace-qualified `reference` for contradiction (`handoff.manufacture.requirements.js:170-180`), while material closure keeps provenance/provider fields disposable. Do not collapse these layers. SEMANTIC BLOCKER — canonical Handoff permits Party endpoint Capacity/Capacity Reference as optional resolution aids and requires unresolved/contradictory capacity references to stay unresolved; Core material closure currently synthesizes endpoint material requirements only for `Kind: role` (`src/tooling/portable/handoff/materialClosure.requirements.js:68-97`). Whether Party capacity material must be package-closed/qualified is a Docs/Axiom semantic decision, not a Core-only change. REQUIRED-MATERIAL NON-DEFECT — closure planning blocks unresolved, ambiguous, or integrity-conflicted Required Context, endpoint Role, participant Role, and dependency material while Reference Context ambiguity remains non-blocking warning, matching Required-versus-reference semantics. CURRENT CARRIER OBSERVATION — the selected audit route's three Required Context items resolved from qualified Workspace archive entries, not cache entries, so opaque cache is not universal to current Handoff carriage. TEST EVIDENCE — focused `node --test test/handoff-participant-projection.test.mjs test/manufacture-hygiene.test.mjs test/blank-workspace-role-cache-grounding.test.mjs` completed ten subtests with ten passes and zero completed failures before the 180-second command timeout; these included exact route-bounded Role/Required Context closure, Anchor/Axiom/Anchor Role roundtrip, holder/delegate separation, Pilot delegation plus Sigma participant projection, manual participant negative case, cache authority negative case, complete-route no-cache projection, sibling bounded-cache ancestor closure, and external Parent closure.
- Material Kind: source-grounded implementation audit summary plus read-only adversarial probe and focused regression execution
- Description: Minimal acceptance surface before implementation: add a direct unit regression where a stale-self-integrity Task containing an otherwise lexical participant declaration produces no semantic participant requirement and an explicit blocking finding; add an end-to-end manufacture regression with a valid selected Handoff whose current-work ancestry includes the tampered Task and assert manufacture blocks before package assembly; retain the existing manual-input/cache-authority negatives; add instrumentation or a seam-level test proving bootstrap/archive builders are not entered after a blocking semantic/material preflight; add a transparent-cache representation test asserting textual detached material has a deterministic inspectable entry identity without changing digest, scope, or semantic authority; after Axiom disposition, add Party-capacity tests only for the semantics actually adopted.

## Preservation And Fidelity

- Preservation State: embedded audit summary grounded in exact carried source snapshots and read-only runtime outputs
- Fidelity Notes: source paths and line ranges refer to the exact Core/Docs bytes materialized by qualified Tiinex continuation; the participant-integrity defect is reproduced directly against those Core modules; non-defect and refactor conclusions distinguish observed mechanics from semantic ownership
- Known Losses: full-suite completion is unavailable because the focused multi-file test command exceeded the execution window after ten passing subtests; no claim is made about unrelated Core modules or Extension VS Code behavior

## Interpretation Limits

- Does Not Prove: that every cache mechanism is defective, that cache bytes have semantic authority, that replacing cache with Workspace Representation is semantically valid, that Party capacity references must become required closure, that the whole Core suite passes, or that any implementation is authorized
- Must Not Be Treated As: Anchor reconciliation, Axiom semantic disposition, program acceptance, VS Code host audit, release approval, or permission to mutate Core before the independent returns are reconciled
- Not Yet Used As: implementation authorization, accepted Core correction plan, release evidence, or program completion evidence
- Need For Review: Anchor should reconcile this Core-mechanical return with Axiom's endpoint/reference/material semantic disposition and Kodax's host-boundary audit before authorizing implementation
- Authority Limits: Loom audit/disposition only; Core implementation, canonical Docs changes, release, publication, deployment, and remote mutation remain unauthorized

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-2-anchor-to-loom-independent-core-material-and-packing-audit.trace.md](001-1-4-1-3-2-anchor-to-loom-independent-core-material-and-packing-audit.trace.md)
  - Value: xLska9WeNlgCuWLLNTztJtkUegX5350kFD5oQbYwCYw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: JLteuSNYC14vVepvcf6Dx6QTIAyr_0iETGvRIKkiE-w