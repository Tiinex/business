# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-27 22:51:00
  - Authors: Axiom
  - Why: Resolve the bounded Anchor-to-Axiom tranche on human transport, receiver qualification, explicit human dialogue, Practitioner specialization, and host/presentation separation without claiming Tooling implementation or publication.
  - Summary: Axiom semantic disposition for human-as-courier defaults, explicit human participation, receiver qualification, Role baseline composition, multi-human dialogue relations, and Loom acceptance evidence.
  - Status: accepted/local

---

# Human Transport And Receiver Contract Semantic Disposition

This Decision records the Axiom-owned semantic disposition for the bounded Anchor handoff received in `tiinex-business-004-anchor-to-axiom.handoff-package.zip`, controlling route `001-3-2-anchor-to-axiom-transport-contract-handoff.trace.md`.

## Decision

- State: accepted within Axiom schema-semantic authority
- Subject: Tiinex Handoff semantics for human transport, receiver-qualified continuation, explicit human dialogue, blocking on human input, terminal closure, Practitioner specialization, and host-specific presentation
- Decision: preserve Handoff as the semantic owner of bounded transfer and logical endpoints; add only a minimal optional human-participation declaration to Handoff; keep blocking and terminal closure on existing dependency/completion semantics; treat receiver qualification and the Human Transport Contract as projection/qualification rules rather than new authority-bearing schemas; add first-class non-Parent Role baseline composition to `tiinex.party.role.v1`; represent additional human dialogue participants through typed non-Parent relations when durable participation evidence is needed; leave attachment count, adjacency, code-block/TTS behavior, package aggregation, and host rate limits to Tooling/presentation/host-profile policy.

### 1. Semantic ownership split

#### `tiinex.handoff.v1`

Handoff continues to own:

- the logical `From` and intended logical `To`;
- the bounded work/responsibility transfer;
- required and reference context;
- retained responsibilities;
- unresolved dependencies and exclusions;
- the completion-facing signal, including `Return To`;
- the new minimal declaration of whether supporting human semantic participation is explicitly requested.

Handoff must continue not to own:

- ZIP/package topology;
- attachment count;
- upload mechanics;
- message placement;
- code-block rendering;
- TTS behavior;
- host rate limits;
- delivery receipts;
- acceptance state inferred from transport.

The existing Handoff rule that the physical sender/receiver of a ZIP or message is not a semantic endpoint unless declared remains controlling.

#### Typed companion artifact or relation

Use `tiinex.relation.v1` when a participation relation itself is worth preserving, especially for additional human participants in an opened dialogue.

Canonical relation shape for bounded dialogue participation:

- Relation Type: `participates in handoff dialogue`
- Relation Direction: `handoff or dialogue context -> participant`
- Relation Scope: `bounded dialogue participation only`

A relation target may be a Party artifact, Role artifact, external descriptor, or bounded textual descriptor. The relation does not prove identity, permanent role holding, delegation, decision authority, consent beyond what is separately evidenced, or recipient acceptance.

Do not create a standalone Relation artifact merely because a human mechanically carried a package. Mechanical transport is not a semantic participation relation by default.

#### Practitioner and specialized Role obligations

The provider-neutral Practitioner baseline should carry the behavioral obligation that, for ordinary inter-role handoffs, a human carrier is not semantic middleware by default.

A specialized role incorporating the Practitioner baseline should therefore:

- produce receiver-qualified continuation when a logical next receiver exists;
- not require the human carrier to summarize, reinterpret, infer, or rewrite semantic instructions;
- explicitly request human dialogue when human observation, policy, priority, choice, clarification, or another human contribution is actually needed;
- keep ordinary human-facing status distinct from copy-ready receiver text;
- preserve the shared-interface principle: humans and LLMs consume the same semantic truth even when their presentation differs.

These are Role/baseline obligations and transport qualification rules, not authority granted to the courier.

#### Tooling, presentation, and host-profile policy

The following remain outside canonical Handoff semantics:

- one attachment per hop;
- whether the attachment is one Markdown artifact or an aggregate ZIP/package;
- attachment-link placement;
- adjacency of human action, attachment, and receiver text;
- use of code blocks for copy-ready text;
- keeping ordinary status outside code blocks because a current TTS surface does not read code-block contents;
- short-status verbosity preferences;
- package aggregation behavior;
- the observed approximately 60-files-per-3-hours host attachment-rate constraint.

