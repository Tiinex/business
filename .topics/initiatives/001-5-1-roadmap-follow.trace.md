# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 13:01:00
  - Trace: [Tiinex Roadmap](001-5-roadmap.trace.md)
  - Origin:
    - [relative](001-5-roadmap.trace.md)
- Current
  - Current Schema: [tiinex.discovery.follow.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/discovery/follow/tiinex.discovery.follow.v1.schema.md)
  - Created At: 2026-08-29 13:12:00
  - Authors: Anchor; Sigma
  - Summary: Bounded follow for resolving current Roadmap phase, linked work state, blockers, and phase-gate evidence without duplicating Epic status into the Roadmap.
  - Status: draft/local

---

# Tiinex Roadmap Follow

## Follow Target

- Target: [Tiinex Roadmap](001-5-roadmap.trace.md), its current phase, the phase-gate authority, and the work artifacts explicitly linked by the Roadmap.
- Current Focus: resolve the **Now** phase first; later phases are planning context unless their work becomes active or the Roadmap itself changes.

## Follow Basis

- Basis: the Roadmap owns sequencing, but execution truth belongs to the linked Project/Epic/Task/Resource artifacts.
- Need: a manager, CEO, sponsor, contributor, or LLM should be able to ask “how is the roadmap going?” without maintaining a second status table that can become stale.

## Interest Boundary

- Interested In: current phase, linked work-package status from each owning artifact, explicit blockers/holds, unresolved external obligations, phase-exit criteria, acceptance/validation evidence, and materially changed resource dependencies.
- Not Interested In: copying implementation subtasks into Business, inferring progress percentages, general repository churn, unrelated technical detail, or rewriting linked artifact state into this Follow.
- Authority Boundary: this Follow observes and projects. It does not become authority for the status of any linked work package and does not replace the Roadmap's sequencing authority.

## Update Expectation

- Expectation: on-demand/manual bounded resolution while exact Roadmap-Follow execution support is incomplete.
- Future Capability: a qualified resolver may follow the Roadmap's declared links, read each owning artifact's current state, and produce a fresh phase roll-up without editing either the Roadmap or this Follow.
- Desired Projection: show current phase, linked work grouped by their authoritative state, blockers needing attention, unresolved phase-exit evidence, and direct paths back to every source artifact.
- Freshness: every generated projection should disclose when it was resolved. A previous projection is evidence of a previous observation, not durable current status.

## Roadmap Status Ownership Rule

- Roadmap owns: phase membership, ordering, phase purpose, and exit intent.
- Linked work artifacts own: execution status, owner, blocker, detailed next step, acceptance criteria, and completion evidence.
- Follow owns: the bounded question and method for resolving those authorities into a current management view.
- Validation/acceptance owns: whether a phase gate may actually be treated as passed.

A linked Epic or Task changing state therefore requires **no Roadmap edit**. The Roadmap changes only when the plan itself changes.

## Stop Or Review Condition

- Review: re-resolve when a linked work artifact materially changes, a blocker or external obligation changes, Foundation acceptance is reviewed, or the Roadmap adds/removes/reorders work.
- Phase Transition: when the current phase gate is accepted, resolve the Roadmap again and shift the Follow's operational attention to the newly current phase; do not infer the transition merely from all visible work appearing complete.
- Stop: this Follow may close if the Roadmap is retired/replaced or a successor follow explicitly takes over the same bounded management question.

## Interpretation Limits

- A Follow projection is not a release claim, accounting record, delivery forecast, percentage-complete calculation, or substitute for opening the linked artifacts.
- “Done-looking” linked work does not itself close a phase; the declared exit gate and required human/validation acceptance still apply.
- Missing or unavailable linked evidence must be shown as unknown/degraded rather than guessed from filenames, Git activity, or neighboring artifacts.
- This Follow must not materialize hundreds of technical subtasks into Business merely to make the roll-up look complete.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Roadmap](001-5-roadmap.trace.md)
  - Value: jj1qLgoL2wZPyT25H26aO0Y03DYuZz2OjeJOFjoYX9o

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:RXmA-vFQnHCVlfgM_mB7_htuHxv4hqg7UwDaZoTaFCA
