# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 19:53:47
  - Trace: [005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md](005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md)
  - Origin:
    - [relative](005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 19:54:25
  - Authors: Anchor
  - Why: The accepted source implementation is deterministically green once runtime matches source, but the carried Workspace is not real-host safe until its emitted runtime is complete and current.
  - Summary: Correct exactly two durable VS Code emitted-runtime parity defects without reopening accepted Major 008 source semantics or Package V1.
  - Status: ready/local

---

# Tooling Major 008 — VS Code Emitted Runtime Parity Correction

## Objective

Correct the exact durable VS Code emitted-runtime inconsistency discovered by Anchor after the final Major 008 Kodax source convergence return, without changing accepted Handoff semantics, Package V1, Core source, Role discovery rules, participant selection semantics, cache/material closure, or the accepted VS Code source implementation unless the canonical repository build proves an additional exact source defect.

The accepted source frontier is provisionally functionally green under Anchor's disposable source-consistent runtime probe. The current durable Workspace is not yet safe for real-host acceptance because two emitted runtime outputs do not match that source frontier.

## Done Criteria

- Regenerate and durably preserve emitted runtime from the exact accepted VS Code source frontier using the repository-owned build path.
- `dist/core/handoffEndpointSelection.js` exists and corresponds exactly to `src/core/handoffEndpointSelection.ts`; include its normal source map if the repository build produces one.
- `dist/core/workspaceChoice.js` corresponds exactly to the current accepted `src/core/workspaceChoice.ts` behavior that selects one direct canonical `.topics/.workspaces/*.workspace.md` artifact and excludes recursively discovered nested fixture/test Workspaces.
- No other `src/**/*.ts` semantic source file changes unless the canonical repository build itself exposes a new exact source defect that cannot be corrected as emitted-output parity; if that occurs, stop and return the blocker instead of broadening scope.
- Core Workspace remains byte-identical to the accepted Major 008 Core frontier.
- Business changes are limited to qualified Kodax Evidence/return artifacts needed for this correction.
- Source-to-emitted-JS parity audit over the complete VS Code TypeScript source surface has:
  - 0 missing expected JS outputs;
  - 0 stale JS outputs relative to the exact accepted source frontier, allowing ordinary source-map metadata normalization only.
- `node test/run.mjs` passes all 117 cases against the exact accepted Core frontier.
- `node test/package-integration.mjs` passes all 4 scenarios.
- The specific Workspace-root regression proves an explicitly renamed checkout root exposes only the direct canonical `vscode` Workspace and does not surface `001-3-acceptance` or `extension-host-acceptance`.
- The exact current `dist/packageBuilder.js` can resolve `./core/handoffEndpointSelection` from the durable Workspace without disposable generation.
- No `.json` recipient/meta sidecar, Package V1 representation change, pointer-lineage change, host-private semantic authority, recursive repository Role discovery, or Core-owned behavior duplication is introduced.
- Return one qualified Kodax-to-Anchor Handoff carrying the exact corrected VS Code Workspace and unchanged accepted Core Workspace.

## Scope

- Kodax / VS Code repository emitted build outputs and matching deterministic regression evidence only.
- Repository-owned build consistency between current `src` and current `dist`.
- Exact current Major 008 source frontier only.

## Dependencies

- [Tooling Major 008](001-2-8-tooling-major-008-native-handoff-authoring-and-durable-pointer-c.trace.md)
- [Anchor Emitted Runtime Parity Blocker Evidence](005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md)
- Exact accepted Core Workspace carried with the Anchor correction Handoff.
- Exact current VS Code source frontier returned by Kodax before this correction.

## Exclusions

- Do not redesign Package V1.
- Do not modify Core source.
- Do not reintroduce artifact-first/recipient-v2 normal package representation.
- Do not add recipient/meta JSON or cache index manifests.
- Do not change endpoint/participant semantics merely to satisfy build parity.
- Do not perform remote commit, push, release, publication, deployment, or registry mutation.
- Do not claim real VS Code Extension Host or Sigma acceptance from deterministic Node/package tests.

## Completion Boundary

Completion of this Task means the exact accepted Major 008 source implementation is durably build-consistent and ready for Anchor's final deterministic fan-in and subsequent real-host gate. It does not itself close Major 008 or replace Sigma acceptance.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md](005-tooling-major-008-anchor-emitted-runtime-parity-blocker-evidence.trace.md)
  - Value: evXhAOARyujwxq1x2x5rIoFxpFtz9maueE54vP6HSDA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 7SQfn4iWGkM48eceRMLm2SCwgWTTN4DTIS879JQrKfw