A reusable implementation-neutral courier surface may be described with `tiinex.presentation.surface.v1` and reusable semantic prompts/actions may be described with `tiinex.interaction.unit.v1`, but neither should duplicate Handoff transfer authority. A ChatGPT-specific rate or rendering behavior belongs in a host profile bound to that surface/tooling, not in Tiinex Handoff semantics.

### 2. Minimal semantic distinction: use orthogonal facts, not a four-state machine

Do not add a four-value protocol state for `transport-only`, `human dialogue`, `blocked`, and `terminal`.

The minimum durable model is two existing axes plus one small new declaration:

1. **Human semantic participation**
   - `not-requested`
   - `dialogue-requested`

2. **Execution readiness/blocking**
   - already represented by `Required Context -> Availability` and `Exclusions And Dependencies -> Kind: unresolved-dependency`;
   - a handoff is waiting on human input when human dialogue is requested and an unresolved dependency or unavailable/unresolved required context makes continuation contingent on that input;
   - no new `blocked` Handoff state is required.

3. **Completion/closure**
   - already represented by `Completion Expectation`;
   - `Signal Kind: none` is terminal/no receiver return required;
   - a non-`none` completion signal plus `Return To` identifies the expected logical return target;
   - no new `terminal` Handoff state is required.

This avoids a state machine that would duplicate facts already owned by dependency and completion semantics.

For older Handoffs that do not carry the new optional participation section, absence means only that human participation was not explicitly declared in the artifact. A transport/Practitioner policy may still apply the ordinary mechanical-courier default, but validators must not rewrite absence into a stronger historical claim.

### 3. Logical receiver, courier action, and acceptance boundary

The logical receiver is already `Handoff Parties -> To`. For a completion return, the logical return receiver is `Completion Expectation -> Return To`.

Do not add another receiver identity field and do not introduce a separate Receiver Contract artifact.

The expected human transport action is a derived transport/presentation instruction, not a transfer of semantic authority. A projection may truthfully say, for example, that the human should deliver the attached artifact unchanged to the declared logical receiver and bring the declared completion result back to the declared return target.

That projected action must obey these rules:

- the courier is not asked to interpret or summarize unless human dialogue is explicitly requested;
- the courier may choose or operate the host interaction needed to deliver material, but that mechanical choice is not semantic authorship or acceptance;
- transport delivery does not prove that `To` accepted the handoff;
- transport delivery does not prove completion;
- the projected instruction must not silently substitute a different receiver for `To` or `Return To`.

### 4. Human Transport Contract disposition

Do not create `tiinex.human.transport.contract.v1`.

“Human Transport Contract” is a useful name for a projection/qualification profile composed from:

- Handoff endpoint and completion semantics;
- optional Handoff human-participation semantics;
- carrier/package control facts owned by Tooling;
- optional reusable `tiinex.interaction.unit.v1` definitions for human action text;
- optional reusable `tiinex.presentation.surface.v1` definition for the courier-facing surface;
- a host profile for attachment, layout, code-block, TTS, and rate-limit behavior.

The profile may be versioned and tested, but it must not become a second semantic authority over Handoff.

### 5. Receiver Contract disposition

Do not create a semantically distinct Receiver Contract.

“Receiver-qualified” is a qualification rule over a Handoff return/projection:

A continuation is receiver-qualified when the material intended for the next logical role is directly usable by that role without requiring the human carrier to semantically transform it, and when the addressed receiver corresponds to the Handoff `To` or the declared completion `Return To`, as applicable.

Receiver qualification does not mean:

- the receiver accepted the handoff;
- the receiver executed the work;
- the receiver agreed with the result;
- the transport was delivered;
- the source role had authority beyond the controlling artifacts.

### 6. Practitioner specialization becomes first-class Role composition

Yes. `tiinex.party.role.v1` should now expose first-class machine-readable baseline composition because Business has accepted stable standalone Relation evidence for Anchor, Axiom, Loom, and Sigma and the same relation is now materially relevant to cross-role transport obligations.

The schema surface must project the same non-Parent relation already accepted in Business. It must not create inheritance of authority.

Canonical direction:

- specialized role -> Tiinex Practitioner baseline

Canonical relation type:

- `incorporates role baseline`

Canonical scope:

- shared working-method obligations, observation, friction detection, and continuous-improvement heuristics only

Authority rule:

- the baseline may constrain or add working-method obligations within the specialized role's existing boundary;
- it cannot widen `May Do`, delegation, representation authority, holder state, decision rights, publication authority, product acceptance, or any other authority omitted or forbidden by the specialized role;
- conflicts are resolved by preserving the specialized Role's explicit authority and responsibility boundary;
- Parent remains same-artifact/same-logical-role continuity only.

