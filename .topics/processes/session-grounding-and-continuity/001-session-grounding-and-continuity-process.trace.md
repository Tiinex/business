# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Trace: [Processes](../001-processes.trace.md)
  - Origin:
    - [relative](../001-processes.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-04 02:24:00
  - Authors: Anchor; Sigma
  - Why: Let a cold Tiinex role enter or resume work without relying on hidden chat memory, transport accidents, or provider-specific improvisation.
  - Summary: Human-first process for session grounding, Handoff/carrier continuity, explicit process applicability, host adaptation, and readiness disposition.
  - Status: ready/local

---

# Session Grounding And Continuity Process

## Purpose

Establish enough qualified context to begin or resume bounded Tiinex work safely, and preserve that context before a volatile host or long session can become the only copy of important state.

The process is intentionally readable without knowing a specific runtime. Tooling may automate it, but Tooling does not replace the semantic authorities named here.

## When This Process Applies

Use this process when a Tiinex session is cold-starting, resuming from a Handoff or carrier, entering work after a material context change, or approaching a host/session boundary where important local state may not survive.

A concrete Session Entry may name this Process and other required Grounding Material. Process inventory, file proximity, package membership, or Role carriage alone do not make a Process applicable.

## Grounding Sequence

1. **Identify the entry boundary.** Determine whether the session is entering through a formal Handoff, an informal continuation, a Workspace/Project frontier, or another explicit Entry. Do not manufacture transfer authority from transport delivery.
2. **Ground the recipient and current work.** Read the exact Role, Handoff, Task/Project, Decision, Evidence, Process, and Workspace material required by the entry boundary. Preserve unknowns instead of filling them from chat intuition.
3. **Ground the applicable process.** Use explicit semantic authority such as the Session Entry, controlling work, Handoff, Decision, or another qualified declaration. A catalog shows what exists; it does not decide what applies.
4. **Prefer carried qualified material.** Resolve required material from the carried Workspace/package representation before using an external repository or connector. External recovery is for material that is not carried, cannot be qualified locally, or is explicitly declared external.
5. **Apply host adaptation only after portable meaning is clear.** Provider-, application-, filesystem-, model-, or session-specific behavior belongs to the relevant Interop/host domain. Core remains host-neutral and must not absorb one provider's operating quirks as portable Tiinex semantics.
6. **Disposition readiness explicitly.** State what the session is ready to do and what is still blocked. Do not collapse transport validity, grounding, and mutation authority into one word.
7. **Checkpoint before survivability becomes uncertain.** When important progress exists and the host/session may lose local state, create a qualified carrier/checkpoint on a durable transport surface before continuing deep work.

## Readiness Ladder

Use the smallest truthful readiness state:

- **Carrier qualified:** the transport/package can be inspected and its declared carriage is qualified. This does not prove the recipient understands or may act on the work.
- **Recipient grounded:** the intended recipient Role/capacity, transfer boundary when present, and session-holder relationship are sufficiently qualified for the current session.
- **Semantically grounded:** current work, required context, applicable Process, relevant Workspace boundaries, and material source identities are sufficiently qualified to understand the next bounded action.
- **Grounded to act:** the next bounded local action is authorized and its required evidence is available.
- **Remote mutation authorized:** a separate explicit authority permits the named remote mutation. No connector, repository login, package delivery, or `grounded to act` state grants this by itself.

A later state requires the earlier truths that matter to that action, but these labels are not a protocol state machine and do not replace the controlling artifacts.

## Handoff And Carrier Boundary

- **Handoff** declares a bounded transfer of work or responsibility.
- **Handoff Package / carrier** transports qualified material and may preserve a session checkpoint.
- A carrier may exist without a new responsibility transfer.
- Package validity does not prove Handoff acceptance, semantic grounding, or action readiness.
- Handoff responsibility must not be inferred from package destination, chat sender/receiver, filename, directory, or upload channel.

## Source Preference And Recovery

For required material, prefer this order when each earlier source is qualified and sufficient:

1. carried qualified Workspace material;
2. carried route/cache or other qualified carrier-local representation;
3. explicit immutable recovery material;
4. live external source/connector access.

Moving to a later source is a recovery decision, not a convenience shortcut. A live source may be fresher but must not silently replace the exact material that the controlling Handoff/Task/Decision intended.

## Host And Interop Boundary

Portable Tiinex meaning belongs in the semantic owner and shared host-neutral mechanics belong in Core. Environment-specific behavior belongs in the relevant Interop or host Workspace.

A host-specific profile may define, for example, volatile-storage behavior, attachment survival, connector limitations, UI constraints, capability names, or provider-specific workarounds. Such a profile must preserve the portable process instead of redefining Handoff, Parent, Role, Process, Workspace, or carrier semantics.

Host capabilities are permissions/opportunities, not semantic authority. In particular, read capability does not imply write authority and remote write requires an explicit bounded authorization.

## Lineage And Continuity Separation

Keep these concerns separate during grounding and checkpointing:

- artifact identity describes the artifact itself;
- Parent describes semantic continuity ancestry;
- filename/dimension provides local navigation/allocation coordinates;
- carrier lineage describes transport/checkpoint continuity.

A matching number, directory, package dimension, or arrival order must never be used to infer one of the other relationships.

## Anchor Readiness Disposition

When Anchor is the active orchestration Role, Anchor owns the readiness disposition for the bounded work: proceed, proceed with an explicit limitation, or stop with an exact blocker.

Sigma or another human may provide intent, feedback, acceptance, or required human action, but should not have to act as hidden memory or independently prove that Anchor is grounded.

## Checkpoint Boundary

A useful checkpoint preserves enough qualified material and routing information that a cold successor can recover the current bounded state without reconstructing it from conversational chronology.

Checkpoint frequency is driven by survivability risk and meaningful progress, not by a fixed number of messages. A host-specific profile may define stricter practical triggers.

Carrier progression is transport continuity only. It must not rewrite Parent ancestry, artifact identity, filename lineage, acceptance, or work ownership.

## Failure Policy

Stop the stronger action when a required grounding obligation cannot be qualified. Name the missing material or authority, why it matters, and the smallest recovery path.

Do not compensate by broad repository archaeology, arbitrary connector search, guessed participant identity, guessed Process applicability, or invented structural placement.

## Interpretation Limits

- Does Not Establish: Handoff acceptance, durable Party identity, process execution, Task completion, semantic truth, remote-write authority, or universal applicability of any carried Process/Role/Scaffold.
- Must Not Be Used To Claim: that package validity equals readiness; that a carried Role is a participant; that a carried Parent target should be fetched remotely again; that provider-specific constraints belong in Core; or that transport/carrier lineage creates semantic Parent ancestry.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Processes](../001-processes.trace.md)
  - Value: 894_R-4DZE3RsHODoloOXj00yq9YAvOSDFA_3iwmBgc

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:t-2I0DOB7QvCRzZPVB16XXvvo5LUqOHfFJFduZgIpok
