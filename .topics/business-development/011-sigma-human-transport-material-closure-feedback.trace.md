# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-08-27 23:14:00
  - Trace: [Axiom To Anchor Human Transport And Receiver Contract Semantics Return](../handoff/017-axiom-to-anchor-human-transport-and-receiver-contract-semantics-return.trace.md)
  - Origin:
    - [relative](../handoff/017-axiom-to-anchor-human-transport-and-receiver-contract-semantics-return.trace.md)
- Current
  - Current Schema: [tiinex.feedback.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/feedback/tiinex.feedback.v1.schema.md)
  - Created At: 2026-08-27 23:47:00
  - Authors: Sigma; Anchor
  - Why: Preserve Sigma's acceptance boundary after Axiom returned materially useful workspace state but used the copy-ready transport block as a second semantic context channel.
  - Summary: Human feedback that durable receiver context belongs in the carried workspace/package, while code blocks are only literal transport instructions and human-facing status cannot replace missing durable artifacts.
  - Status: accepted/local

---

# Human Transport Must Not Become A Second Context Channel

## Observed Signal

- Sigma accepted that Axiom had materially improved the return by carrying a Business workspace, durable Decision, Axiom-to-Anchor Handoff, and validation evidence.
- Sigma rejected the return transport presentation because its copy-ready receiver block repeated semantic interpretation, workspace-content summary, blocker detail, and continuation guidance that a receiver should obtain from the package itself.
- Sigma explicitly classified this as a transport failure even though the semantic work and carried material remained useful.

## Source

- Source: Sigma review of Axiom's 2026-08-27 workspace-bearing provisional return package and the human-visible return text emitted with it.
- Recorder: Anchor.

## Interpretation

- A copy-ready transport block is a literal ingress instruction, not a durable context artifact and not a fallback knowledge channel.
- The strongest qualification test is removal: if the receiver loses necessary semantic context after the receiver text is reduced to the package name, Start path, Continue-from path, and declared role/route instruction, the package is not self-contained enough for normal successful transport.
- Human-facing status outside a code block is allowed and useful, including a truthful blocker summary, but it does not cure missing durable workspace state.
- In the current ChatGPT host, keeping ordinary prose outside code blocks also preserves text-to-speech usefulness; that is presentation ergonomics, not semantic authority.

## Feedback Target

- Target: Human Transport / receiver-qualified Handoff projection and recipient-v2 package qualification.
- Related Semantic Disposition: [Human Transport And Receiver Contract Semantic Disposition](../decisions/002-axiom-human-transport-and-receiver-contract-semantics-decision.trace.md)
- Related Tooling Work: [Browser Companion And Bounded Human-In-The-Loop Transport](../initiatives/002-7-browser-companion-bounded-human-in-loop-transport-task.trace.md)
- Related Baseline: [Tiinex Practitioner](../roles/001-practitioner-role.trace.md)

## Feedback Received

- Source: Sigma
- Durable State Rule: attachment/package/workspace carries durable truth and continuation state.
- Copy Surface Rule: a code block is reserved for text intended to be copied verbatim to the next chat/role.
- Human Status Rule: short status may be presented outside the code block for the human transporter, but receiver-required context must remain durable inside the package/workspace.
- Detached Artifact Exception: one standalone Markdown result is acceptable when an already-grounded role is genuinely blocked before materialization/package manufacture or intentionally returns one bounded finding; it must not become the default closure for successful durable work.
- Cold-Start Rule: a cold recipient should normally receive a grounding-bearing workspace/package rather than an isolated result artifact.

## Disposition

- State: accepted as current Anchor/Sigma transport qualification feedback.
- Follow-Up: Anchor must carry this boundary into the next Business checkpoint and successor Handoff; Loom should later implement qualification/presentation behavior consistent with Axiom's semantic disposition and this human acceptance boundary.
- Failure Classification: Axiom's workspace-bearing provisional return is retained as useful material/provenance evidence, but its human transport emission is not accepted as a successful receiver-qualified presentation example.

## Limits

- This Feedback does not change Axiom's schema-semantic authority or claim that its Decision has already been implemented in Tooling.
- This Feedback does not require every status sentence to become a Tiinex artifact; only receiver-required semantic state must be durable.
- This Feedback does not turn code-block behavior, attachment placement, TTS behavior, or host file limits into canonical Handoff semantics.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Axiom To Anchor Human Transport And Receiver Contract Semantics Return](../handoff/017-axiom-to-anchor-human-transport-and-receiver-contract-semantics-return.trace.md)
  - Value: 8kETRGUl9pwb9XBv2japxSCfkHoZfb-B4bbkN3FU9eM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:pDmoeL1_JbS2r8ZOa9q7Ufhjhu4KXREqmEiRwFgsGpk
