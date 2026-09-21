# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 15:36:36
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-anchor-to-kodax-vs-code-core-boundary-recovery-and-extension-hos.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-anchor-to-kodax-vs-code-core-boundary-recovery-and-extension-hos.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-anchor-to-kodax-vs-code-core-boundary-recovery-and-extension-hos.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 16:03:38
  - Authors: Kodax
  - Why: Return exact implementation and fail-closed acceptance evidence to Anchor without advancing to Sigma.
  - Summary: Bounded VS Code host repair completed; required true Extension Host acceptance remains blocked by environment.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: Did the bounded Extension VS Code implementation remove host-local semantic weakening, enforce Core requalification at Pack and Transport/restart boundaries, and complete the required machine acceptance before Sigma?
- Evidence Role: Kodax implementation evidence and acceptance disposition for Anchor.

- Supported conclusion: the carried Extension VS Code source was changed only in the bounded host tranche. The confirmed participant-set weakening command was removed; public package-builder inputs no longer accept participant Roles; Pack reprojects the exact Core participant set immediately before manufacture; Transport no longer trusts persisted semantic manufacture receipts after restart; and participant confirmation was extracted into a focused VS Code-owned controller. The required true VS Code Extension Host acceptance did not execute in this environment, so the implementation must return blocked rather than candidate-for-Sigma.

## Provenance

- Known Source: Tiinex-qualified carried Extension VS Code, Core, Docs, and Business workspaces from the selected Anchor-to-Kodax implementation Handoff.
- Preservation Basis: exact carried workspace archive identities were qualified before use; Core and Docs remained read-only; only the qualified Extension VS Code workspace and Business continuation were mutated.
- Provenance Limits: npm dependencies and a VS Code CLI/Extension Host runner were unavailable in the execution environment.

- Baseline Extension VS Code archive SHA-256: `df886043c5183c4e6d015c7d22a6dddf34c9449fb8fac5ae61873b0abebe4024`.
- Qualified Core source used read-only for Local-mode attempts: `/mnt/data/kodax-deps/core` from the received carrier.
- No Core or Docs source files were modified.

## Evidence Material

- Material: Exact modified Extension VS Code source plus bounded implementation/test evidence and acceptance blocker receipts described below.
- Material Kind: bounded source implementation, dependency-free syntax/behavior checks, partial direct test execution, and explicit machine-acceptance blocker receipts.

### Implemented host-boundary repairs

- Removed `tiinex.outgoing.removeParticipantPointer` from activation registration, contributed commands, activation events, menus, and command palette exposure.
- Removed `removeOutgoingParticipantPointer` and all participant-array subset splicing from `src/operatorTrees.ts`.
- Changed tracked attached-Handoff participants to a read-only array at the controller type boundary.
- Extracted exact participant confirmation/presentation into `src/vscode/outgoingParticipantController.ts`; this is VS Code presentation/controller behavior only and does not recreate participant semantics.
- Removed `participantRoles` from public `PackageRouteInput` and `PackageBuildInput` so callers cannot inject or weaken semantic participant authority.
- Added `projectExactRouteParticipants` in `src/packageBuilder.ts`; every routed Pack re-runs Core participant projection immediately before manufacture and feeds only that fresh exact set into the internal Core manufacture arguments.
- Kept endpoint-role bindings as explicit Handoff authoring selections; no new endpoint/participant inference was introduced.

### Restart and Transport repair

- Removed persisted `tiinex.transport.receipts.v1` semantic manufacture receipts and the SHA-only fast path that could bypass Core after restart.
- `restoreTransportQueue` now restores only package path/route-selection bookkeeping and calls `qualifyTransportPackage` for every item.
- `queueBuiltTransportPackage` also reopens freshly manufactured bytes through Core before Transport accepts them.
- Transport route identities and exact transport text therefore come from current Core orientation/projection on each qualification rather than serialized semantic host state.
- Incoming and Outgoing composition remain intentionally ephemeral host session state; no serialized semantic state was added.

### Bounded controller decomposition

- Carried baseline `src/operatorTrees.ts`: 4628 lines.
- Modified `src/operatorTrees.ts`: 4575 lines at the first bounded-extraction check; the extracted participant controller is 50 lines.
- The change removes one semantic mutation surface and moves only participant confirmation/presentation out of the monolith. No broad controller rewrite or `landing.ts` deletion was performed.
- `src/landing.ts` remains deliberately untouched because the prior audit established it as legacy/suspect but not runtime-reachable; compatibility routing already enters the native operator tree.

