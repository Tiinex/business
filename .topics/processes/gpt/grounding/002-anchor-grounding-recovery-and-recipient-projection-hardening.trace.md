# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-12 17:09:27
  - Trace: [010-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-anchor-production-successor-takeover.trace.md](../../../initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-anchor-production-successor-takeover.trace.md)
  - Origin:
    - [relative](../../../initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-anchor-production-successor-takeover.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-12 19:09:24
  - Authors: Anchor
  - Why: The current successor recovered bounded authority correctly but required Sigma correction turns to prioritize stable self-grounding, program-map recovery and scan-first recipient behavior; ChatGPT branch/turn limits make those gaps operationally expensive.
  - Summary: Harden fresh/re-grounded Anchor behavior, durable Recovery hygiene, recipient projection and safe orchestration throughput before Sub-Anchor scaling.
  - Status: ready/local

---

# Anchor Grounding, Recovery And Recipient Projection Hardening

## Objective

Make fresh and re-grounded Anchor behavior reliably recover the durable Tiinex-wide mission, Role boundary, program map, current carrier/frontier and qualified recipient needs before local execution dominates attention, while keeping the behavior portable to non-Tiinex projects that adopt the same Roles/process patterns.

## Done Criteria

- Fresh Anchor takeover follows the already-adopted stable-baseline-then-current-frontier grounding order before bounded execution; package/task readiness must not be treated as proof of project-wide Anchor grounding.
- Re-grounding is treated as Anchor hygiene, not only cold-start bootstrap. Specialist returns, new Recovery, Major open/close, source reconciliation, authority uncertainty and material context drift are explicit triggers to reassess the relevant program map before continuing.
- Recipient projection becomes operational behavior: when Sigma or another qualified human gate is the current recipient, default output is visually scannable and starts with meaningful delta, blocker and next human action rather than implementation history.
- Sigma-facing work labels visually separate Prefix/Major, Role and Workspace. A compact default such as `[Prefix / Major] -> [Role]`, State, Scope, Flow and Human Action is preferred where it preserves meaning; code blocks are used for copyable transport/routing text and scan-friendly state summaries.
- Chat-provider identity and nickname are non-authoritative. A nickname such as `Sigma`, `0` or any other host label must not assign a Tiinex Role or holder capacity; qualified Role material plus explicit interaction/session binding remains the basis.
- Branch/fork signals in a disposable chat runtime cause the Role to recommend a fresh start from the newest qualified Recovery/carrier rather than extending a fragile branched conversation. Host chat titles may be used only when actually visible; explicit user branch notation is sufficient evidence when provided.
- Accepted changes intended to survive provider/session loss are followed by a stable, committable Recovery checkpoint and refreshed master Anchor carrier so normal loss is bounded to the latest uncheckpointed iteration rather than durable project state.
- Anchor actively considers safe parallel Majors after grounding. Independent work should be delegated in parallel when scope, authority and reconciliation boundaries are clear and the wall-time saving outweighs coordination overhead.
- Sub-Anchor use remains an experiment gated on stable fresh/re-grounding behavior. When tried, Sub-Anchors cover meaningful program segments rather than one wrapper per specialist; Master Anchor retains cross-segment coherence, shared-scope coordination, final audit and human gates.
- The process is tested through fresh successors without coaching: durable material -> correct North Star/program map -> recipient-appropriate communication -> bounded work, with correction turns treated as evidence for improvement rather than hidden operator burden.

## Current Evidence

- The current successor required Sigma prompting to prioritize Tooling-backed stable self-grounding and to inspect historical Anchor workflow before recovering the wider program model. This is a real correction turn even though bounded authority/scope handling was otherwise strong.
- Video/history review showed useful prior behavior: Anchor maintained a multi-lane send queue/program map, cold-ground-tested corrected carriers, delegated fresh specialists, and manufactured full Recovery checkpoints after meaningful frontier changes.
- Sigma reports ChatGPT conversations may become non-continuable after roughly 20-30 turns depending on intensity; branched continuation can lose sandbox state, while user-exposed carrier files remain transportable. This makes durable Recovery frequency a reliability concern, not only convenience.
- Sigma also reports that scan-first presentation materially improves usability for dyslexia: stable visual patterns and short copyable blocks are preferable to prose-heavy status when the same meaning can be preserved.

## Scope

Business/Anchor process, grounding/re-grounding reliability, recipient projection, Recovery hygiene and orchestration-throughput behavior. This Task may route implementation/documentation changes to the owning Business/Docs/Core/host repository as separate bounded work when required.

## Dependencies

- Current qualified Anchor Role, executive grounding, two-phase grounding Process/adoption Decision and Sigma Role.
- Current full Recovery and production successor takeover as the durable transient frontier.
- Future specialist returns, branch/fresh-start observations and Sigma human-gate observations as evidence for whether the process is behaving naturally.
- Owning repository/Role delegation when a discovered grounding defect belongs to Docs, Core, a host extension or another specialist surface.

## Exclusions

- Do not redefine `grounded-to-act` as global project understanding; it remains bounded route/action readiness.
- Do not create new canonical grounding states merely because local mental models such as task/frontier/Anchor-grounded are useful explanations.
- Do not make `human == Sigma`, hardcode a ChatGPT nickname, or make provider-specific UI state semantic authority.
- Do not create Sub-Anchors merely because they are possible; require measurable coordination/throughput value.
- Do not weaken existing Tiinex principles, schema authority, exact-byte reconciliation or fail-closed package behavior for convenience.

## Near-Term Gate

Use the next real specialist returns and fresh sessions as evidence. Anchor should re-ground without Sigma prompting, keep a readable program map, refresh durable Recovery after accepted work, and surface only the human action Sigma actually needs. When this behavior is stable enough in practice, Anchor should proactively propose the first bounded Sub-Anchor experiment; Playthings plus its dependencies is the current candidate segment.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [010-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-anchor-production-successor-takeover.trace.md](../../../initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-anchor-production-successor-takeover.trace.md)
  - Value: j6rJnhk5iSvszAADNr_hiOh67-cel_aQ_o7q1pW5uMM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: mK4JerPYAZOZ_kE5IiYaXyvvMaJG088uZtuBc-a9VBw