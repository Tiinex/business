# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 18:38:24
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-3-anchor-to-loom-real-host-sigma-gate-shared-mechanics-recovery-package-correction.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-3-anchor-to-loom-real-host-sigma-gate-shared-mechanics-recovery-package-correction.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-3-anchor-to-loom-real-host-sigma-gate-shared-mechanics-recovery-package-correction.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 19:04:57
  - Authors: Loom
  - Why: Return the Anchor-authorized shared-mechanics recovery with exact source delta, tests, ownership boundaries, and residual integration risks.
  - Summary: Exact bounded Core endpoint-source and optional endpoint-material corrections plus Workspace-integrity ownership evidence and regressions.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: Which of the failed real-host Sigma gate seams are owned by shared Core mechanics, what exact Core correction is warranted, and which failure remains host-owned?
- Evidence Role: Loom implementation and ownership evidence for Anchor reconciliation of the bounded real-host Sigma gate shared-mechanics recovery tranche.

- Supported conclusion: two of the three transferred seams require bounded Core correction. Endpoint projection now admits Role/Party material only through one explicitly selected, exactly qualified Workspace material authority and excludes repository-wide/nested `.topics` material from that selected surface. Handoff endpoint References remain schema-optional: absent References create optional unresolved transport closure, while explicit References remain required and contradictions still fail closed.
- Supported ownership conclusion: Core's Workspace self-integrity qualification and Pack preflight already preserve and verify exact Workspace bytes. Exact source/incoming/local byte identity qualifies; the first byte drift produces both observed Sigma blocker codes. No Core writer in the audited path mutates those Workspace bytes. The observed real-host drift therefore remains a host/Kodax byte-write-or-switch investigation, not a Core sanitization target.
- Scope boundary: no Docs/schema widening, no Role schema-authority substitution, no Extension VS Code mutation, no release/publication, and no attempt to convert host presentation/label policy into Core semantics.

## Provenance

- Known Source: Tiinex-qualified Anchor -> Loom route from the received carrier `business-002-1-4-1-1-1-1-1-1-1-anchor-to-loom-and-kodax.handoff-package.zip`.
- Preservation Basis: cold-started from the carrier Start trace, verified the declared bootstrap payload, grounded the exact Loom pointer through Tiinex, and materialized the qualified Business and Core representations through Tiinex continuation/representation evidence before mutation.
- Provenance Limits: the real Extension Host's mutated Workspace bytes were not transferred to Loom. Workspace ownership is therefore established by exact Core-path byte invariants and mutation boundaries, while the first host mutation site remains a Kodax integration question.

- Received outer carrier SHA-256 from continuation state: `9a96ca1a644bff873d43a9078b0cc26b26cd37bd7515cb65aec890aeae0fa669`.
- Selected route pointer: `001-3-1-1-1-handoff-pointer.trace.md`.
- Controlling Anchor -> Loom Handoff: `business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-3-anchor-to-loom-real-host-sigma-gate-shared-mechanics-recovery-package-correction.trace.md`.
- Controlling Task: `business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-real-host-sigma-gate-root-cause-recovery.trace.md`.
- Sigma blocker Evidence: `business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-sigma-real-host-gate-blocker-evidence.trace.md`.
- Qualified received Core representation payload: `001-4-core.workspace.zip`, SHA-256 `2ff12a1af5b9254604f8ccedd5c742f9db84ef9c75ed5f47bbd8f4c856a1b8c7`, Coverage `complete`, Binding State `verified`.
- Current Core Workspace artifact exact bytes remain unchanged by this tranche: `.topics/.workspaces/tiinex-core.workspace.md`, 1516 bytes, SHA-256 `3ee262e761c1c3a64b62608cdbc53677a52fe706ce1b1c9c31f66e6042ed65c5`.
- An untouched materialized reference copy of the received Core tree was retained separately and used for the final source delta comparison.

## Evidence Material

