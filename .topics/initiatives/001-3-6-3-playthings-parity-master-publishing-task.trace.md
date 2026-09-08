# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-08 17:38:00
  - Trace: [001-3-6-core-app-site-extraction-task.trace.md](001-3-6-core-app-site-extraction-task.trace.md)
  - Origin:
    - [relative](001-3-6-core-app-site-extraction-task.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-08 20:41:55
  - Authors: Anchor
  - Why: Continue the supplied current source with explicit compatibility, release and qualification boundaries.
  - Summary: Playthings public adapter and master-only npm publishing
  - Status: active/local

---

# Playthings public adapter and master-only npm publishing

## Objective

Close the concrete App/Playthings public-entrypoint gap and establish one shared, tested master-only version/publication mechanism. Preserve the six current source Workspaces and prepare a bounded Playthings successor handoff without making source transport equivalent to production acceptance.

## Done Criteria

- App reads the supplied corrected App source; Site lazy-loads the actual Playthings React adapter through public npm exports.
- Existing headless Playthings semantics remain intact; the minimal history view does not pretend to be the planned complete world renderer.
- Core owns one Node release helper consumed by App and Playthings; only master can publish after tests and explicit npm/OIDC setup.
- Automatic patch/minor/major selection, registry error handling, exact-source staging, retries and tampering controls have executable tests.
- Pinned browser build/render and live npm/GitHub publication are separately qualified before declaring rollout ready. Local network absence is a blocker, not a pass.
- Complete source, current claims, limitations and explicit next steps are transported to Sigma and the successor Playthings Anchor.

## Scope

Current source is the user-replaced Workspace payloads in tiinex-all-002, not its stale outer metadata. No GitHub connector, remote writes, npm publish, VS Code implementation or other role delegation was performed. This is under the Viewer extraction task with Tooling/Core context. Business delivery mechanics move to a verified detached supplement; historical bytes remain preserved. Historical lineage reduction and CLI/Interop/Chrome remain Turn 2. VS Code follows Turn 2 with the next Refactor Anchor.

## Dependencies

- [Core Initiative](001-1-core-project.trace.md) and [Tooling Initiative](001-2-tooling-project.trace.md) retain their existing ownership boundaries.
- [Playthings Initiative](001-9-playthings-project.trace.md) retains its independent productization direction.
- Current App 0.1.1, Core 0.1.1 and Playthings 0.1.0 candidate packages, their exact source and the shared release documentation.
- npm-connected dependency/browser qualification; Sigma-owned one-time account configuration.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-3-6-core-app-site-extraction-task.trace.md](001-3-6-core-app-site-extraction-task.trace.md)
  - Value: SOxxB77pxLrbHBJ3AodTGDgynI770PNNulV-Ov0MPqQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 78cJ5X-DngDlHi9HdWMLDoIZ0KkHwN2RxnQPA4rNyNA