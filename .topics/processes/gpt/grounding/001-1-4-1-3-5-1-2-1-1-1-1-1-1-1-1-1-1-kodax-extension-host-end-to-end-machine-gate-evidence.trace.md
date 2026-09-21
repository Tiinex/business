# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 16:24:46
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-anchor-to-kodax-extension-host-end-to-end-acceptance-completion.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-anchor-to-kodax-extension-host-end-to-end-acceptance-completion.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-anchor-to-kodax-extension-host-end-to-end-acceptance-completion.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 17:15:14
  - Authors: Kodax
  - Why: Return exact machine-gate evidence without promoting unexecuted host acceptance.
  - Summary: Repository-owned full-flow host gate completed; real Local/Published execution remains blocked by missing VS Code CLI and dependency tree.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: Does the current Extension VS Code candidate now contain a repository-owned real VS Code Extension Host gate broad enough to prove the required Local/Published operator flow, and did this machine execute that gate successfully?
- Evidence Role: Kodax machine-gate completion evidence and blocked acceptance disposition for Anchor.
- Supported Conclusion: the previously shallow host suite was replaced with a deterministic repository-owned Extension Host acceptance gate that drives the registered production command/controller path across Incoming, Replace, Outgoing, two Handoff attachments, exact participant confirmation, Pack, Transport, restart requalification, and the required negative cases. The static fixture independently qualifies to the exact Core participant set `Pilot + Sigma`, and dependency-free source checks are clean. This machine cannot execute the real host gate because no VS Code CLI/runtime is available; dependency-backed typecheck is also blocked by absent declared type packages, and the exact Published Core dependency is not installed. Therefore the tranche is blocked and is not candidate-for-anchor-reconciliation or Sigma.

## Provenance

- Known Source: Tiinex-qualified Anchor-to-Kodax carrier selected through `001-3-1-1-1-handoff-pointer.trace.md`, with exact carried Business, Extension VS Code, Core, and Docs workspace identities qualified before use.
- Preservation Basis: the exact carried Extension VS Code workspace was the writable candidate; the exact carried accepted Core workspace was used read-only for Local-mode fixture qualification; Core and Docs source were not mutated; the outer carrier was not rewritten or package-wide extracted.
- Baseline Extension VS Code workspace archive SHA-256: `769c0ac2d6a321de5c34f5cdbac2d2e30b76e10890b21046809afdfd469c61e0`.
- Accepted Core workspace archive SHA-256: `2ff12a1af5b9254604f8ccedd5c742f9db84ef9c75ed5f47bbd8f4c856a1b8c7`.
- Received carrier SHA-256: `b6fec7b674239bb6aed3e2bb3952d2706e22da987ef82d0690f6c89a0b6f725d`.
- Provenance Limits: the environment has Node/npm but no real VS Code CLI/runtime and no installed lock-qualified npm dependency tree, so real Extension Host execution and dependency-backed regression cannot be claimed.

## Evidence Material

- Material: Exact modified Extension VS Code workspace, full registered-command Extension Host acceptance harness, deterministic pointerless two-Handoff fixture, Core fixture-qualification receipts, dependency-free source checks, and exact environment blocker receipts.
- Material Kind: bounded acceptance-harness implementation plus machine-validation evidence.

### Repository-owned real Extension Host gate

- `scripts/test-extension-host.mjs` now resolves a real `code`, `code-insiders`, `codium`, or explicitly supplied VS Code CLI and fails closed when none exists.
- The runner builds before host launch when a CLI exists, verifies the static fixture bytes, stages a disposable Git-backed workspace, and executes both Local and Published Core modes with at least two launches per mode so restart behavior is exercised.
- Local mode requires the exact carried Core package source and its portable Tooling entrypoint.
- Published mode requires the package-lock-qualified `@tiinex/core` dependency and verifies the installed dependency version; it has no Local fallback.
- The Extension Host suite activates the real extension and then uses registered extension commands and the production controller path; it does not substitute direct Core manufacture or participant helper calls for host acceptance.

### Full-flow acceptance coverage now encoded

- Pointerless Incoming carriage through normal Discovery/Incoming commands.
- Pointerless Transport negative case: zero synthetic Handoff routes and no fabricated `Continue from` text.
- Replace/landing through normal `tiinex.incoming.replace`, with source bytes asserted at the destination.
- Outgoing creation through normal `tiinex.outgoing.new` using deterministic VS Code-owned presentation selections only.
- Invalid Handoff negative case through normal `tiinex.outgoing.attachHandoff`, asserted rejected before Pack.
- Participant weakening negative case through the same production participant-confirmation controller: a deliberately weakened selection is rejected by the real exact-set comparison.
- Two independently qualified valid Handoff attachments through normal `tiinex.outgoing.attachHandoff`.
- Deliberate acceptance-only corruption of host participant bookkeeping before normal Pack; Pack must still emit two fresh Core participant requalification progress events, proving stale host participant arrays are not semantic authority.
- Normal `tiinex.outgoing.package` followed by Transport qualification of the produced carrier, with exact two-route paths/text asserted.
- Second real host launch asserts persisted Transport bookkeeping causes the package bytes to be requalified through Core on restore; a subsequent normal Transport refresh is also asserted as a fresh Core qualification.
- The removed `tiinex.outgoing.removeParticipantPointer` command is asserted absent.

### Deterministic fixture and legitimate host seams