### 7. Exact schema amendment text: `tiinex.handoff.v1`

Axiom concludes that one schema amendment is required so explicit human semantic participation can be distinguished from ordinary courier transport without inventing a transport state machine.

In `### Handoff Body`, add:

```md
Optional Sections

- Participation Expectation
```

Add the following contract group after `### Handoff Parties` and before `### Transfers`:

```md
### Participation Expectation

Required Fields

- Human Participation
- Participation Meaning

Field Value Constraints

- Human Participation
  - Allowed Value: not-requested
  - Allowed Value: dialogue-requested
  - Domain Policy: closed

Rules

- `Participation Expectation` declares whether supporting human semantic participation is explicitly requested for this bounded Handoff; it does not identify physical transport mechanics.
- `Human Participation: not-requested` means the Handoff does not ask a human transport participant to interpret, summarize, decide, clarify, rewrite, or otherwise act as semantic middleware for the transfer.
- `Human Participation: dialogue-requested` means bounded human semantic participation is intentionally requested; `Participation Meaning` must state what observation, policy, priority, choice, clarification, decision, or other human contribution is requested.
- Human participation declared here does not transfer the Handoff work or responsibility to the human. If the human becomes the intended recipient of transferred work or responsibility, that party or role must be represented through the normal Handoff `To` endpoint.
- This section does not create a protocol state machine. Waiting or blocking remains represented through required-context availability and unresolved dependencies. Terminal closure remains represented through `Completion Expectation -> Signal Kind: none`.
- A human participant named or implied by this section does not thereby gain role-holding, delegation, representation, acceptance, publication, product, or decision authority.
- Additional durable participant identity or participation relations should be represented through Party, Role, Relation, Decision, Evidence, or another artifact that owns that truth.
- Absence of this optional section means only that human semantic participation was not explicitly declared in the Handoff artifact; validators must not infer historical dialogue or non-dialogue solely from transport behavior.
```

No Handoff field for attachment count, ZIP/package kind, code-block behavior, host rate limits, transport receipt, or acceptance is added.

### 8. Exact schema amendment text: `tiinex.party.role.v1`

Axiom concludes that first-class baseline composition is now required.

In `### Party Role Body`, extend `Optional Sections` to include:

```md
- Role Composition
```

Add the following contract group after `### Role Boundary` and before `### Authority And Responsibility Boundary`:

```md
### Role Composition

Entry Shape

- First-Level Hyphen List Item

Required Fields

- Baseline Role
- Relation Type
- Relation Direction
- Relation Scope

Optional Fields

- Baseline Role Reference
- Notes

Field Value Constraints

- Relation Type
  - Allowed Value: incorporates role baseline
  - Domain Policy: closed

- Baseline Role Reference
  - Allowed Shape: Markdown Link
  - Domain Policy: closed

Rules

- `Role Composition` declares typed non-Parent composition between the current specialized Role and a reusable Role baseline.
- `Baseline Role` identifies the reusable Role baseline being incorporated.
- `Relation Type` must be `incorporates role baseline`.
- `Relation Direction` must read from the current specialized Role toward the baseline Role.
- `Relation Scope` must state the bounded obligations or working-method semantics incorporated from the baseline.
- `Baseline Role Reference`, when present, is a resolution aid and must not override contradictory readable baseline identity.
- Role composition is not Tiinex continuity ancestry. It must not be represented through `Parent`.
- Incorporating a baseline does not widen the specialized Role's `May Do`, `Does Not Authorize`, holder state, delegation, representation authority, decision rights, publication authority, product acceptance, or other authority boundary.
- The specialized Role's explicit `Role Boundary`, `Authority And Responsibility Boundary`, `Holder Relationship`, and `Interpretation Limits` remain controlling for authority.
- A baseline may contribute working-method obligations, heuristics, or shared behavioral constraints only within the specialized Role's existing authority boundary.
- A standalone `tiinex.relation.v1` artifact may preserve the same relation when the relation instance has independent provenance, state, interpretation limits, or lifecycle worth preserving.
```

No Parent specialization or authority inheritance is introduced.

### 9. Durable Loom acceptance and qualification cases

Loom should later produce separate semantic and presentation-profile evidence. Passing host ergonomics must not be confused with passing Handoff semantics.

#### Semantic qualification cases

