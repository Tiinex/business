# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.decision.v1
  - Created At: 2026-09-21 15:27:28
  - Trace: [001-1-4-1-3-5-1-2-1-anchor-core-tranche-acceptance.trace.md](001-1-4-1-3-5-1-2-1-anchor-core-tranche-acceptance.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-anchor-core-tranche-acceptance.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 15:29:46
  - Authors: Anchor
  - Why: Core is accepted; the remaining implementation-ready risk is the host/controller boundary that previously produced participant, packing, transport, restart, and late-failure regressions.
  - Summary: Repair the remaining VS Code host drift against the accepted Core frontier and prove the real operator path in Extension Host before Sigma.
  - Status: ready/local

---

# VS Code Core-Boundary Recovery And Extension Host Acceptance

## Objective

Complete the architecture-recovery host tranche against the exact Anchor-accepted Core frontier: remove Extension VS Code semantic-owner drift, make the Incoming/Replace/Outgoing/Attach/participant/Pack/Transport path use one Core-owned truth path, reduce the current operator-controller hotspot only where host responsibilities can be separated without semantic duplication, and establish real Extension Host machine acceptance before Sigma is asked to test again.

## Done Criteria

- The extension consumes the exact accepted Local Core source for Local mode and preserves the lock-qualified Published Core binding for Published mode; mode/restart behavior must not silently substitute one for the other.
- After Attach, the host cannot weaken, splice, or retain a partial locally edited semantic participant set. Any participant presentation or operator choice must come from an exact current Core projection, and Pack must use the exact qualified set or explicitly re-run Core qualification before replacing it.
- Participant presentation is actually visible in the relevant VS Code operator flow when Core projects participant authority; absence is explicit when Core projects none/unresolved. Role inventory, endpoint labels, cache contents, speaker state, and host-local defaults never manufacture participants.
- Incoming, Merge/Replace, Outgoing, Attach, and Pack all surface known Core qualification/material/route blockers at the earliest owning operation rather than deferring a known Attach/Input defect into a later Pack failure.
- Pointerless packages never receive synthetic Handoff `Continue from` text. The host renders only the exact Core-projected transport output appropriate to the qualified package/route state and never reconstructs semantic routing text itself.
- Packing uses Core-owned carrier allocation, route qualification, participant projection, material closure, manufacture/preflight, and transport projection. Extension-local helpers may adapt receipts/view models but must not contain a second copy of these rules.
- The `operatorTrees.ts` hotspot is reduced only through bounded host-controller extraction where responsibilities are genuinely VS Code-owned (TreeView/commands/dialog/progress/session/filesystem/Git presentation/execution). Do not perform a broad rewrite merely to reduce file size.
- Legacy/suspect receive/landing paths are reconciled deliberately: either prove they remain live and bring them through the same Core boundary, or preserve them as explicit legacy/deferred surface with tests preventing them from silently becoming a second semantic path. Do not delete compatibility code without evidence.
- Restart/reload persists only host-local identifiers/choices needed for resumability. Any semantic package/Handoff/participant/manufacture state used after restart is reopened and requalified through Core before mutation or Pack; persisted receipts are not authority merely because they survived workspace state.
- Add machine coverage that exercises the real extension controller/command path, not only source-text/regex/unit helpers. The acceptance path must cover Incoming/Replace, Outgoing, Attach, participant presentation, two-Handoff Pack, Transport output, restart/reload, and representative fail-fast errors.
- Run a true VS Code Extension Host acceptance attempt for the repaired path under Local Core and under the Published binding. A missing runner/dependency/environment capability is a blocker to a Sigma candidate and must be returned exactly; it must not be replaced by a synthetic PASS from unit tests.
- Existing focused regression/package integration/build/typecheck surfaces remain green or exact unrelated/environment limitations are reported without false PASS.
- Produce one self-contained Kodax-to-Anchor return carrying exact changed Extension VS Code source, qualified Evidence, the exact machine/Extension-Host acceptance receipts, known residual risks, and a clear `candidate-for-anchor-reconciliation` versus `blocked` disposition. Do not manufacture a Sigma handoff yourself.

## Scope

Extension VS Code host/controller implementation, host-owned lifecycle/runtime binding, integration/E2E test harness and tests, and bounded refactoring required to enforce the accepted Core boundary.

## Dependencies

- Anchor Core Tranche Acceptance Decision immediately preceding this Task.
- Anchor Architecture Recovery Reconciliation Decision.
- Independent VS Code Host Boundary Audit returned by Kodax.
- Exact Anchor-accepted Core Workspace carried with this delegation.
- Exact current Extension VS Code Workspace baseline carried with this delegation.
- Canonical Docs Workspace carried read-only for semantic/schema authority.

## Boundaries

- No Docs schema mutation and no new Handoff/participant/cache/material semantics in the extension.
- No Core mutation in this lane. If the accepted Core API is genuinely insufficient, stop and return the exact capability gap to Anchor instead of recreating it privately in VS Code.
- No Business semantic/governance rewrite beyond bounded technical Evidence and the required return Handoff.
- No optional endpoint/kind semantic widening, no Party Capacity auto-closure, no internal binding promoted to durable semantic Reference, and no repository-global inference fallback.
- No release, publication, deployment, push, or other remote mutation.
- No Sigma involvement during debugging. Sigma receives only a later Anchor-manufactured human gate after Anchor reconciles this return and machine acceptance is complete.
- Do not optimize for passing existing narrow tests if the real controller/Extension Host path still diverges. Architecture boundary and real-path behavior are acceptance requirements, not optional cleanup.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-anchor-core-tranche-acceptance.trace.md](001-1-4-1-3-5-1-2-1-anchor-core-tranche-acceptance.trace.md)
  - Value: zTXZ92BWFrRrCNXQPEQCnkFEQsXbnGqljHWQb4HW7Nk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: hP5Nf8xrog4gwgHMk2jQPu1qbB22vEsxABza35ElMgs