- Material: exact Core delta, source/control-flow ownership trace, adversarial regressions, compatibility tests, and residual integration boundaries for the three transferred Sigma-gate seams.
- Material Kind: bounded implementation plus deterministic regression evidence against the qualified received Core snapshot.

### 1. Endpoint source eligibility — Core correction

- Prior Core seam: `projectQualifiedHandoffEndpoints` accepted every supplied exactly-qualified Role/Party-shaped record without first binding those candidates to an explicitly selected qualified Workspace/material authority. A host that supplied a repository-wide record set could therefore let nested fixture or other unrelated records enter the shared candidate projection.
- Correction: `handoffEndpointProjection.js` now resolves the requested package-local Workspace identity through `projectQualifiedWorkspacePackageSources`, requires exactly one exact qualified source candidate, derives that source's own `.topics` material root from its qualified Workspace target path, and rejects endpoint projection entirely when that source authority is unresolved, ambiguous, or lacks a qualified material root.
- Eligibility rule: endpoint Role/Party records are considered only when their exact path is inside that selected material root. A second `.topics` segment below the selected root is excluded, so nested fixture Workspaces cannot become part of the selected Workspace's endpoint surface. If that nested Workspace is itself explicitly selected, its own `.topics` becomes the material root and can be evaluated independently.
- Identity rule preserved: candidate identity remains `workspaceId::artifact-path`; candidates are sorted deterministically and are not collapsed by human label. Same-label exact candidates therefore remain distinct at the Core projection boundary. Host-side human-label recency/collapse remains Kodax-owned and is not reproduced in Core.
- Qualification rule preserved: the existing exact Role/Party runtime schema authority remains fail-closed. This tranche does not reinterpret an unqualified Role-shaped record as qualified material merely because it is inside a selected source surface.
- Existing independent issue retained: current `tiinex.party.role.v1` runtime lineage authority can fail closed on a compiled/source lineage mismatch already covered by `schema-lineage-source-authority.test.mjs`. That authority was deliberately not broadened or replaced in this endpoint-source repair.

### 2. Authoring -> Pack contract — Core correction

- Canonical premise retained from the controlling route: Handoff `From Reference` / `To Reference` are optional resolution aids. Their absence must not silently become a mandatory schema/material-closure requirement.
- Requirements projection now marks a Role endpoint with an explicit Reference as `closureStrength: required`; a Role endpoint with no Reference is `closureStrength: optional` and emits an informational `portable.handoff-material.endpoint-role.reference-absent-optional` finding rather than the prior missing-reference warning.
- `closureStrength` is carried through material resolution, plan binding/replay, closure descriptor, and readiness so downstream stages cannot accidentally re-promote optional absence into a mandatory blocker.
- Plan/readiness rule: `ambiguous` and `integrity-conflict` endpoint material always block. `unresolved` blocks only when the endpoint requirement is required. Optional unresolved endpoint material remains explicitly unresolved with an informational finding.
- Recipient-v2 pointer rule: a missing endpoint Role pointer target may be skipped only when the exact route-scoped closure descriptor contains exactly one matching endpoint requirement whose `closureStrength` is `optional` and whose disposition is `unresolved`. Required unresolved material, ambiguity, integrity conflict, route mismatch, or descriptor mismatch still fails closed.
- Positive explicit transport remains intact: existing exact route endpoint Role bindings can still close and carry endpoint Role material even when the Handoff itself omits optional References; explicit endpoint References remain required transport closure and fail closed if their exact material is absent.
- No Handoff schema fields were added and no optional Reference was made semantically mandatory.

### 3. Workspace self-integrity — Core ownership disposition