1. **ordinary receiver-qualified return — pass**
   - Handoff `To`: Axiom.
   - Human participation: `not-requested`.
   - Completion signal expects a result/return to Anchor.
   - Sender output contains a direct copy-ready continuation addressed to Anchor for the return leg.
   - Human-facing prose only instructs delivery and does not ask the human to summarize or reinterpret.

2. **courier used as semantic middleware — fail**
   - Completion `Return To`: Anchor.
   - Human participation is absent or `not-requested`.
   - Output only says, in human-facing prose, “tell Anchor that the work is done” or equivalent.
   - No receiver-qualified material for Anchor exists.
   - Required diagnostic: receiver qualification failure; human courier improperly required to transform semantics.

3. **explicit human dialogue — pass**
   - `Human Participation: dialogue-requested`.
   - `Participation Meaning` states the bounded question/decision/observation requested.
   - The visible response asks that bounded question directly.
   - No claim is made that the human thereby became the Handoff recipient or accepted transferred responsibility.

4. **blocked awaiting human input — pass as blocked, not complete**
   - Human dialogue is requested.
   - Required Context is unavailable/unresolved or an `unresolved-dependency` states that continuation depends on human input.
   - Output exposes the bounded question and does not claim completion.
   - Tooling reports blocked/unresolved from dependency facts rather than a new Handoff protocol state.

5. **terminal closure — pass**
   - `Completion Expectation -> Signal Kind: none`.
   - No receiver return is required.
   - Tooling does not require a copy-ready receiver block merely to satisfy a transport convention.

6. **delivery is not acceptance — pass only with non-overclaim**
   - A package/message is delivered to the declared `To`.
   - No separate acceptance evidence exists.
   - Tooling must preserve `delivered/transported` separately from `accepted`; it must reject an inferred acceptance claim.

7. **logical receiver mismatch — fail**
   - Handoff `To` or completion `Return To` names one role.
   - The generated receiver-qualified block is addressed to another role without a separately declared new Handoff/route change.
   - Tooling reports endpoint mismatch rather than silently rerouting.

8. **multi-human dialogue participation — pass**
   - Human dialogue is explicitly requested.
   - A durable Relation records one or more participants with `Relation Type: participates in handoff dialogue`.
   - Each participant relation is bounded to the dialogue and does not claim permanent identity, role holding, or authority.
   - If work/responsibility is actually transferred to one of those humans, a Handoff endpoint change/new Handoff is required.

9. **Practitioner specialization — pass**
   - Specialized Role has `Role Composition` pointing to Tiinex Practitioner with `Relation Type: incorporates role baseline`.
   - No Practitioner specialization uses Parent.
   - Specialized Role authority remains unchanged except for working-method obligations within its pre-existing boundary.

10. **authority inflation through baseline — fail**
    - Baseline composition is used to claim a `May Do`, delegation, holder, publication, product-acceptance, or decision authority absent from or forbidden by the specialized Role.
    - Tooling/validator reports authority overread.

#### Host/presentation qualification cases

These belong to a host profile or presentation qualification suite, not canonical Handoff validity:

- one attachment maximum per hop on the current preferred Access-Level-0 ChatGPT profile;
- package aggregation instead of many exposed internal attachments;
- short status outside code blocks;
- explicit human action, attachment link, and receiver text adjacent near the bottom;
- code blocks reserved for verbatim receiver text;
- TTS-sensitive ordinary status remains outside code blocks;
- attachment-rate limits are configurable host evidence, not hard-coded Tiinex semantics;
- a violation of these host-profile rules may fail the profile while leaving the underlying Handoff artifact semantically valid.

### 10. Multi-human participation

When the current human transport participant invites another human into an explicitly opened dialogue:

- preserve the Handoff logical `To` unless work/responsibility itself is transferred;
- record additional durable participation, when needed, as typed non-Parent Relation evidence;
- use a bounded textual participant descriptor when durable identity is unavailable or unnecessary;
- if a Party artifact exists, it may be referenced, but participation still does not prove Role holding or authority;
- if the new human is asked to make a decision, the decision authority must come from the relevant Role, Instrument, Decision, policy, or other controlling artifact, not from the participation relation;
- if the new human becomes the actual recipient of transferred work/responsibility, create or amend the Handoff endpoint under normal Handoff semantics rather than treating dialogue participation as transfer.

This allows multi-human dialogue without assuming permanent identity, organizational membership, role assignment, or authority.

## Basis

