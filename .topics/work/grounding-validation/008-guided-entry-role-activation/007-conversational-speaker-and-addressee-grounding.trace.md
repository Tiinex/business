# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-12 23:07:16
  - Trace: [001-grounding-validation-and-acceptance.trace.md](../001-grounding-validation-and-acceptance.trace.md)
  - Origin:
    - [relative](../001-grounding-validation-and-acceptance.trace.md)
- Current
  - Current Schema: [tiinex.evidence.v1](https://github.com/Tiinex/docs/blob/9ef3c2caed38152b1948c93cb45c985786660d91/.topics/.schemas/core/evidence/tiinex.evidence.v1.schema.md)
  - Created At: 2026-10-19 12:12:53
  - Authors: Anchor (bounded explicit-session)
  - Why: Ground low-risk contact inference without creating semantic holder authority
  - Summary: Local target regression for participant addressing, speaker swaps and Handoff sender fallback
  - Status: ready/local

---

# Conversational Speaker And Addressee Grounding — Local Evidence

## Supported Claim Or Question

- Supported Claim Or Question: Can a ChatGPT Web receiving session route conversation to the most relevant participant without treating role order, message prefixes, or formal Handoff sender labels as semantic role-holder/participant authority?
- Evidence Role: Bounded host-adaptation and manual source/test evidence; separate independent ChatGPT Web receiver acceptance remains open.

## Provenance

- Known Source: Exact `tiinex-028-1-1-1-1-1-1-1-1` pointerless carrier, direct Start read, checksum-verified embedded bootstrap, `orient` and `orient --full` showing 18/18 qualified Workspaces; carried Business Anchor/Sigma Role materials; Core Guided Entry participant projection; Interop OpenAI ChatGPT Web Target.
- Governing Work: Existing Business Grounding And Continuity Readiness Project and Grounding Validation And Acceptance Task. Interop OpenAI owns target-local conversation presentation; Docs continues to own canonical holder and Handoff semantics; Core and VS Code explicit operator binding remains unchanged. No new owner, Role schema, Task, Workspace, sidecar or JSON artifact is introduced.
- Preservation Basis: Requalify existing ChatGPT Web Target at the same path using `author --preflight` and `author`, extend the existing target-instructions contract test, preserve unchanged other Workspace snapshots in a full pointerless successor carrier.
- Provenance Limits: This is a local host-target source and test claim. It does not demonstrate model compliance in a new GPT Web conversation, human acceptance or installed VS Code host behavior.

## Evidence Material

**Observation:** Sigma reports that normally the first Participant Role is the human chatting; others may be relayed through that contact or join with identity-prefixed messages. In a formal Handoff, a qualified sender Role may be the conversational contact when no Participants are declared. Previous transport requires explicit operator-participant binding for semantic participation, which is correct for authority but leaves ordinary addressee and multi-speaker conversation guidance under-specified.

**Correction:** The existing ChatGPT Web Target now states a conversation-routing precedence: an explicitly qualified operator-participant binding is first; live explicit self-identification or unquoted Role prefix is a conversational speaker cue, not a holder assignment; absent those, first selected Participant is tentative primary addressee only; for a selected formal Handoff without Participant selection, qualified `From` may be a tentative conversational fallback; otherwise speak neutrally. Preserve speaker cue between turns until superseded or corrected; never promote quoted/forwarded text, inferred ordering, transport metadata, sender Role or prefix into durable identity, Handoff acceptance, Task authority or remote permission. For decisions with authority impact seek independent binding, but avoid repeated confirmations for ordinary status.

**Local directed test:** `node --test test/target-instructions.contract.test.mjs` in carried Interop OpenAI Workspace passed 4/4, including a contract regression for first-participant contact, formal qualified `From`, speaker swap, quotes, and explicit authority separation. The exact Target Role was requalified at its existing path with zero preflight errors and verified self-integrity.

**Expected receiver behavior:** A fresh ChatGPT Web session with explicit operator Sigma should address Sigma and conserve communication load; if Sigma is selected only as the first Participant, it should use Sigma as a tentative conversational point of contact without claiming the human actually holds Sigma. An unquoted `Axiom:` in a later message should change the address/speaker context but not Role holder authority. Formal Handoff sender fallback must remain conditional on selected qualified `From`. Do not treat an incoming Role-prefixed quotation as a speaker change.

## Preservation And Fidelity

- Preservation State: Local qualified Interop OpenAI Target update and its existing test, plus Business Evidence under current acceptance Task. Intended complete carrier to preserve all 18 prior Workspaces.
- Fidelity Notes: No change to Core role assignment, VS Code operator choice, canonical Docs Assignment Modes or formal Handoff Pointer sibling semantics.
- Known Losses: No new live GPT Web receiver behavioral acceptance; rule implementation is a grounded host-target instruction and not a deterministic speaker-authentication mechanism.

## Interpretation Limits

- Not Yet Used As: Sigma final approval, durable participant holder assignment, formal Handoff transfer, or publication to remote sources.
- Does Not Prove: that a tentative conversational contact is the actual person typing or that a message prefix is authorization to decide or mutate.
- Must Not Be Treated As: extra Handoff authority or a replacement for qualified Role/Task/Process grounding.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-grounding-validation-and-acceptance.trace.md](../001-grounding-validation-and-acceptance.trace.md)
  - Value: EQCmmsJdhNwzxbzRoaT82XPMIRujdkIw4q9VFQ-UCTY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: ac-xyEIJjn3IjAvf3SXztrfNfDrABe5UmzBrhuipNJk