- `workspaceTargetConformance.js` already verifies exact c14n-v2 self-integrity and emits the two Sigma codes `workspace-target-self-integrity-mismatch` and `workspace-target-artifact-conformance-unqualified` when exact Workspace bytes no longer match their sealed self-integrity.
- Workspace initialization already seals generated Workspace self-integrity. Manufacture enumeration reads exact file bytes and calculates their digest; the landing plan inspected for this tranche is planning-only with `sourceMutation: false`.
- New byte-path regression copies the exact canonical Core Workspace artifact as source -> Incoming/Replace -> Local without transformation. All three exact byte images retain the same SHA-256 and `qualifyHandoffWorkspaceTarget` reports qualified/verified self-integrity.
- The regression then changes the first controlled byte content without resealing (`Tiinex/core` -> same-length `Tiinex/c0re`). The SHA-256 changes and qualification fails with both exact real-host Sigma blocker codes.
- Core therefore detects the drift at Pack/preflight but does not create it in the audited source -> plan -> enumerate -> qualify path. Repairing Core to normalize/reseal/sanitize host-written bytes would erase provenance and violate the fail-closed boundary. No such patch was made.
- Remaining owner question transferred to Kodax/Anchor: record exact bytes and SHA-256 at host source selection, Incoming/Replace write, Local switch/re-open, and immediately before Pack; the first changed byte boundary identifies the real host owner.

### Exact source delta

- Final comparison against the untouched received Core tree: 11 changed files, 0 added files, 0 removed files.
- Changed shared source files:
  - `src/tooling/portable/handoff/handoffEndpointProjection.js`
  - `src/tooling/portable/handoff/materialClosure.requirements.js`
  - `src/tooling/portable/handoff/materialClosure.materials.js`
  - `src/tooling/portable/handoff/materialClosure.plan.js`
  - `src/tooling/portable/handoff/materialClosure.readiness.js`
  - `src/tooling/portable/handoff/materialClosure.inputBinding.js`
  - `src/tooling/portable/handoff/materialClosure.inputBinding.support.js`
  - `src/tooling/portable/handoff/materialClosure.descriptor.js`
  - `src/tooling/portable/handoff/recipientV2.endpointRolePointers.js`
- Changed regression files:
  - `test/endpoint-role-route-binding.test.mjs`
  - `test/workspace-initialization.test.mjs`
- No canonical Docs files and no Extension VS Code files were changed.

### Regression and compatibility results

- `node --test test/endpoint-role-route-binding.test.mjs` -> 8/8 PASS, clean process exit. New coverage includes optional unresolved no-Reference manufacture, bounded explicitly-selected Workspace endpoint source eligibility, and explicit Reference required/fail-closed closure.
- `node --test test/workspace-initialization.test.mjs` -> 3/3 PASS, clean process exit. New coverage proves exact source/incoming/local bytes stay qualified and first host-side byte drift yields both exact Sigma integrity codes.
- Serial compatibility checks already completed cleanly in this tranche:
  - `test/minimal-carrier-material-transport-projection.test.mjs` -> 3/3 PASS.
  - `test/bounded-handoff-carrier.test.mjs` -> 1/1 PASS.
  - `test/handoff-participant-projection.test.mjs` -> 2/2 PASS.
  - `test/manufacture-hygiene.test.mjs` -> 10/10 PASS.
  - `test/manufacture-runtime-source-alignment.test.mjs` -> 4/4 PASS.
  - `test/source-frontier-comparison.test.mjs` -> 16/16 PASS.
  - `test/qualification-boundaries.test.mjs` -> 20/20 PASS.
  - `test/schema-lineage-source-authority.test.mjs` plus `test/canonical-role-authoring-cutover.test.mjs` -> 10/10 PASS.
- Additional post-hardening checks:
  - `test/secure-transport-v1.test.mjs` -> 8/8 PASS.
  - `test/release-integration.test.mjs` -> 1/1 PASS.
  - `test/master-release.test.mjs` -> 18/18 PASS.
  - `test/bootstrap-recovery.test.mjs` -> 2/2 PASS.
  - `test/package-surface.test.mjs` -> one test SKIPPED because `npm_execpath` is required to inspect the actual npm pack surface; no failure.
  - `test/blank-workspace-role-cache-grounding.test.mjs` reported its two observed subtests PASS, then the command process remained alive until the external command window timed out. It is therefore retained as reported PASS subtests plus process/harness timeout, not represented as a clean complete suite exit.
