# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 08:49:02
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-major-002-anchor-fan-in-stale-vs-code-test-identity-evidence.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-major-002-anchor-fan-in-stale-vs-code-test-identity-evidence.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-major-002-anchor-fan-in-stale-vs-code-test-identity-evidence.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 08:49:33
  - Authors: Anchor
  - Why: Anchor fan-in isolated the only remaining integrated failure to stale Kodax-owned test identity debt.
  - Summary: Align stale VS Code regression expectations and package fixtures to the current qualified vscode Workspace identity without changing product semantics.
  - Status: ready/local

---

# Major 002 — Final VS Code Regression Identity Alignment

## Objective

Land the bounded repository-owned VS Code regression correction that aligns tests/fixtures with the currently qualified `vscode` Workspace artifact and repository identity, without changing product behavior or reopening shared Core semantics.

## Scope

- Update the operator-context integration expectation so the current extension root projects exactly the directly qualified `vscode` Workspace and does not preserve the superseded `extension-vscode` identity.
- Update package-integration fixture setup to use only the current `.topics/.workspaces/tiinex-vscode.workspace.md` artifact, Workspace id `vscode`, and the repository identity carried by that artifact.
- Preserve all Kodax product/controller/source bytes from the accepted sibling return unless the corrected repository-owned tests expose a new exact product failure.
- Re-run the broad bridge and package-integration suites against the exact returned Loom Core candidate.

## Done Criteria

- No test or fixture in the corrected paths references removed `tiinex-extension-vscode.workspace.md` as a current Workspace artifact.
- The operator-context integration test expects the current direct Workspace projection and still rejects nested acceptance/test Workspace leakage.
- Package integration constructs a source fixture consistent with the carried `tiinex-vscode.workspace.md` repository identity and qualifies the exact selected Workspace.
- `node test/run.mjs` passes all 116 bridge cases against the exact Loom Core candidate under a truthful Local/available runtime binding; any Published-only environment limitation remains explicit rather than mocked in durable evidence.
- `node test/package-integration.mjs` passes all 4 scenarios.
- No product-source file changes unless one of those corrected tests exposes a new reproducible product defect; any such defect must be returned to Anchor rather than broadened opportunistically.
- Return exact VS Code delta and qualified Evidence/Handoff to Anchor with no remote mutation.

## Dependencies

- Anchor fan-in stale VS Code test identity Evidence.
- Exact Loom Core returned Workspace from the sibling specialist branch.
- Exact Kodax VS Code returned Workspace from the sibling specialist branch.
- Existing Major 002 post-Sigma recovery Task remains the controlling program scope.

## Ownership Boundaries

- Kodax owns VS Code repository tests/fixtures and any bounded host correction proven necessary by those tests.
- Loom/Core is read-only for this correction; no Core mutation is authorized.
- Docs semantics are unchanged.
- Anchor retains fan-in, integrated acceptance and Sigma sequencing.

## Exclusions

- No Workspace identity rewrite merely to satisfy stale tests.
- No fixture deletion/move as a substitute for production discovery correctness.
- No product refactor, schema change, package-format change, remote commit/push/release/deploy, or Sigma promotion from specialist-local results alone.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-major-002-anchor-fan-in-stale-vs-code-test-identity-evidence.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-6-1-2-1-1-1-1-1-1-3-major-002-anchor-fan-in-stale-vs-code-test-identity-evidence.trace.md)
  - Value: 0V1im6FCnYB0TrRFeDNPfpBiEXIPDdGt6mrQmuHwvbU

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: RpM6w3Lb5KvHr2L0JXm8t8AXGGqgGP5GgQUDbcxcG2Q