### Added acceptance harness

- Added `scripts/test-extension-host.mjs` and `test/extension-host/suite.cjs`.
- The harness requires a real `code`, `code-insiders`, `codium`, or explicit VS Code CLI; it runs Local and Published Core modes and requires at least two Extension Host launches per mode so restart activation is exercised.
- The real host suite activates `tiinex.tiinex-vscode`, verifies public controller commands, verifies `tiinex.outgoing.removeParticipantPointer` is absent, verifies the requested dependency mode, and executes non-interactive Discovery/Incoming/Transport refresh command paths.
- This harness is intentionally fail-closed; absence of a real VS Code CLI is an acceptance blocker rather than a skipped PASS.

### Dependency-free and direct behavioral receipts

- Dependency-free TypeScript transpile: all 51 `src/**/*.ts` files parsed with zero syntax diagnostics.
- Dependency-free boundary assertions passed for command removal, no participant splice, no public participant input, Pack re-projection, no persisted semantic transport receipt, and restart requalification.
- Behavioral participant-controller checks passed: exact full Core set accepted; partial subset rejected with warning; blocked Core projection rejected with surfaced Core error.
- Direct `node test/run.mjs` against emitted JavaScript reached 55 passing tests before missing installed `@tiinex/core` stopped the suite; both the activation registration test and the new exact-participant controller test passed before that environment stop.
- A bounded direct Local-source binding attempt using the carried Core source reached 67 passing tests. It then stopped on a test whose expected default binding path is `node_modules/@tiinex/core`, while explicit Local mode correctly resolved `/mnt/data/kodax-deps/core`; this was a harness-mode expectation mismatch, not treated as product acceptance.

### Required acceptance blockers

- `npm run typecheck`: blocked because type definition packages `node` and `vscode` are unavailable in the source-only environment.
- `npm test`: build phase blocked for the same missing type definitions; emitted JavaScript was separately exercised as described above, but the npm test command is not green.
- `npm run test:local-core -- --core /mnt/data/kodax-deps/core` with npm offline: blocked by `ENOTCACHED` for `undici-types-6.20.0`; no registry/network fallback was available.
- `npm run test:extension-host -- --mode local --local-core /mnt/data/kodax-deps/core`: blocked with `tiinex.extension-host.vscode-cli-unavailable`.
- `npm run test:extension-host -- --mode published`: blocked with `tiinex.extension-host.vscode-cli-unavailable`.
- Therefore the required real Extension Host scenarios for Incoming/Replace, Outgoing, Attach, participant handling, two-Handoff Pack, Transport, restart/requalification, and negative fail-fast under both Local and Published Core are not proven here.

## Preservation And Fidelity

- Preservation State: Core and Docs carried source remained read-only. The outer received Handoff carrier was not rewritten. Extension VS Code changes are bounded to the host implementation/test surfaces described above.
- Fidelity Notes: environment failures are recorded as blockers, not product failures and not PASSes. Partial Node test progress is reported only as partial evidence.
- Known Losses: no real VS Code Extension Host execution receipt, no clean npm typecheck/test receipt, and no Published Core host run are available in this environment.

## Interpretation Limits

- Not Yet Used As: Sigma acceptance, release approval, publication approval, or proof of complete real Extension Host operator-flow acceptance.
- Does Not Prove: full operator-flow acceptance, Published Core compatibility in a real Extension Host, Sigma readiness, release readiness, or remote publication readiness.
- Must Not Be Treated As: a substitute for the required machine acceptance gate.
- Disposition: blocked pending execution of the real Extension Host gate and clean dependency-backed validation in a capable environment; do not hand to Sigma yet.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-anchor-to-kodax-vs-code-core-boundary-recovery-and-extension-hos.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-anchor-to-kodax-vs-code-core-boundary-recovery-and-extension-hos.trace.md)
  - Value: P5p1W4t_BI6qo69J7DsKd_GkOe251jMwyWjqp0DuOK0

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: z_1IDCbDcWWLDGcedI4Rh1kAFtxeIFlEDWxe7G71jPA