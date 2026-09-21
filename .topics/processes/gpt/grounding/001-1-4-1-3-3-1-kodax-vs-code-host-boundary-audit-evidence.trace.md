# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 13:52:55
  - Trace: [001-1-4-1-3-3-anchor-to-kodax-independent-vs-code-host-boundary-audit.trace.md](001-1-4-1-3-3-anchor-to-kodax-independent-vs-code-host-boundary-audit.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-3-anchor-to-kodax-independent-vs-code-host-boundary-audit.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 14:16:29
  - Authors: Kodax
  - Why: Return independent Kodax audit evidence to Anchor before any further host mutation.
  - Summary: Source-grounded Extension VS Code boundary, failure-seam, monolith, lifecycle, and acceptance audit.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: Does the carried Extension VS Code host preserve a thin host/shared boundary and adequate machine-level operator acceptance before further host mutation?
- Evidence Role: Independent Kodax source audit evidence for Anchor reconciliation; supports bounded architecture and acceptance decisions without authorizing implementation.

- Question: does the current Extension VS Code host preserve a thin host/shared boundary across Incoming, Replace, Outgoing, Attach, participant selection, Pack, Transport, Core binding, restart/session lifetime, and controller-level acceptance?
- Supported conclusion: the carried Extension VS Code source has one confirmed source-grounded semantic-owner violation around participant removal, one material host-session lifetime seam, one dominant controller-monolith hotspot, one sizeable legacy/suspect receive implementation that is no longer runtime-reachable, and an acceptance gap because current tests do not execute the operator flow in a real VS Code Extension Host.
- Boundary conclusion: most local filesystem/Git mutation, VS Code presentation, progress/error UI, workspace selection, and destination-local file publication are legitimate host responsibilities. Core projections/manufacture are already the semantic source for route, participant, carrier-allocation, and transport-text truth. The correction should therefore thin and constrain the host rather than move all host logic into Core.

## Provenance

- Known Source: Tiinex-qualified carried Extension VS Code and Core workspace snapshots from the selected Kodax Handoff route in the received carrier.
- Preservation Basis: Exact nested workspace archive byte identities were qualified by Tiinex before read-only extraction for audit.
- Provenance Limits: Runtime dependencies were not carried, so the audit is source-grounded except where explicitly described as an attempted but blocked baseline command.

- Received carrier: `tiinex-002-1-anchor-to-axiom-and-loom-and-kodax.handoff-package.zip`, qualified SHA-256 `5e8e192a510bc80b3473c1fdca3f01e1e014fd4c935d40cb0d76557c65e74d8e`.
- Selected route: `001-3-3-1-1-handoff-pointer.trace.md` -> `business::.topics/processes/gpt/grounding/001-1-4-1-3-3-anchor-to-kodax-independent-vs-code-host-boundary-audit.trace.md`.
- Extension VS Code carried workspace archive: `001-6-extension-vscode.workspace.zip`, qualified byte size `3840466`, SHA-256 `df886043c5183c4e6d015c7d22a6dddf34c9449fb8fac5ae61873b0abebe4024`.
- Core carried comparison workspace archive: `001-4-core.workspace.zip`, qualified byte size `8565085`, SHA-256 `32e9cbad1e72d66d11efc579de7b8fadef89b3bfdc8c70978746556ff260a4b0`.
- Audit basis: read-only inspection of the two qualified carried workspace snapshots after Tiinex grounding. No Extension VS Code, Core, or outer-carrier source bytes were modified.
- Baseline command attempted from the qualified Extension VS Code snapshot: `npm test`. It did not reach extension tests because the source-only carrier has no `node_modules`; TypeScript stopped on unavailable Node/VS Code type definitions. This is an environment limitation, not a product-test failure, and no runtime failure claim below depends on it.

## Evidence Material

- Material: Boundary map, monolith/legacy hotspots, participant-authority and restart seams, Core-binding observations, test-surface assessment, and a minimal host-thinning/controller-E2E plan derived from the qualified carried source snapshots.
- Material Kind: Read-only source/control-flow audit with exact carrier/workspace archive provenance.

### Host/shared boundary map

- Host-only and legitimate adapter responsibilities:
  - `src/extension.ts`: command registration, activation lifecycle, VS Code error presentation, compatibility command routing.
  - `src/operatorTrees.ts`: TreeView projection, dialogs/QuickPick, progress notifications, clipboard/reveal actions, VS Code context keys, workspace-state presentation, and orchestration entrypoints are host responsibilities even though the file currently owns too many of them at once.
  - `src/incomingApply.ts` plus `src/host/git.ts`: local repository precondition checks and filesystem/Git mutation for Merge/Replace are host execution responsibilities. The flow delegates incoming comparison/projection to shared Core and rechecks mutation preconditions before executing.
  - `src/host/carrierPublish.ts`: destination-local collision detection and fail-closed publication are host filesystem mechanics. Qualified carrier naming/allocation remains Core-derived.
  - `src/host/corePackageBinding.ts`, `src/tiinex/bootstrap.ts`, and `src/packageBuilder.ts`: legitimate binding/adaptation surfaces when they consume exact Core projections and fail closed instead of inventing semantic authority.
  - Transport queue/prepared-state persistence is presentation state and is appropriately stored in `workspaceState`; exact manufactured transport receipts are keyed by package path and SHA-256.
- Shared/Core-owned truth already visible in the host:
  - participant authority is projected by Core and intentionally described in `pickCoreQualifiedParticipantSet` as an exact required set;
  - package manufacture, route allocation, carrier allocation, and exact transport text are obtained from shared tooling rather than reconstructed in UI code;
  - Incoming delta/comparison uses shared `compareIncomingWorkspaceToLocal` before host mutation.
- Review candidates rather than established defects:
  - `src/core/receivedHandoff.ts`, `src/core/sourceSelection.ts`, and adjacent pure helpers parse or reshape qualified receipts for host presentation. They should remain receipt adapters only; any future semantic rule added there should instead be projected by Core.
  - `src/core/outgoingUx.ts` contains presentation and filename/frontier helpers. Current comments and package-builder checks preserve Core ownership of qualified carrier allocation, so this is not established as a semantic defect; keep the distinction explicit during thinning.

### Confirmed semantic-owner violation: participant set can be weakened after Attach

- `pickCoreQualifiedParticipantSet` explicitly states that Core owns semantic participant authority and that the projected participant set is exact. Attach refuses a partial user selection and stores the exact projected roles.
- The exposed `tiinex.outgoing.removeParticipantPointer` command later calls `tracked.participants.splice(index, 1)` in `removeOutgoingParticipantPointer` without re-running Core projection or requalifying the Handoff.
- `packageOutgoing` forwards `participantRoles: item.participants` for every attached route to `buildHandoffPackageFromForm`.
- Therefore the host can transform a previously exact Core-qualified set into a partial subset after Attach. That is a semantic-owner violation in the host and shifts rejection from Attach to later Pack/manufacture qualification.
- Existing tests simultaneously assert that Attach must keep the exact Core-qualified set and that the remove-participant command/menu exists, but do not execute the end-to-end state transition proving those two behaviors remain coherent.

### Restart/session lifetime seam

- `TiinexOperatorTrees` initializes `private incoming: IncomingState[] = []` and `private outgoing: OutgoingState | null = null`.
- `start()` restores Transport queue/prepared state, refreshes Discovery, updates UI contexts, and resumes only the dedicated multi-root Incoming handoff via `consumeIncomingMultiRootResume`.
- The only general `workspaceState` persistence for operator session data covers Transport, tree display preferences, and the Outgoing bootstrap-payload preference. There is no general serialization/restoration of Incoming packages, Outgoing workspace selection, attached Handoffs, exact participant projections, package parent topology, drafts, or `lastBuilt`.
- The multi-root Incoming resume file is a deliberately narrow exception used around `vscode.openFolder`; it does not establish general Incoming/Outgoing session durability.
- Result: an Extension Host restart can discard an in-progress Outgoing composition and ordinary Incoming review state even though Transport presentation state survives. This is a host lifecycle seam; the product contract should either persist/requalify resumable state or explicitly treat it as ephemeral and prove that behavior in acceptance tests.

### Monolith and legacy/suspect hotspots

- `src/operatorTrees.ts` is `4628` lines in the carried snapshot. It owns Discovery, Incoming qualification and presentation, Merge/Replace entrypoints, Outgoing composition, Handoff authoring/attachment, participant selection, package-parent topology, Pack, Transport qualification/presentation/persistence, artifact/material navigation, tree rendering, error/progress presentation, and restart behavior. This concentrates change coupling across otherwise separable host controllers.
- `src/core/*` contains about `1915` lines of pure host-side helpers. Many are useful extraction targets for host view models, but the `core` folder name makes semantic ownership easy to blur; these are Extension-local helpers, not `@tiinex/core` authority.
- `src/landing.ts` is `410` lines and still has source-pattern tests, but no runtime source imports it. `tiinex.landHandoffPackage` in `src/extension.ts` now routes directly to `trees.openIncoming`. This makes `landing.ts` a legacy/suspect implementation surface rather than a second live Incoming path. It should not be used as evidence of current operator behavior and should be removed only after compatibility/test references are deliberately reconciled.

### Local/Published Core binding seam

- The Extension manifest and lock target `@tiinex/core ^0.35.0` / locked `0.35.0`.
- The carried current Core comparison snapshot identifies `@tiinex/core` version `0.1.1`.
- Explicit Local mode intentionally permits binding the configured sibling source even when its manifest version differs from the durable published lock; Published mode remains strict. `test:local-core` also validates a disposable exact-local-source installation without mutating the durable manifest/lock.
- The version difference is therefore not itself a defect. It does mean Local and Published are materially different acceptance surfaces and both must be exercised at controller level before a candidate is presented to Sigma.

### Acceptance-surface gap

- `test/run.mjs` has broad pure/module and source-contract coverage, including participant projection, Core-binding restart behavior, package mechanics, and a mocked activation check.
- The activation test monkeypatches Node module loading to supply a fake `vscode` object. Numerous operator tests read `src/operatorTrees.ts`, `src/landing.ts`, `src/incomingApply.ts`, and other files as text and assert source patterns.
- `package.json` has no real VS Code Extension Host test dependency such as `@vscode/test-electron`; `test:package` is package/VSIX integration, not an operator-flow Extension Host run.
- Consequently the current suite does not machine-exercise a real command -> controller -> TreeView/workspaceState -> filesystem/Git -> Core projection/manufacture lifecycle, and cannot catch the exact-set Attach followed by participant-removal/Pack seam or ordinary Incoming/Outgoing restart loss.

### Minimal host-thinning and controller-E2E plan

1. Participant authority: remove the host capability to weaken a Core-qualified participant set, or make any participant change an immediate Core re-projection that must reproduce the exact qualified set before state is committed. Treat the qualified participant projection as immutable host state between Attach and Pack.
2. Controller split without semantic relocation: extract `operatorTrees.ts` into bounded host controllers for Discovery, Incoming, Outgoing/authoring, Transport, and material navigation. Keep one thin composition/root controller for VS Code registration/context wiring. Move only host state/presentation; do not recreate Core semantics in the extracted controllers.
3. Legacy cleanup: retire `src/landing.ts` and its source-pattern assertions only after confirming no external compatibility surface still calls it. Keep the public compatibility command, which already routes to native Incoming.
4. Session contract: define the intentional durability boundary for Incoming and Outgoing. If resumable, persist only identifiers/host choices, then re-open and requalify package/Handoff/participant/Core state on restart rather than trusting serialized semantic receipts. If ephemeral, surface that explicitly and test it.
5. Machine-level Extension Host acceptance before Sigma:
   - activate the packaged/development extension in an actual VS Code Extension Host fixture with temporary repositories;
   - open a qualified carrier through the public Incoming command and prove blocked/unqualified inputs are non-mutating;
   - exercise Merge and Replace through commands/controller state, including dirty/conflict handling and multi-root resume;
   - create/select Outgoing, attach a Handoff, obtain the exact Core participant projection, and prove host UI cannot retain a partial set;
   - Pack and verify the produced carrier re-qualifies and Transport presents the exact Core-projected transport text;
   - restart/reload the Extension Host mid-Incoming and mid-Outgoing and verify the declared durability contract;
   - run the same controller flow once against exact Local Core source and once against the lock-qualified Published Core binding.
6. Do not use Sigma as the debugger for any of the above. Reconcile this Kodax evidence with Axiom/Loom findings first, implement only the reconciled minimal change, then require the machine-level host flow to pass before another live replay.

## Preservation And Fidelity

- Preservation State: Qualified source snapshots preserved unchanged; audit findings authored separately in the Business continuation workspace.
- Fidelity Notes: Findings distinguish directly source-grounded behavior, environment-limited baseline execution, and review candidates; no runtime behavior is claimed where it was not executed.
- Known Losses: No live VS Code Extension Host execution evidence was available because the carried Extension snapshot omitted installed dependencies.

- All findings above are tied to exact carried archive identities recorded in Provenance.
- “Confirmed” means directly established by static source/control-flow inspection of the qualified carried snapshot; it does not mean reproduced in a running VS Code Extension Host.
- The attempted baseline did not execute because dependencies were absent from the source carrier. No failed compile/test result has been reclassified as a product defect.
- No inference was made from `src/landing.ts` as an active runtime receive path after confirming it has no source importer and the compatibility command routes into `TiinexOperatorTrees`.
- No Extension VS Code or Core source mutation, refactor, deletion, release, publication, or remote write was performed.

## Interpretation Limits

- Does Not Prove: It does not prove every large module is wrong, that all Extension-local helpers belong in Core, or that all observed operator failures share one root cause.
- Not Yet Used As: This evidence has not yet been reconciled with Axiom/Loom returns or used as implementation, Sigma, release, or publication authority.
- Must Not Be Treated As: Runtime reproduction, Core semantic authority, Sigma acceptance, release readiness, or authorization to mutate Extension VS Code or Core source.

- This evidence does not claim that every large module belongs in Core, that all Extension-local `src/core/*` helpers are semantic duplication, or that all Sigma-observed failures share one root cause.
- It does not establish a Core semantic defect. The participant issue is specifically a host mutation of already-projected Core authority.
- It does not claim runtime reproduction of the participant or restart seams; those are source-grounded and are exactly why a real Extension Host acceptance layer is required.
- It does not authorize implementation. Anchor retains reconciliation and implementation authorization under the controlling audit task.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-3-anchor-to-kodax-independent-vs-code-host-boundary-audit.trace.md](001-1-4-1-3-3-anchor-to-kodax-independent-vs-code-host-boundary-audit.trace.md)
  - Value: wXQA-E_OUgmhMfTZEy7FbNCISRNQvxtym1W4h6aCAPM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 6ZYaCPwWYMzLfKItJk7BuMTlxyo4wBztwEMEENQErQ0