- `tiinex.handoff.v1` at Docs commit `3988951208eb9a8926e84ab42625d4b42fa00c2d` already makes `From` and `To` explicit, separates endpoint identity from capacity, states that physical ZIP/message transport is not a Handoff endpoint, separates required/reference context from transfer, and states that delivery does not prove acceptance or completion.
- The same Handoff schema already owns blocking-relevant facts through required-context availability and unresolved dependencies and already owns terminal/no-return semantics through `Completion Expectation -> Signal Kind: none`.
- `tiinex.relation.v1` explicitly exists for typed non-Parent relations and permits bounded textual targets when a durable Party artifact is unavailable.
- `tiinex.interaction.unit.v1` separates portable semantic interaction units from concrete UI components, and `tiinex.presentation.surface.v1` separates implementation-neutral presentation surfaces from framework/host implementation.
- The accepted Tiinex Practitioner Role establishes a provider-neutral shared human/LLM working-method baseline and says interface-specific presentation may differ without creating hidden parallel truth.
- Business already contains accepted standalone specialization Relation evidence from Anchor, Axiom, Loom, and Sigma to the Practitioner baseline using non-Parent composition.
- The prior Axiom Business disposition already rejected embedding transport-private package facts into visible semantic carrier artifacts and already accepted Practitioner specialization as a non-Parent relation.
- The observed malformed closure class is therefore best caught by receiver qualification plus an explicit human-participation exception, not by turning delivery into acceptance or Handoff into a transport state machine.

## Consequences

- Canonical Handoff semantics gain exactly one optional participation declaration and no transport-mechanics fields.
- Blocking remains dependency truth; terminal closure remains completion truth.
- No Human Transport Contract schema is created.
- No Receiver Contract schema is created.
- Receiver qualification becomes a Tooling/transport validation rule derived from Handoff semantics.
- `tiinex.party.role.v1` gains first-class baseline composition matching accepted Relation semantics.
- Practitioner/specialized Role material should be updated by its owner to make the mechanical-courier default and explicit-dialogue exception operationally legible.
- Host-specific attachment, layout, TTS, code-block, and rate-limit behavior remains in profile/presentation/tooling policy.
- Multi-human participation may be durable without becoming authority inheritance or permanent identity.
- Delivery, acknowledgement, acceptance, completion, correctness, and publication remain separate claims.

## Follow-up ownership

### Axiom

- Owns the exact Handoff and Role schema amendment text in this Decision.
- Owns later semantic correction if schema-authority review finds a contradiction with the pinned contracts.
- Does not claim implementation, repository mutation, publication, or cross-role acceptance.

### Anchor

- Review this disposition for cross-role architectural coherence.
- Route the two schema amendments through the schema-authority workflow.
- Update or route the Practitioner/role obligation wording so ordinary human transport is explicitly mechanical and human dialogue is an explicit exception.
- Keep the Human Transport Contract and Receiver Contract as named policy/qualification concepts rather than new authority-bearing artifacts unless later evidence proves a distinct semantic owner is necessary.
- Return implementation work to Loom only after the semantic amendments are accepted for implementation.

### Loom

- Implement parser/validator/projection support only after the semantic changes are accepted through the appropriate schema workflow.
- Produce the semantic fixtures and host-profile qualification evidence listed above.
- Keep semantic validity failures separate from host/presentation-profile failures.
- Do not infer acceptance from delivery or courier activity.
- Do not hard-code the observed ChatGPT numeric attachment-rate evidence as canonical Tiinex semantics.

### Sigma / human authority

- Supply bounded human observation and product/ergonomic acceptance for the courier-facing presentation profile.
- Confirm or revise host-profile preferences such as adjacency, verbosity, TTS accommodation, attachment aggregation, and observed rate-limit behavior.
- Supply decision authority only where a controlling Role/policy/instrument actually assigns it; ordinary transport participation does not create such authority.

## Review Conditions

Re-open this disposition only if qualified evidence shows one of the following:

- human semantic participation cannot be represented without transferring work/responsibility;
- existing dependency/completion semantics cannot truthfully represent blocking or terminal closure;
- Role baseline composition needs authority semantics beyond the explicitly non-Parent bounded model;
- multi-human dialogue requires a durable interaction-session artifact with independent lifecycle not representable by Handoff plus Relation;
- a host-independent transport concept emerges that cannot be represented as a presentation/qualification profile over existing semantic owners.

Do not reopen the already accepted separation between Handoff semantics and ZIP/package/private transport mechanics merely because a host UI changes.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: JXcGRTG-qo0sP48tlcPjTLcYDwEnsjYCiipWTXVH-4s
