# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 08:49:33
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-1-major-002-final-vs-code-regression-identity-alignment.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-1-major-002-final-vs-code-regression-identity-alignment.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-1-major-002-final-vs-code-regression-identity-alignment.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 09:29:45
  - Authors: Kodax
  - Why: Preserve the exact Kodax-owned correction and execution receipts for Anchor fan-in.
  - Summary: Durable stale VS Code Workspace identity regression correction passes 116/116 bridge and 4/4 package-integration scenarios with no product-source change.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: Was the remaining Major 002 VS Code failure only stale repository-owned Workspace identity regression debt, and does the durable correction pass the exact broad bridge and package-integration scenarios without changing product source?
- Evidence Role: Kodax implementation and regression evidence for Anchor fan-in.
- Supported Conclusion: Yes. The durable correction is limited to `test/run.mjs` and `test/package-integration.mjs`; all 53 `src/**/*.ts` product files remain byte-identical to the qualified received VS Code Workspace. The corrected repository-owned regressions pass 116/116 bridge cases and 4/4 package-integration scenarios against the exact carried Loom Core code in an offline disposable installed-binding harness. No new product defect was exposed.

## Provenance

- Known Source: Tiinex-qualified Anchor-to-Kodax route from `business-001-2-3-anchor-to-kodax.handoff-package.zip`, selected by `001-3-1-1-1-handoff-pointer.trace.md`.
- Preservation Basis: the exact carried VS Code Workspace archive was read from qualified package path `001-5-vscode.workspace.zip`; the exact carried Core Workspace archive was read from qualified package path `001-4-core.workspace.zip`; both were materialized only after grounding reported `grounded-to-act`.
- Mutation Boundary: only the qualified VS Code Workspace test surface and Business continuation were mutated. Core remained read-only. Product `src/**` bytes were not changed.
- Provenance Limits: the offline broad test harness copied the exact Core code into disposable `node_modules/@tiinex/core` and changed only that disposable Core copy's package `version` metadata to `0.35.0` so the existing installed-binding branch could execute against the extension lockfile. This is not Published Core acceptance and no durable Core byte was changed.

## Evidence Material

- Material: exact two-file VS Code regression delta, exact Core/VS Code carried source bytes, broad Node regression receipts, package-integration receipt, and byte-comparison receipts.
- Material Kind: repository-owned test/fixture identity correction plus bounded offline execution evidence.

### Durable regression correction

- `test/run.mjs` changes the installed-Core operator-context integration expectation from `[extension-vscode, vscode]` to exactly `[vscode]`, matching the directly qualified `.topics/.workspaces/tiinex-vscode.workspace.md` artifact and continuing to rely on Core for nested-surface exclusion.
- `test/package-integration.mjs` now copies only `tiinex-vscode.workspace.md`, uses fixture repository `https://github.com/Tiinex/vscode.git`, selects Workspace id `vscode`, and expects orientation id `vscode`.
- No production controller, host, package, schema, carrier, Workspace artifact, or Core behavior was changed.

### Exact delta receipts

- Original `src/**/*.ts` tree fingerprint: `5bc543e87eed030a206d82526754327fadd7e27703b3a8e71d891c39c197a556` across 53 TypeScript files.
- Final `src/**/*.ts` tree fingerprint: `5bc543e87eed030a206d82526754327fadd7e27703b3a8e71d891c39c197a556` across the same 53 files.
- Original `test/run.mjs` SHA-256: `eb59f913649d3efdc261d942e559e7d971d7308e2f57207a66ecf3a1c8b6fd5d`.
- Final `test/run.mjs` SHA-256: `1a8fe9f5f2224ef9426a8d8e28136a56444c92d0fc9c83ccfd5281f4da5e5762`.
- Original `test/package-integration.mjs` SHA-256: `b7697374b598c933d967e3ae24d8baee6632e83ea1426793d178e6907204d5ec`.
- Final `test/package-integration.mjs` SHA-256: `26eedefb35edb49ba1c1abd1413c86a843c32dcc11725e860bf6073414c52aba`.
- Full Workspace byte comparison against the qualified received VS Code archive reports exactly 2 changed files, 0 added files, and 0 deleted files.

### Execution receipts

- Disposable offline installed-binding run: `node test/run.mjs` completed `116/116 Tiinex VS Code bridge core cases passed`.
- Disposable offline installed-binding run: `node test/package-integration.mjs` completed `4/4 package integration scenarios passed. Windows/VS Code UI acceptance remains separate.`
- The package-integration scenarios include real extension package-builder output, re-orientation to exact Workspace selection with no invented Handoff/lineage, idempotent exact retry versus divergent overwrite rejection, and extracted VSIX execution of its bundled public Core entrypoint.
- The durable source itself did not receive `node_modules`, dependency-mode state, Core metadata changes, or any generated fixture from the disposable probe.

## Preservation And Fidelity

- Preservation State: Core source, VS Code product source, qualified Workspace artifact identity, fixtures outside the targeted stale expectations, and the received outer carrier are preserved. No remote mutation, commit, push, publication, release, deployment, or Sigma promotion occurred.
- Fidelity Notes: the disposable Core metadata edit exists only to traverse the extension's installed-binding lock check offline; it is reported at exactly that strength and is not used as registry/Published acceptance evidence.
- Known Losses: no real VS Code Extension Host replay and no registry-published Core verification were performed in this correction; those remain downstream acceptance concerns, not blockers for the repository-owned stale test correction itself.

## Interpretation Limits

- Not Yet Used As: Sigma acceptance, release approval, Published Core acceptance, or real Extension Host acceptance.
- Does Not Prove: that any later real-host environment is free of unrelated machine-specific defects.
- Must Not Be Treated As: authority to change Core semantics, rewrite Workspace identity, delete fixtures to hide discovery behavior, or broaden this correction into product refactoring.
- Disposition: durable Kodax test/fixture identity correction is complete and ready for Anchor fan-in; no new exact product defect was exposed by the corrected regressions.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-1-major-002-final-vs-code-regression-identity-alignment.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-1-major-002-final-vs-code-regression-identity-alignment.trace.md)
  - Value: RpM6w3Lb5KvHr2L0JXm8t8AXGGqgGP5GgQUDbcxcG2Q

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 2XsEdxhYSRk_5McszZqEOIkA2DhKeLH57stjgoOaGmQ