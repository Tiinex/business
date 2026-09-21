# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 17:27:25
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-kodax-to-anchor-extension-host-end-to-end-machine-gate-return.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-kodax-to-anchor-extension-host-end-to-end-machine-gate-return.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-kodax-to-anchor-extension-host-end-to-end-machine-gate-return.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-21 17:49:18
  - Authors: Anchor
  - Why: Sigma has the real VS Code execution capability missing from Kodax and Anchor, so the machine and human gates can be sequenced in one operator interaction without weakening either gate or inventing an intermediate transport format.
  - Summary: Run the remaining real-host machine gate first inside the same bounded Sigma operator interaction, stopping on the first blocker and continuing to human acceptance only after a complete machine PASS.
  - Status: ready/local

---

## Decision

- State: accepted
- Subject: Sequence the remaining real-host machine gate and Sigma human acceptance in one Sigma operator interaction
- Decision: authorize one bounded Anchor-to-Sigma gate in which Sigma first executes the repository-owned real VS Code machine acceptance on the exact carried candidate; any machine failure stops immediately and returns the first exact blocker without debugging or product mutation, while a complete machine PASS permits Sigma to continue directly into the human operator acceptance in the same interaction.

## Basis

- Kodax returned the complete repository-owned full-flow Extension Host harness and exact candidate source, while correctly preserving the machine disposition as blocked because its environment lacked a real VS Code CLI/runtime and lock-qualified dependency tree.
- Anchor review confirmed the harness now covers the required production command/controller path: pointerless Incoming boundary, Replace, Outgoing, invalid Attach rejection, exact participant-set weakening negative, two qualified Handoff attachments, Pack, Transport, and restart/requalification under both Local and Published Core modes.
- The remaining blocker is execution capability rather than an identified product-semantic gap.
- Sigma has access to the real VS Code operator environment needed to execute the final gate. Using that capability does not grant Sigma implementation authority.

## Gate Ordering

1. Machine phase: restore the exact lock-qualified Extension VS Code dependency tree from the carried candidate, run clean dependency-backed typecheck and repository/package regressions, then execute the repository-owned real Extension Host gate under both Local and Published Core with the exact carried accepted Local Core.
2. Fail-closed boundary: on the first machine failure, stop the gate. Preserve the exact command/stage and observable blocker; do not debug, patch, reinterpret, or continue into human acceptance.
3. Human phase: only after the complete machine phase passes, exercise the real VS Code operator workflow as Sigma and judge the product behavior against the controlling acceptance boundary.
4. Return: return either the first exact blocker or a bounded Sigma acceptance result to Anchor. No commit, push, release, publication, or product mutation is authorized by this gate.

## Authority Boundaries

- Sigma is operator/human acceptance authority for this gate, not implementation authority.
- The Handoff package, carried Workspaces, filenames, machine logs, and host UI do not create semantic authority beyond the controlling artifacts.
- A machine PASS is necessary but not sufficient for Sigma acceptance; Sigma must still perform the human operator phase.
- A machine failure is not a Sigma product rejection; it is a blocked gate requiring Anchor reconciliation.
- No synthetic, mocked, source-text-only, fixture-only, direct-Core, or dependency-free result may substitute for the real VS Code machine phase.

## Supersession Boundary

- This Decision revises only the sequencing constraint from the earlier Anchor machine-gate disposition that kept Sigma entirely excluded until a separately completed machine PASS.
- All technical Done Criteria, fail-closed requirements, product boundaries, and prohibition on synthetic PASS remain unchanged.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-kodax-to-anchor-extension-host-end-to-end-machine-gate-return.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-kodax-to-anchor-extension-host-end-to-end-machine-gate-return.trace.md)
  - Value: EcQiVIh2nC7KKnJyEiQ9uideNjFBHtHw6Q6C2h5SwsM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: EIWkIxhzvtotc9YaT9sZvcTwnFNL5wGuiY17XPub1sA