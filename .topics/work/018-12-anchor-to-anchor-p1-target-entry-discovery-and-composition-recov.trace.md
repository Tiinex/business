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
  - Created At: 2026-10-05 19:51:32
  - Authors: Anchor
  - Why: Keep Target semantics provider-neutral and Core-owned while making the next host/UI tranche recoverable without conversation reconstruction.
  - Summary: Preserve the verified Core WHAT/WHERE Target discovery and composition frontier before VS Code presentation work.
  - Status: ready/local

---

## Handoff Parties

- Purpose: preserve the verified P1 host-neutral WHAT/WHERE Entry discovery and Target composition frontier before VS Code presentation work begins
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Transfers

- target-entry-discovery-and-composition-continuation
  - Transfer Kind: work-and-responsibility
  - Description: continue from the verified Core Target Entry discovery/composition boundary and implement host presentation from Core projections without duplicating Target semantics in VS Code
  - Controlling Artifact: [Recover Post-023 Authority And Lineage Closure Batch](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Boundary: local bounded P1 continuation only; no legacy Entry/Work migration, no P1 final acceptance claim, no Task closure, no hygiene cleanup, no remote mutation

## Required Context

- prior-p1-authority-frontier
  - Material: exact preceding P1 authority Handoff
  - Material Reference: [P1 Entry Process And Work Authority Recovery](018-11-anchor-to-anchor-p1-entry-process-and-work-authority-recovery-ha.trace.md)
  - Purpose: preserve what/where, Work-area/Reduction, Process decomposition, OpenAI placement and migration exclusions
  - Availability: available
- current-core-workspace
  - Material: exact current Core Workspace
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: host-neutral Entry catalog, Target discovery/composition projection and CLI input surface
  - Availability: available
- current-docs-workspace
  - Material: exact current Docs Workspace
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: canonical Target Entry schema authority including machine-readable Target Material declarations
  - Availability: available
- current-native-workspace
  - Material: exact current Native Workspace
  - Material Reference: [Native Workspace](native::.topics/.workspaces/tiinex-native.workspace.md)
  - Purpose: maintained Target Entry schema snapshot and provider-neutral reusable WHAT Entries
  - Availability: available
- current-openai-interop-workspace
  - Material: exact current OpenAI Interop Workspace
  - Material Reference: [OpenAI Interop Workspace](interop-openai::.topics/.workspaces/tiinex-interop-openai.workspace.md)
  - Purpose: ChatGPT Web WHERE Target Entry and referenced OpenAI-specific process material
  - Availability: available

## Reference Context

- target-entry-schema
  - Material: canonical Target Entry schema
  - Material Reference: [Target Entry Schema](docs::.topics/.schemas/entry/target/tiinex.entry.target.v1.schema.md)
  - Purpose: semantic WHAT/WHERE composition and Target discovery/authority boundaries
  - Availability: available
- chatgpt-web-target
  - Material: current ChatGPT Web Target Entry
  - Material Reference: [ChatGPT Web Target Entry](interop-openai::.topics/.entries/where/chatgpt-web/001-chatgpt-web-target-entry.trace.md)
  - Purpose: real provider-owned Target used to verify generic discovery/composition
  - Availability: available

## Current Verified Frontier

### Core Target discovery

- `projectPortableEntryCatalog` now classifies qualified Entry descendants as `purpose` or `target` from schema lineage rather than directory names.
- `tiinex.entry.target.v1` descendants project normalized Target identity: handle, kind, canonical target identifier, provider, host, declared capabilities/limitations, compatibility fields and Target Material references.
- Qualified Target Entry discovery remains schema-driven; `.entries/where/` is a human/discovery surface only.
- Existing Native Start/Explore/Resume Entries remain purpose Entries even on their legacy flat paths.

### Core WHAT/WHERE composition

- `projectWorkspaceCarrierEntry` now exposes purpose Entries through `modes` and Target Entries through a separate `targets` projection.
- Target options always include runtime `Generic / no target`; Target selection is optional.
- A selected purpose Entry may be composed with one qualified compatible Target Entry.
- Target family compatibility is evaluated in Core when explicitly declared.
- A Target requiring Entry capabilities that Core cannot yet qualify is withheld rather than silently treated as compatible.
- Rendered cold-start transport now preserves separate `Entry intent` and `Target intent` sections.
- Target guidance includes qualified Target identity, host/provider, capabilities/limitations and declared Target Material, followed by an explicit non-authority boundary.
- Target selection does not create Role authority, Handoff routing/work transfer, Process applicability, remote mutation authority, or override the WHAT Entry.

### CLI input boundary

- The existing `project-workspace-carrier-entry` operation accepts purpose Entry selection through `--mode`, `--entry`, or `--entry-id`.
- It accepts WHERE selection through `--target`, `--where`, `--target-entry`, or `--target-entry-id`.
- This is only an input/projection surface; no VS Code host UI has been implemented in this tranche.

### Schema correction discovered by dogfood

- The first Target discovery test showed that `Target Material` was human-described in `tiinex.entry.target.v1` but lacked the machine-readable rule that entries occur under `## Target Material`.
- The fix was made in canonical Docs schema authority, then copied byte-exact into Native.
- Core was not given a special Target-Material parser; generic named-declaration projection now supplies the references through the schema contract.
- The real ChatGPT Web Target now projects its ChatGPT continuity/source-discipline Process reference through the generic path.

## Verification

- Full current Core suite was executed in deterministic chunks to avoid host call time limits.
- Distinct Core test count after this tranche: **450**.
- Direct chunk runs: 68/68, 126/126, 118 pass + one environment skip out of 119, and 137/137; zero failures.
- The one skipped test was the npm package-surface test, skipped only because direct `node --test` lacks `npm_execpath`; it was rerun separately through `npm exec` and passed 1/1.
- Therefore all **450/450 distinct Core tests pass** under the intended execution environment.
- Focused Entry/Target tests: 15/15 pass.
- Native local-Core: 5/5 pass.
- OpenAI Interop: 1/1 pass.
- Real ChatGPT Web Target projection reports `entryKind=target`, canonical target `openai.chatgpt.web`, its declared capabilities/limitations and one qualified Target Material reference.

## Next Continuation

1. Keep Core as the semantic projection owner.
2. Inspect current VS Code Guided Entry host flow and replace/extend presentation so it consumes Core `modes` for WHAT and Core `targets` for WHERE.
3. UX target: first QuickPick selects WHAT (for example Explore); second QuickPick appears only when discovered Target options exist and offers `Generic / no target` plus qualified targets such as `ChatGPT Web`.
4. Reinvoke Core with the selected WHAT + WHERE rather than making VS Code compose or parse Target semantics itself.
5. Keep `where` discovery dynamic across carried/content-source Workspaces; do not hardcode OpenAI target names in VS Code.
6. Add host tests proving target discovery/presentation and that routed Handoff authority remains unchanged by Entry/Target selection.
7. Do not migrate legacy Native Entries or flat Work trees in this host tranche.

## Retained Responsibilities

- anchor-host-orchestration
  - Retained By: Anchor
  - Responsibility: implement the smallest VS Code presentation over the Core projection and preserve Core as semantic owner
  - Boundary: no new VS Code Target parser, no OpenAI-specific host semantics outside interop-openai
- anchor-architecture
  - Retained By: Anchor
  - Responsibility: keep Process schema decision, Work-area migration tooling, and CLI/Core ownership classification as separate later P1 work
  - Boundary: host UI work must not silently settle those unrelated questions

## Exclusions And Dependencies

- entry-migration
  - Kind: excluded-scope
  - Description: do not move existing Native WHAT Entries into `.entries/what/` in this tranche
  - Responsible Party Or Role: later qualified migration work
- work-tree-migration
  - Kind: excluded-scope
  - Description: do not restructure existing flat Work histories while implementing target selection UI
  - Responsible Party Or Role: later qualified migration work
- openai-hardcoding-in-host
  - Kind: excluded-scope
  - Description: VS Code must not embed `ChatGPT Web`, OpenAI capability lists, or Target compatibility semantics as local truth
  - Responsible Party Or Role: Core projection plus interop-openai material
- remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release, deployment, or provider mutation
  - Responsible Party Or Role: separately authorized operator

## Completion Expectation

- Signal Kind: result
- Signal Meaning: successor Anchor implements and verifies the VS Code WHAT→WHERE presentation over Core projections, or returns the smallest concrete host-boundary blocker without broadening scope
- Return To: Anchor
- Return To Reference: [Anchor Role](../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: P1 architecture is finally accepted, VS Code host acceptance is complete, legacy Entry/Work migration is authorized, Process schema is decided, Task 018 is closed, hygiene cleanup is authorized, or remote mutation is authorized
- Must Not Be Used To Claim: final host UX, final Target compatibility taxonomy, completed CLI extraction, migration completion, or Project closure

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md](018-recover-post-023-authority-and-lineage-closure-batch-task.trace.md)
  - Value: 7g55_HJ1fGhCLlR-o11oSeyefoUdu4dmxF90oujTy68

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: OWzAd7b3rcu7l9hbr6sasD9n-AMCS9lgAGIiNtudEdQ