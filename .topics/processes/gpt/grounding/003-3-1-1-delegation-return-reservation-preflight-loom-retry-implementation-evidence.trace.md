# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-13 13:27:24
  - Trace: [003-3-1-anchor-to-loom-delegation-return-reservation-preflight-enforcement-retry.trace.md](003-3-1-anchor-to-loom-delegation-return-reservation-preflight-enforcement-retry.trace.md)
  - Origin:
    - [relative](003-3-1-anchor-to-loom-delegation-return-reservation-preflight-enforcement-retry.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-13 13:39:14
  - Authors: Loom
  - Why: The retry delegation supplies the direct return reservation and exposes the receive-compatibility gap in the first Loom candidate.
  - Summary: Qualify preflight, legacy-carrier reservation recovery, continuation persistence, and exact reserved-return consumption.
  - Status: ready/local

---

# Delegation Return Reservation Preflight — Loom Retry Implementation Evidence

## Supported Claim Or Question

- Supported Claim Or Question: whether portable Tooling now enforces explicit expected-return reservation before dispatch, preserves that reservation across new and legacy package-v1 carriers, and consumes exactly the delegated non-Major sibling on direct return without allocation or Sigma repair
- Evidence Role: bounded Loom implementation and validation evidence for the Anchor → Loom retry delegation

## Provenance

- Known Source: qualified Business preflight contract, controlling Grounding Major 001 Task, retry Anchor → Loom Handoff with durable direct-return sibling reservation `1`, and the exact portable Tooling bootstrap carried by the retry package
- Preservation Basis: the previous Loom candidate was compared byte-for-byte against the freshly carried bootstrap, then corrected only where the retry exposed a receive-side compatibility gap; validation used the same portable Tooling package/orient/ground/handoff surfaces
- Provenance Limits: no canonical Docs schema or Business policy semantics were changed; no sibling index was discovered from filenames, neighboring packages, output directories, counters, or host state

## Evidence Material

- Material: portable Tooling detects `Completion Expectation / Signal Kind: return`; requires one explicit usable non-Major reservation in range `1..9999` or explicit Major return; rejects Major plus sibling conflicts; carries qualified reservations on newly manufactured Handoff route pointers; re-derives the durable `reserved-return-package-sibling-index` transfer from authoritative Handoff bytes when receiving an older carrier whose pointer lacks the new transport projection; persists the resolved reservation through `ground --continue`; and lets public `handoff` consume exactly that continued sibling when no current `--package-sibling-index` is supplied. Focused qualification produced: missing reservation → blocked with `portable.delegation-return-reservation.sibling-index.required`; explicit `12` → qualified; `10000` → blocked; explicit Major → qualified; Major plus sibling → blocked with `portable.delegation-return-reservation.major-index-conflict`; acknowledgement → not-required; durable retry transfer → qualified non-Major sibling `1`. All 15 modified modules passed `node --check`. Grounding the actual retry carrier with the candidate recovered continuation state `returnPackageCarrierKind: non-major` and `returnPackageSiblingIndex: 1` despite the incoming pointer being produced by older Tooling.
- Material Kind: exact portable Tooling candidate bytes plus focused qualifier checks and actual retry-carrier receive/ground evidence

## Preservation And Fidelity

- Preservation State: changes remain bounded to portable Tooling runtime code and this Business evidence artifact
- Fidelity Notes: reservation remains transport coordination metadata only; it does not create semantic Parent, Workspace, Role, acceptance, completion, provenance, or schema authority; missing reservation still fails closed; existing Major semantics remain explicit; public return manufacture consumes only the exact reservation carried by qualified continuation state
- Known Losses: no distributed allocator or local next-slot discovery mechanism exists or is implied; Anchor retains canonical integration/release disposition

## Interpretation Limits

- Does Not Prove: globally distributed uniqueness can be inferred locally, arbitrary missing reservations may be repaired, or transport metadata creates semantic authority
- Not Yet Used As: Anchor integration acceptance, canonical Core release, or Grounding Major 001 behavioral closure
- Must Not Be Treated As: permission to guess, increment, recycle, scan for, or silently replace sibling reservations

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [003-3-1-anchor-to-loom-delegation-return-reservation-preflight-enforcement-retry.trace.md](003-3-1-anchor-to-loom-delegation-return-reservation-preflight-enforcement-retry.trace.md)
  - Value: JGjtYXJJskqdukeX71K5Dy2FrTPYMWG9nsZ4zgIaZ5M

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 5ibdVRjJ5Dc09zkUb5GuUwQUhN9T4Ytkcs_QeWj-YqU