# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-20 10:34:26
  - Trace: [001-1-4-1-1-anchor-to-axiom-human-session-participant-and-meeting-semantics.trace.md](001-1-4-1-1-anchor-to-axiom-human-session-participant-and-meeting-semantics.trace.md)
  - Origin:
    - [relative](001-1-4-1-1-anchor-to-axiom-human-session-participant-and-meeting-semantics.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-20 10:46:27
  - Authors: Axiom
  - Why: The received handoff requires one durable Axiom-to-Anchor semantic disposition before Core or VS Code implementation may begin.
  - Summary: Return the canonical separation of person/Role/holder/participant/speaker state, existing meeting/process applicability pattern, and downstream qualified/unresolved projection boundary with no implementation mutation.
  - Status: ready/local

---

# Axiom To Anchor — Human Session, Participant And Meeting Semantic Return

## Handoff Parties

- Purpose: return the canonical semantic disposition for multi-human identity/Role/holder/participant/speaker separation, meeting/conversation applicability, and the exact downstream shared-Tooling/VS Code projection boundary without implementation mutation.
- From: Axiom
- From Kind: role
- From Reference: [Axiom Role — Canonical Holder Cutover Continuation](business::.topics/roles/001-2-1-axiom-canonical-holder-cutover-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role — Canonical Holder Cutover Continuation](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Semantic Disposition

### Multi-human identity, Role, holder, participant and speaker separation

- Party/person identity is a durable identity claim only when explicit qualified Party/person authority establishes it. The current conversation, account identity, display name, writing style, message order, speaker prefix, Role inventory, Handoff endpoint or carrier presence does not establish a particular durable person Party.
- Role identity is the reusable qualified `tiinex.party.role.v1` capacity artifact. Knowing or carrying a Role establishes that Role's meaning and boundaries only; it does not establish a current holder, semantic participant, active speaker, delegation, acceptance or durable person identity.
- Holder-assignment authority is the qualified Role's `Holder Relationship -> Assignment Modes`. It authorizes only the named bounded assignment mechanisms; it is not itself an occurrence of holding. Session assertion, assignment authorization, resulting bounded holder binding and durable holder identity remain separate claims.
- For the current Sigma Role, `explicit-participation` is the bounded assignment mode. A human may therefore act in Sigma capacity only after an explicit participation assertion/selection is paired with the qualified Sigma Role authorization. A textual `Sigma:` speaker label alone is host/operator speaker state and does not satisfy semantic participation, holder binding or durable identity by convenience.
- Consuming-session holder binding is the bounded result of one qualified assignment occurrence for one Role in the current consuming session. It may be qualified, unresolved or absent independently for each Role. It does not create a permanent holder relationship and does not by itself make the holder a semantic participant in a broader interaction.
- Semantic participant authority is a current interaction/work relevance claim. It requires explicit qualified forward authority from the controlling Role/Task/Epic/Handoff/Decision/process and/or typed Relation chain. Existing Party/Role + typed Relation + Handoff/Task/Decision/process semantics remain sufficient; no new Participant schema is justified by this use case. Role/cache carriage, Handoff endpoint presence, holder binding or speaker state must not be promoted into participation.
- A participant may be qualified as a Party/person or as a Role/capacity according to the controlling authority. A human need not be forced into a Tiinex Role merely to be present; conversely, acting under a Role requires the independently qualified holder-assignment/binding path for that Role.
- Active speaker state is conversational/host state only. It may identify which local speaker label is currently producing input, but it is non-authoritative and must remain mechanically separate from Party identity, Role identity, holder binding and semantic participant authority. If durable attribution matters to a Decision, Feedback, Evidence or other output, the owning durable artifact carries that attribution/evidence; the transcript itself does not become provenance.

### Meeting/conversation applicability

- No new Meeting, Conversation, Participant or Session schema is required for the transferred use case.
- The lowest existing pattern is: controlling work/lineage selects the interaction purpose; explicit qualified current-work authority selects participant/relevance claims; applicable reusable process authority is selected forward from the controlling Role/Task/Epic/Handoff/Decision and, where needed, an explicit typed Relation; Required Context carries the exact process/adoption/applicability and participant authority needed by a cold recipient; Role holder binding is then resolved independently for any participant expected to act in a Role capacity.
- Process presence or qualification establishes availability only. Applicability, requiredness, active execution, participant membership, Role holding, ownership/responsibility and completion evidence remain separate facts with separate authority. Reverse scanning, process inventory, filenames, repository adjacency, Role inventory and carriage are not applicability authority.
- A one-off Handoff may start a bounded conversation/meeting by carrying its controlling work, interaction purpose, explicit participant/relevance authority, required context and expected durable outputs. The Handoff endpoint alone is not the participant declaration; participant authority must still be forward-qualified rather than inferred from routing.
- When an interaction pattern is reusable, represent it as the ordinary Business process artifact and select its applicability through the already-qualified forward applicability pattern. An explicit applicability Relation may bind the process to a bounded target context without turning the Relation label into a global privileged predicate.
- The live conversation is working interaction, not durable provenance. Durable results remain in the artifact family that owns the truth: Decision, Feedback, Evidence, Task, Handoff, Relation or another qualified owned artifact. No transcript-to-provenance promotion is introduced.

### Downstream projection boundary

Shared Tooling may project the following semantic dimensions only from exact qualified authority and must preserve `unresolved`/absent states rather than filling them from inventory or host context:

1. qualified Party/person identity reference, when one exists;
2. qualified Role identity/reference and its bounded Role semantics;
3. holder-assignment authorization, including exact Assignment Modes and source authority;
4. current consuming-session holder binding and its exact assignment basis;
5. semantic participant/relevance authority and its exact forward-selected source;
6. applicable interaction/process authority and its exact forward-selected source;
7. expected durable outputs/completion boundary from the controlling Handoff/process/current work.

Active speaker is a separate host-local state. Shared Tooling may transport/display it only as non-authoritative operator state. Mapping that state to a semantic Role requires the independently qualified Role plus bounded holder binding, and using it as a participant choice additionally requires qualified participant authority.

VS Code may render participant choices only from shared qualified participant projections. It may expose a clearly separate host-only speaker-label/speaker-switch affordance, but that affordance must not create Party identity, Role holding, participant authority, process applicability, delegation or acceptance. When semantic participant authority is unresolved, the UI must preserve and display the unresolved state rather than treating available Roles, endpoints or cached material as selectable participants.

## Transfers

- multi-human-session-semantic-disposition
  - Transfer Kind: work-and-responsibility
  - Description: accept the separation of Party/person identity, Role identity, holder-assignment authorization, bounded consuming-session holder binding, semantic participant authority and active-speaker state as independent claims with independent authority.
  - Boundary: no textual speaker label, account/display identity, chat position, Role inventory, Handoff endpoint, cache/carrier presence or holder binding is promoted into a stronger claim by convenience.

- meeting-conversation-applicability-disposition
  - Transfer Kind: work-and-responsibility
  - Description: use existing Handoff/Task/Decision/process/typed-Relation semantics for bounded meeting/conversation purpose, explicit forward participant relevance, process applicability and durable outputs; introduce no new meeting/participant/session schema for this use case.
  - Boundary: process availability is not applicability, routing is not participant membership, and the live conversation is not durable provenance.

- downstream-projection-boundary
  - Transfer Kind: responsibility
  - Description: route shared projection implementation to Loom and host presentation to VS Code only after Anchor reconciliation, preserving the separate qualified/unresolved dimensions returned here and keeping active-speaker state non-authoritative.
  - Boundary: Axiom does not implement Core or VS Code source; downstream hosts must not manufacture missing semantic authority.

## Required Context

- controlling-major-task
  - Material: Anchor Major 001 — Session, Participant And Operator Continuity Hardening.
  - Material Reference: [Controlling Task](business::.topics/processes/gpt/grounding/001-1-4-1-anchor-major-001-session-participant-and-operator-continuity-har.trace.md)
  - Purpose: exact Major scope, sequencing and acceptance criteria.
  - Availability: available

- received-semantic-handoff
  - Material: Anchor To Axiom — Human Session, Participant And Meeting Semantics.
  - Material Reference: [Received Handoff](business::.topics/processes/gpt/grounding/001-1-4-1-1-anchor-to-axiom-human-session-participant-and-meeting-semantics.trace.md)
  - Purpose: exact transferred semantic questions, exclusions and completion expectation.
  - Availability: available

- holder-semantics-basis
  - Material: Canonical Holder Semantics And Blocker-Return Closure Reconciliation.
  - Material Reference: [Holder Semantics Decision](business::.topics/initiatives/001-2-7-5-1-4-holder-semantics-and-return-closure-reconciliation.trace.md)
  - Purpose: accepted separation of assignment authorization, session assertion, bounded holder binding and durable identity plus canonical Assignment Modes.
  - Availability: available

- process-applicability-basis
  - Material: Second Specialist Reconciliation And Process-Grounding Disposition.
  - Material Reference: [Process Applicability Decision](business::.topics/initiatives/001-2-7-2-2-second-specialist-reconciliation-and-process-grounding-disposition.trace.md)
  - Purpose: accepted forward-only process applicability semantics and no-new-participant/process-schema boundary.
  - Availability: available

- current-sigma-role
  - Material: Sigma Role — Canonical Holder Cutover Continuation.
  - Material Reference: [Sigma Role](business::.topics/roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)
  - Purpose: exact `explicit-participation` holder mode and human-role authority boundary.
  - Availability: available

## Reference Context

- operator-session-process-continuation
  - Material: Successor Grounding Gap Review — Operator Session And Human Participation Continuation.
  - Material Reference: [Process Continuation](business::.topics/processes/gpt/grounding/001-1-4-successor-grounding-gap-review-operator-session-and-human-partic.trace.md)
  - Purpose: observed multi-human and host/operator facts that motivated this classification; not independent semantic authority.
  - Availability: available

- applicability-relation-pattern
  - Material: Foundation Work-Turn Applicability Relation.
  - Material Reference: [Applicability Relation](business::.topics/processes/002-1-1-foundation-cross-repository-work-turn-applicability-relation.trace.md)
  - Purpose: existing bounded pattern for explicit process applicability without global predicate invention.
  - Availability: available

## Retained Responsibilities

- integration-and-major-control
  - Retained By: Anchor
  - Responsibility: reconcile this semantic disposition into the controlling Major, preserve fixed scope, dispatch exact implementation lanes, and own subsequent acceptance/recovery.

- shared-tooling-implementation
  - Retained By: Loom
  - Responsibility: after Anchor reconciliation, implement only the shared host-neutral projections/mechanics required to expose the returned qualified/unresolved dimensions without semantic inference.

- host-presentation-and-interaction
  - Retained By: VS Code implementation lane
  - Responsibility: render Core-qualified participant choices and progress/wait states, and keep any speaker-switch UX explicitly separate from semantic authority.

- human-host-gate
  - Retained By: Sigma
  - Responsibility: exercise the real VS Code operator path later, provide bounded observation/test/audit evidence, and perform only separately authorized commit/push or return feedback plus a qualified carrier.

## Exclusions And Dependencies

- no-new-schema-by-convenience
  - Kind: excluded-scope
  - Description: do not introduce a Participant, Meeting, Conversation or Session schema merely to mirror host UI state; current semantic primitives are sufficient for this use case.

- no-prefix-or-account-authority
  - Kind: excluded-scope
  - Description: do not make `Sigma:`, display/account identity, writing style, chat position or message order into Party identity, Role holding, participant membership or acceptance authority.

- no-endpoint-participation-inference
  - Kind: excluded-scope
  - Description: Handoff endpoint, Role/cache carriage or current holder binding does not itself establish semantic participant authority.

- implementation-after-anchor-reconciliation
  - Kind: unresolved-dependency
  - Description: Core/VS Code changes depend on Anchor reconciling this return and dispatching exact bounded implementation work.
  - Responsible Party Or Role: Anchor

## Completion Expectation

- Signal Kind: return
- Signal Meaning: Anchor receives one qualified Axiom → Anchor return that closes the transferred semantic classification, introduces no unnecessary schema, and supplies exact qualified/unresolved projection boundaries for Loom and VS Code without implementation mutation.
- Return To: Anchor
- Return To Reference: [Anchor Role — Canonical Holder Cutover Continuation](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: the current conversation establishes a durable person Party; Sigma is permanently held by any particular person; every qualified holder is a meeting participant; every participant must hold a Role; every conversation needs durable participant materialization; or one-off host speaker state requires a canonical artifact.
- Must Not Be Used To Claim: participant authority from Role inventory or endpoint presence; holder identity from speaker labels; process applicability from process availability; acceptance or delegation from participation; transcript provenance; remote mutation authority; or implementation completion.
- Authority Limits: this return completes Axiom's semantic-classification lane only. Anchor owns reconciliation and orchestration; Loom owns shared Tooling implementation qualification; VS Code owns host UX/integration; Sigma owns the declared bounded human observation/gate.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-1-anchor-to-axiom-human-session-participant-and-meeting-semantics.trace.md](001-1-4-1-1-anchor-to-axiom-human-session-participant-and-meeting-semantics.trace.md)
  - Value: a7Do5DpfVqEGt_wMf06bNT7v1_nQ3DeS5F5nl0IO8bM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 5kDQJHxNKucBnqMA4xe9sUM_K1aC7Hb41_Otp82Lc3o