- Added `test/extension-host/fixtures/incoming-pointerless.handoff-package.zip` with SHA-256 `d98488f6a2fa37834a4954b3b84a38f17f348f535b2e08a1bdb0e91b9d460401` plus a checked manifest and exact source workspace.
- The fixture contains two valid Handoff routes. Independent qualification with the accepted Core projects each route to exactly `Pilot, Sigma` with zero findings.
- Acceptance-only environment-gated seams exist at VS Code-owned presentation/observation boundaries: deterministic QuickPick/folder choices, non-blocking acceptance notifications, read-only controller snapshots, and deliberate corruption of mutable host bookkeeping for the stale-state negative test.
- Those seams do not import Core, manufacture Handoff packages, project semantic participants, or replace the production exact-set guard. Normal extension behavior is unchanged when `TIINEX_EXTENSION_HOST_ACCEPTANCE` is not enabled.

### Exact Extension VS Code source delta

- Modified `scripts/test-extension-host.mjs`.
- Modified `test/extension-host/suite.cjs`.
- Added `test/extension-host/fixtures/**`.
- Added `src/vscode/extensionHostAcceptance.ts`.
- Modified `src/vscode/outgoingParticipantController.ts` only for environment-gated deterministic selection/observation around the existing exact-set guard.
- Modified `src/operatorTrees.ts` only for environment-gated acceptance commands/observations and deterministic presentation choices required by the real host suite.
- Modified `src/packageBuilder.ts` only to make the acceptance-mode build announcement non-blocking/observable.
- No Core or Docs source file was modified and no general controller refactor, release, publication, commit, push, or deployment occurred.

### Validation receipts available on this machine

- JavaScript syntax checks for the Extension Host runner and suite: passed.
- Dependency-free TypeScript transpile/syntax pass: all 52 TypeScript source files transpile with zero syntax diagnostics.
- Static source invariants: 12 required invariants passed, including no registered participant-weakening command, fresh Pack participant projection, Transport qualification on queue/restore, no Core semantic helpers in the acceptance seam, and presence of the required full-flow suite actions.
- Static fixture qualification with exact accepted Core: both Handoff routes are qualified, project exactly `Pilot, Sigma`, and have zero Core findings.
- Final fixture carrier SHA-256 reproduction: `d98488f6a2fa37834a4954b3b84a38f17f348f535b2e08a1bdb0e91b9d460401`.
- Package lock Published Core requirement: `@tiinex/core@0.35.0`.

### Exact unresolved machine gates

- First canonical real-host blocker: `node scripts/test-extension-host.mjs --mode both --local-core <accepted-core-root>` exits non-zero with `tiinex.extension-host.vscode-cli-unavailable` before host execution because this environment has no `code`, `code-insiders`, or `codium` CLI/runtime.
- Dependency-backed typecheck: `npm run typecheck` exits non-zero with TypeScript `TS2688` because type definition libraries `node` and `vscode` are not installed in this source-only environment.
- Published Core: package-lock requires `@tiinex/core@0.35.0`, but no installed `node_modules/@tiinex/core` is available here; npm/network cache cannot provide the dependency tree in this machine context.
- Because the real VS Code host never launched, no Local-mode real-host receipt, Published-mode real-host receipt, restart-host receipt, or clean dependency-backed regression receipt exists.

## Preservation And Fidelity

- Preservation State: the accepted host semantic repair remains intact. This tranche adds/corrects the acceptance harness and only environment-gated VS Code-owned presentation/observation seams necessary to drive it deterministically.
- Fidelity Notes: fixture qualification, source/transpile checks, and encoded suite coverage are evidence that the gate is runnable and semantically bounded; they are not substituted for real VS Code Extension Host execution.
- Known Losses: no real Extension Host process receipt, no clean dependency-backed `npm run typecheck`, no full dependency-backed package regression, and no installed Published Core host execution on this machine.

## Residual Risks And Next Machine Action

- Residual Risk: the full-flow gate is materially broader than the prior suite but remains unexecuted in a real Extension Host, so host lifecycle, VS Code API behavior, and Published Core integration remain empirically unproven.
- Required Next Environment: a machine with a real compatible VS Code CLI/runtime plus the exact lock-qualified npm dependency tree, including `@tiinex/core@0.35.0` and declared Node/VS Code type packages.
- Required Next Action: from the exact returned Extension VS Code workspace, install/restore the lock-qualified dependency tree; run clean dependency-backed typecheck/test/package regressions; then run `npm run test:extension-host -- --mode both --local-core <exact-carried-accepted-core-root>` and preserve all Local, Published, and restart receipts. Any genuine bounded host defect exposed by that run may be corrected within the existing Task boundary; shared/Core semantic gaps return to Anchor.

## Interpretation Limits

- Not Yet Used As: candidate-for-anchor-reconciliation, Sigma delegation, Sigma acceptance, release approval, publication approval, deployment approval, or proof of complete real Extension Host acceptance.
- Does Not Prove: that the Local or Published full operator sequence actually passed inside VS Code, that restart behavior passed inside a real host, or that the dependency-backed build/regression suite is green.
- Must Not Be Treated As: a synthetic PASS produced from source assertions, fixture qualification, mocks, direct Core invocation, or dependency-free transpilation.
- Disposition: blocked at the first exact unresolved real-host machine gate `tiinex.extension-host.vscode-cli-unavailable`; return to Anchor with the exact runnable gate and candidate source, not to Sigma.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-anchor-to-kodax-extension-host-end-to-end-acceptance-completion.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-anchor-to-kodax-extension-host-end-to-end-acceptance-completion.trace.md)
  - Value: NDXxB15RbQCCqk7HYE2a1w0gsXjB96hUV57-HhvtawA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: -7Mb-R6wPMwxo4ULiu0gMpcEf6prnMvaxdiUV1GMf7E