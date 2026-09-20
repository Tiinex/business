# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-20 10:33:15
  - Trace: [001-1-4-1-anchor-major-001-session-participant-and-operator-continuity-har.trace.md](001-1-4-1-anchor-major-001-session-participant-and-operator-continuity-har.trace.md)
  - Origin:
    - [relative](001-1-4-1-anchor-major-001-session-participant-and-operator-continuity-har.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-20 11:59:25
  - Authors: Anchor
  - Why: Axiom returned the canonical semantic classification; Anchor must reconcile it before implementation lanes proceed.
  - Summary: Accept Axiom's semantic separation and authorize Core-first projection before VS Code host adoption.
  - Status: ready/local

---

# Anchor Reconciliation — Human Session, Participant And Meeting Semantics

## Decision

- State: accepted-for-implementation
- Subject: Axiom semantic return for multi-human conversation/session identity, Role holding, semantic participation, speaker state and reusable meeting/process applicability.
- Decision: accept Axiom's returned separation without adding a Participant, Meeting, Conversation or Session schema. Preserve Party/person identity, Role identity, holder-assignment authorization, bounded consuming-session holder binding, semantic participant/relevance authority, process applicability and active-speaker state as separate claims. Route shared host-neutral projection mechanics to Loom first; route VS Code presentation/interaction only after the shared projection qualifies.

## Accepted Semantic Boundary

- A speaker label such as `Sigma:` is host-local speaker state only. It is useful operator state but does not establish durable Party/person identity, Role holding, holder binding, semantic participation, delegation or acceptance.
- A human may be a semantic participant without being forced into a Tiinex Role. Acting under a Role still requires the independently qualified holder-assignment/binding path for that Role.
- For Sigma, `explicit-participation` is the bounded assignment mode. Role authorization and an explicit participation occurrence are required; Role/cache carriage or conversational naming is insufficient.
- Semantic participant authority must be forward-selected by qualified controlling work/Handoff/Decision/process/Relation authority. Handoff endpoint, holder binding, Role inventory and carrier presence do not create participant membership.
- Process availability is not process applicability. One-off meetings/conversations may be initiated by ordinary Handoff/current-work semantics plus exact participant/process authority and expected durable outputs. Reusable interaction patterns belong in ordinary Business process lineage.
- The live transcript is working interaction, not durable provenance. Durable results remain in Decision, Feedback, Evidence, Task, Handoff, Relation or another owning artifact.

## Downstream Projection Contract

Shared Tooling may project, independently and with provenance, only exact qualified states for:

1. Party/person identity reference when established;
2. Role identity/reference and Role semantics;
3. holder-assignment authorization and exact Assignment Modes;
4. bounded consuming-session holder binding and assignment basis;
5. semantic participant/relevance authority and exact forward-selected source;
6. applicable interaction/process authority and exact forward-selected source;
7. expected durable outputs/completion boundary.

Unresolved or absent state must remain unresolved/absent. Active speaker remains separate host-local non-authoritative state.

VS Code may render semantic participant choices only from shared qualified participant projections. It may separately expose speaker-label/speaker-switch UX, but that host affordance must not manufacture semantic authority.

## Sequencing

1. Loom implements/qualifies the shared Core projection boundary and exact unresolved behavior.
2. Anchor audits the Loom return and integrates the accepted Core frontier.
3. VS Code implementation consumes the qualified Core projection and adds clear participant/speaker separation plus visible progress for long qualification/preview/manufacture waits.
4. Fresh-Anchor replay and Sigma live operator acceptance close the Major.

## Boundaries

- No new participant/session/meeting schema by convenience.
- No participant inference from Role/cache/endpoint inventory, display/account identity, chat position, speaker prefix, filename, package placement or transport topology.
- No transcript provenance promotion.
- No remote mutation or release authority is created by this Decision.
- Carrier Major, carrier dimension, artifact filename lineage, semantic Parent lineage and ChatGPT conversation numbering remain independent.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-anchor-major-001-session-participant-and-operator-continuity-har.trace.md](001-1-4-1-anchor-major-001-session-participant-and-operator-continuity-har.trace.md)
  - Value: G720AFkM8X7Eug8WzTPnRCFxcKNLIRZ6HJQG4FJPEeY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: qEyvt2XBjKbngSRrcEs7EARvAYf4fw4hNJ7-zZ5FYwc