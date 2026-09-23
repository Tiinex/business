# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 20:17:16
  - Trace: [032-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-resume.trace.md](handoffs/032-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-resume.trace.md)
  - Origin:
    - [relative](handoffs/032-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-resume.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 21:11:54
  - Authors: Kodax
  - Why: Preserve the exact bounded resume result without misclassifying host-substituted diagnostic output as canonical emitted-runtime parity.
  - Summary: The authorized HandoffLeavesResult findings type correction is complete and deterministic diagnostics are green, but canonical emitted-runtime regeneration remains blocked by unavailable exact lockfile build dependencies.
  - Status: ready/local

---

# Tooling Major 008 — Kodax Emitted Runtime Parity Resume Dependency Blocker Evidence

## Supported Claim Or Question

- Supported Claim Or Question: After the exact authorized `HandoffLeavesResult.findings` type-surface correction, can the accepted VS Code frontier be canonically rebuilt and durably restore emitted-runtime parity on this machine?
- Evidence Role: exact Kodax resume evidence separating the now-corrected internal source contract from the remaining external locked-build dependency blocker.

## Provenance

- Known Source: exact qualified `business`, `core`, and `vscode` Workspace snapshots carried by the selected Anchor-to-Kodax Handoff after Start-only cold read, verified portable Tooling bootstrap, Tiinex orientation, exact route grounding, and qualified Workspace materialization.
- VS Code Baseline Archive Identity: carried `001-5-vscode.workspace.zip`, SHA-256 `883ed4a0bfede2b86efa09c077ac96727ab43410da3f4f4f70447ada7b26e04b`.
- Core Archive Identity: carried `001-4-core.workspace.zip`, SHA-256 `50a8f620aa0f2cf657370d95302c53db97126009a373a3a4c69a5ecb1673d15e`.
- Preservation Basis: the authorized correction was applied only to the materialized VS Code source frontier; all canonical and diagnostic builds ran in disposable copies, and temporary dependency material was excluded from the durable Workspace.
- Provenance Limits: the exact lockfile TypeScript `5.7.2`, `@types/node` `22.10.2`, and `@types/vscode` `1.95.0` package bytes are not available locally and registry acquisition fails in this execution environment.

## Evidence Material

- Material Kind: bounded source-contract correction, repository-owned canonical build attempt, lockfile dependency-acquisition receipt, disposable diagnostic emitted-runtime probe, deterministic regression receipts, and exact durable byte-delta audit.
- Material: corrected `src/tiinex/bootstrap.ts`, `npm ci` / `npm run build` receipts, disposable diagnostic `dist`, 117-case bridge receipt, 4-scenario package integration receipt, and before/current Workspace byte comparison.

### Authorized source correction

The exact Decision-authorized correction was applied and nothing else in product source was changed:

- `HandoffLeavesResult` now declares `findings?: Array<{ severity: string; code: string; message: string }>;`.
- `projectHandoffLeaves` runtime behavior is unchanged.
- `src/packageBuilder.ts` is unchanged.
- Core source is unchanged.

Durable VS Code byte audit against the received qualified snapshot:

- baseline/current file count: `391` / `391`;
- changed paths: exactly `src/tiinex/bootstrap.ts`;
- added paths: none;
- removed paths: none;
- durable `node_modules`: absent.

### Canonical build dependency blocker

The repository lock binds these exact build dependencies:

- `typescript@5.7.2`;
- `@types/node@22.10.2`;
- `@types/vscode@1.95.0`;
- transitive `undici-types@6.20.0`.

`npm ci --ignore-scripts --no-audit --no-fund` cannot materialize them on this machine. The npm receipt reaches the exact registry tarball URLs and fails with `EAI_AGAIN`; no complete locked package set is installed.

A disposable repository-owned `npm run build` after the source correction therefore exits `2` at the external type-library gate:

- `TS2688: Cannot find type definition file for 'node'`;
- `TS2688: Cannot find type definition file for 'vscode'`.

The previously reported internal `TS2339` `projected.findings` / `HandoffLeavesResult` mismatch no longer appears after the authorized correction.

### Non-canonical diagnostic probe

A separate disposable diagnostic build used the repository-owned `npm run build` command but host-supplied TypeScript `5.8.3`, host `@types/node` `22.19.7`, and a host-only VS Code API type stub. This probe is diagnostic only and is not canonical parity acceptance.

The probe shows:

- build completes without a new product diagnostic;
- expected emitted JS outputs: `54`;
- missing expected JS outputs: `0`;
- relative to the received durable runtime, the diagnostic JS delta is exactly:
  - added `dist/core/handoffEndpointSelection.js`;
  - changed `dist/core/workspaceChoice.js`;
- `dist/tiinex/bootstrap.js` remains byte-identical despite the type-only source correction;
- `dist/packageBuilder.js` remains byte-identical.

Against exact carried Core source in a disposable installed-binding harness (only probe package-version metadata adjusted to the extension lock branch), deterministic execution is green:

- `node test/run.mjs`: `117/117 Tiinex VS Code bridge core cases passed`;
- `node test/package-integration.mjs`: `4/4 package integration scenarios passed`.

These receipts show the bounded source correction is internally coherent and that the known runtime target remains exactly the original two parity outputs. They do not authorize copying the diagnostic `dist` into the durable Workspace.

## Preservation And Fidelity

- Preservation State: durable VS Code retains only the authorized one-file source correction; durable emitted runtime remains the received bytes and therefore still has the known missing/stale two-file parity defect. Core remains unchanged.
- Fidelity Notes: all generated diagnostic runtime stayed in a disposable probe. No diagnostic compiler/type substitution is promoted as canonical repository build output.
- Known Losses: canonical emitted-runtime regeneration, canonical full parity acceptance, and downstream real Extension Host acceptance remain unavailable until the exact locked build dependencies can be materialized on a capable machine.

## Interpretation Limits

- Does Not Prove: canonical emitted-runtime parity, registry-backed Published-Core acceptance, real VS Code Extension Host acceptance, Sigma acceptance, or Major 008 completion.
- Must Not Be Treated As: authority to hand-author `dist`, copy diagnostic generated runtime into the durable Workspace, relax the lockfile toolchain, modify Core, or broaden Package V1 / endpoint / participant / cache / pointer semantics.
- Not Yet Used As: parity PASS, real-host PASS, or Sigma promotion.

## Review Notes

The internal source-contract blocker is resolved exactly as Anchor authorized. The next bounded blocker is environmental: a capable build machine must provide the exact lockfile build dependencies, rerun the repository-owned build, land canonical emitted runtime, verify zero missing/stale outputs, and rerun the deterministic gates before Anchor proceeds to real-host acceptance.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [032-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-resume.trace.md](handoffs/032-anchor-to-kodax-tooling-major-008-emitted-runtime-parity-resume.trace.md)
  - Value: O2aBPnKKEJtMajT2h1A5sL9RzIh8FVWSQMERetEmN_s

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: v1GJvZmogHALyg33U4nWKlbNe4wqeUH8XIK-hGuJf6s