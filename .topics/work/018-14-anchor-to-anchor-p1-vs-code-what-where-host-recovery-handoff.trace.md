# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-05 13:22:47
  - Trace: [018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Origin:
    - [relative](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-10-05 21:13:44
  - Authors: Anchor
  - Why: Keep the host result recovery-safe without duplicating VS Code implementation truth in Business or broadening into migration/release acceptance.
  - Summary: Preserve the verified VS Code WHAT-to-WHERE Guided Entry host presentation, Workspace-local work evidence and exact locked-dependency build limitation.
  - Status: ready/local

---

## Handoff Parties

- Purpose: preserve the verified VS Code WHAT -> WHERE Guided Entry host presentation and its exact verification boundary before external dogfood or further P1 architecture work
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Transfers

- vscode-guided-entry-what-where-host-frontier
  - Transfer Kind: work-and-responsibility
  - Description: continue from the bounded VS Code host implementation that presents Core-owned purpose Entry WHAT choices followed by optional compatible Target WHERE choices, without duplicating Target/OpenAI semantics in the extension
  - Controlling Artifact: [Recover Post-023 Authority And Lineage Closure Batch](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Boundary: local host implementation/recovery only; no P1 final acceptance, no legacy Entry/Work/Process migration, no Task 018 closure, no release/publish claim, no remote mutation

## Required Context

- typed-process-maintenance-frontier
  - Material: exact preceding typed Process recovery Handoff
  - Material Reference: [P1 Typed Process Maintenance Recovery](018-13-anchor-to-anchor-p1-typed-process-maintenance-recovery-handoff.trace.md)
  - Purpose: preserve the governing Process-development discipline and corrected Native/OpenAI typed process topologies
  - Availability: available
- current-vscode-workspace
  - Material: exact current VS Code Workspace
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: owning Workspace for the bounded host implementation and Workspace-local work-area evidence
  - Availability: available
- vscode-local-task
  - Material: exact Workspace-local host Task
  - Material Reference: [VS Code Guided Entry What Where Presentation](vscode::.topics/work/guided-entry-what-where/001-vs-code-guided-entry-what-where-presentation.trace.md)
  - Purpose: bounded implementation request and completion criteria in the natural owning Workspace
  - Availability: available
- vscode-verification-evidence
  - Material: exact Workspace-local verification Evidence
  - Material Reference: [VS Code Guided Entry What Where Verification Evidence](vscode::.topics/work/guided-entry-what-where/001-1-vs-code-guided-entry-what-where-verification-evidence.trace.md)
  - Purpose: exact runtime/Core regression result, real-carrier projection and environment-bound TypeScript-build limitation
  - Availability: available
- current-core-workspace
  - Material: exact current Core Workspace
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: verified WHAT/WHERE Entry/Target discovery, compatibility and final transport composition authority
  - Availability: available
- current-native-workspace
  - Material: exact current Native Workspace
  - Material Reference: [Native Workspace](native::.topics/.workspaces/tiinex-native.workspace.md)
  - Purpose: provider-neutral Entry/Target schema snapshot and reusable WHAT Entries
  - Availability: available
- current-openai-interop-workspace
  - Material: exact current OpenAI Interop Workspace
  - Material Reference: [OpenAI Interop Workspace](interop-openai::.topics/.workspaces/tiinex-interop-openai.workspace.md)
  - Purpose: ChatGPT Web WHERE Target Entry and OpenAI-specific Target/Process material
  - Availability: available

## Reference Context

- p1-target-entry-authority
  - Material: exact preceding Target Entry discovery/composition recovery Handoff
  - Material Reference: [P1 Target Entry Discovery And Composition Recovery](018-12-anchor-to-anchor-p1-target-entry-discovery-and-composition-recov.trace.md)
  - Purpose: preserve the Core WHAT/WHERE semantic projection contract consumed by this VS Code host implementation
  - Availability: available
- process-development-maintenance
  - Material: reusable Process Development And Maintenance root
  - Material Reference: [Process Development And Maintenance](../processes/process-development-and-maintenance/001-process-development-and-maintenance.trace.md)
  - Purpose: keep future material Process changes behind the qualified typed Process maintenance discipline rather than host-side improvisation
  - Availability: available

## Current Verified Host Result

### WHAT -> WHERE presentation

- VS Code still asks Core for the Guided Entry catalog and renders Core `modes` as the first QuickPick, now titled `Guided Entry · What`.
- After WHAT selection (and Custom instruction when applicable), VS Code calls Core again for the selected Entry and consumes Core `targetOptions`.
- A second `Guided Entry · Where (optional)` QuickPick appears only when at least one non-generic Target is discovered.
- Core-projected `Generic / no target` remains available; provider, host, label, summary and Target identity are presentation data projected by Core rather than host-owned semantics.
- The selected Target identity is returned to Core through `--target-entry-id` for final transport rendering.
- Primary Role and participant selection still occur after WHAT/WHERE; Target selection does not alter Handoff routing, recipient authority or Role-holder semantics.

### Host/Core ownership boundary

- VS Code contains no hardcoded `ChatGPT Web`, OpenAI Target list, capability matching or Target compatibility logic.
- Real current carrier projection yields WHAT `Explore`, `Resume`, `Start`, `Custom` and WHERE `Generic / no target`, `ChatGPT Web` from carried Native/OpenAI material.
- Selecting `Explore + ChatGPT Web` returns Core status `ready`, canonical target `openai.chatgpt.web`, and transport containing both `Entry intent: Explore` and `Target intent: ChatGPT Web`.
- The VS Code wrapper accepts the new Target identity while preserving the previous positional `ProcessRunner` call shape so older host/test callers are not accidentally reinterpreted as Target IDs.

### Workspace-local work pattern dogfood

- The VS Code implementation is represented in the owning Workspace at `.topics/work/guided-entry-what-where/` rather than adding another implementation journal entry to Business.
- That work area currently contains one bounded Task plus its verification Evidence, demonstrating the new Work Scaffold convention without migrating legacy work trees.
- Business retains the cross-Workspace orchestration/recovery Handoff and controlling Task rather than duplicating VS Code implementation truth.

### Verification

- VS Code bridge runtime regression: **147/147 pass** against an exact locally assembled current Core/Native/OpenAI package-surface composition.
- Focused Core Entry/Target regression: **16/16 pass** for `entry-catalog` + `workspace-entry-projection`.
- Targeted host assertions pass for exact `--target-entry-id` forwarding, legacy positional-runner compatibility and explicit WHAT -> WHERE -> Role ordering without OpenAI hardcoding.
- Real carrier WHAT/WHERE projection and final render pass against the current recovery package.
- VS Code Workspace Tiinex inspect is clean with zero findings after the Workspace-local Task/Evidence are authored.
- One pre-existing VS Code config/test mismatch was repaired: `Tiinex: Build linked extension (Local)` is now a non-default Build task, matching the already-existing repository test and the sibling Latest shortcut.

## TypeScript Build Environment Boundary

- A fresh ordinary repository `npm run build` is **not claimed** in this container.
- The uploaded Workspace does not carry `node_modules`, the local npm cache lacks `undici-types`, and an online npm restore fails with registry DNS `EAI_AGAIN`; therefore the exact locked `@types/vscode@1.95.0` dev dependency cannot be restored here.
- The changed TypeScript modules transpile successfully for runtime verification and the complete runtime bridge suite exercises the emitted behavior, but a clean canonical typecheck/build remains a later environment gate when the locked dev dependencies are available.
- This limitation is environment evidence, not permission to hand-write substitute VS Code typings into canonical source or to claim release readiness.

## Next Continuation

1. Prefer real-user/real-VS-Code dogfood of Guided Entry: select `Explore` then `ChatGPT Web`, verify the second dropdown appears dynamically, and inspect the produced transport text.
2. When an environment with the locked npm dev dependencies is available, run the normal `npm run typecheck` / `npm test` / package checks and treat any new compile finding as a concrete host blocker.
3. If host dogfood is clean, return to remaining bounded P1 questions separately: Process-root schema need (only if justified), Work/Reduction authoring+migration tooling, and CLI/Core ownership classification.
4. Do not migrate legacy `.entries`, Work trees or historical Topic process branches merely because the new structures now have dogfood evidence.

## Retained Responsibilities

- anchor-host-orchestration
  - Retained By: Anchor
  - Responsibility: reconcile real VS Code dogfood or the clean canonical build gate, and repair only concrete host blockers before broader P1 continuation
  - Boundary: no inference of release acceptance or Task closure
- anchor-architecture
  - Retained By: Anchor
  - Responsibility: keep later Process-schema, Work-migration and CLI-boundary work separate from this completed host presentation slice
  - Boundary: VS Code success does not settle those wider architecture questions

## Exclusions And Dependencies

- legacy-entry-work-migration
  - Kind: excluded-scope
  - Description: do not move existing flat Entries or historical Work trees during host dogfood
  - Responsible Party Or Role: later explicitly qualified migration work
- provider-hardcoding
  - Kind: excluded-scope
  - Description: do not encode OpenAI/ChatGPT Target identity or compatibility semantics in VS Code
  - Responsible Party Or Role: Core projection plus interop-openai material
- release-acceptance
  - Kind: excluded-scope
  - Description: runtime regression and real projection do not substitute for a clean locked-dependency TypeScript build, real desktop UI dogfood, or release audit
  - Responsible Party Or Role: later host/release acceptance work
- remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release, deployment or provider mutation
  - Responsible Party Or Role: separately authorized operator

## Completion Expectation

- Signal Kind: result
- Signal Meaning: successor Anchor receives a recovery-safe VS Code WHAT->WHERE host implementation and should next reconcile real host/build dogfood rather than re-derive Target semantics or broaden into migration
- Return To: Anchor
- Return To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: P1 architecture is finally accepted, VS Code release is accepted, Task 018 is closed, legacy trees are migrated, `process.v1` is decided, CLI extraction is complete, or remote mutation is authorized
- Must Not Be Used To Claim: clean locked-dependency TypeScript build in this container, real desktop UI acceptance, Marketplace readiness, migration completion, or Project closure

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Value: 7g55_HJ1fGhCLlR-o11oSeyefoUdu4dmxF90oujTy68

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: LDaU9wh83uRMGgdX-VAVegmiHMGKF5zyt1JSBwI6vpE