- All nine changed shared JavaScript source modules pass `node --check` after the final source-boundary hardening.

### Done-Criteria disposition

- The three real-host gate failures are preserved as distinct regressions/ownership evidence rather than collapsed into one generic blocker.
- Endpoint projection is now bounded by explicit qualified Workspace material authority; nested `.topics`, repository-wide scans, schema/example records outside the selected surface, caches, filename/label recency, and arbitrary readable Role-shaped Markdown cannot create endpoint authority through this shared projection.
- Same-label exact candidate identity remains distinct by exact target; no Core recency/label collapse was introduced.
- Optional endpoint References stay optional; unresolved optional endpoint material remains unresolved at allowed strength, while explicit References and contradictions fail closed.
- Role/identity-unresolved Handoff manufacture remains possible when exact endpoint transport is genuinely optional, and exact explicit route endpoint bindings continue to carry Role material when supplied.
- Workspace exact-byte integrity is verified in Core and first drift is detected; no unproven Core writer repair was invented.
- Local/Published binding semantics, host Outgoing/session behavior, positive real Extension Host participant UX, and Sigma human acceptance remain outside this Core tranche.

## Preservation And Fidelity

- Preservation State: the received Core source snapshot was retained untouched as a reference tree; implementation occurred in a separate materialized Core working tree. Business evidence is authored separately through Tiinex continuation.
- Fidelity Notes: source-delta counts and hashes were calculated from exact file bytes. Test claims distinguish clean process exits from skipped tests and from reported passing subtests followed by process timeout.
- Known Losses: Loom did not receive the exact mutated real-host Workspace byte image or a host timestamped source/Incoming/Replace/Local byte trace, so this evidence cannot name the first host statement that changed those bytes.

- Core Workspace self-integrity is not rewritten to conceal drift.
- Existing exact Role schema/runtime authority is not weakened to make endpoint tests artificially positive.
- No repo-wide label heuristic is introduced as semantic identity.
- No Handoff/Workspace schema contract is widened.
- No Extension VS Code source is mutated in this route.
- No remote mutation, release, publication, deployment, or push is performed.

## Interpretation Limits

- Does Not Prove: that the integrated VS Code endpoint picker is already corrected, that the host no longer collapses choices by human label/latest, that the actual host Workspace drift site is identified, that Published and Local host modes are both accepted, or that Sigma has accepted the operator flow.
- Not Yet Used As: release authority, publication authority, Docs semantic authority, host acceptance, or human acceptance.
- Must Not Be Treated As: permission to make optional Handoff References mandatory, permission to accept unqualified Role schema authority, permission to reseal mutated Workspace bytes, or proof that every real-host gate failure is Core-owned.

- Anchor must reconcile/accept the exact Core delta before downstream integration.
- Kodax retains the host fixes: bind the endpoint UI to the corrected bounded Core source surface without repo-wide/label-recency authority; remove or constrain host-only candidate widening; and capture exact Workspace bytes across source -> Incoming/Replace -> Local -> Pack to identify the first mutation boundary.
- The existing `tiinex.party.role.v1` runtime lineage-source mismatch remains an independent fail-closed authority condition. This evidence does not resolve or bypass it.
- Positive participant UX, Outgoing/session lifetime, real Extension Host controller flow, Local-vs-Published integration, and final Sigma replay remain downstream acceptance surfaces.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-3-anchor-to-loom-real-host-sigma-gate-shared-mechanics-recovery-package-correction.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-3-anchor-to-loom-real-host-sigma-gate-shared-mechanics-recovery-package-correction.trace.md)
  - Value: 3UqpEhLZhZKfTUIrPOZAfh5u4b076gyvrOUZPKf7_Wc

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: E84fsgBmJS49POoaWZCee974GK9lN8FmBP348p6Zz1M