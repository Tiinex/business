# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-13 16:35:37
  - Trace: [001-1-2-loom-to-anchor-recovery-major-001-recovery-integrity-return.trace.md](../001-1-2-loom-to-anchor-recovery-major-001-recovery-integrity-return.trace.md)
  - Origin:
    - [relative](../001-1-2-loom-to-anchor-recovery-major-001-recovery-integrity-return.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-13 18:11:15
  - Authors: Anchor
  - Why: The two qualified branches were missing from the prior salvage checkpoint and must be integrated without regressing either return-reservation or Recovery WIP-protection behavior.
  - Summary: Qualify the non-overlapping Grounding/Recovery Core reconciliation and broad validation before the next Full Recovery.
  - Status: ready/local

---

# Recovery Major 001 + Grounding Tooling Reconciliation Evidence

## Supported Claim Or Question

- Supported Claim Or Question: whether the independently qualified Grounding return-reservation Tooling branch and Recovery Major 001 WIP-protection/acceptance-audit branch can be reconciled without losing either behavior and with broad Core validation green
- Evidence Role: Anchor integration evidence for the new Full Recovery checkpoint

## Provenance

- Known Source: prior stable reconstructed Full Recovery Core snapshot, qualified Loom Recovery Major 001 return carrier, qualified Fresh Anchor succession return carrier, and exact common pre-branch Core snapshot recovered from qualified earlier carrier material
- Preservation Basis: the Grounding and Recovery branches were compared against the same common Core basis; branch deltas were applied only where they differed from that basis, and overlapping changed/added paths were byte-identical
- Provenance Limits: no VS Code candidate bytes were promoted; no historical Business artifact was deleted; this evidence covers the Core branch reconciliation and recovered Business return artifacts only

## Evidence Material

- Material: the Grounding branch added six paths and changed fourteen Core paths relative to the common basis; the Recovery branch added six paths and changed twelve Core paths. The only five overlapping branch paths were byte-identical. The reconciled Core therefore preserves `delegationReturnReservation.js` and adds `recoveryAcceptanceAudit.js` plus the Recovery landing-preflight changes. One unrelated bounded-carrier regression fixture was re-scoped from `Signal Kind: return` to `Signal Kind: acknowledgement` because that test exercises bounded carrier isolation rather than return transport; the explicit return-reservation behavior remains covered by its dedicated tests. `npm run validate` on the exact reconciled Core completed 106/106 Node tests, portable smoke, and embedded bootstrap verification with zero failures.
- Material Kind: exact three-way source-frontier comparison, deterministic non-overlap reconciliation, one test-fixture scope correction, and broad Core validation

## Preservation And Fidelity

- Preservation State: both qualified Tooling behaviors are present in the reconciled Core source; no branch deletion was applied; recovered Fresh Anchor and Recovery Major Business artifacts are added to the prior stable Business snapshot without treating branch-absent files as deletions
- Fidelity Notes: the prior stable Extension VS Code snapshot remains unchanged because the latest Kodax carrier is still live-gated and unaccepted
- Known Losses: the latest VS Code candidate remains a separate qualified carrier rather than accepted Full Recovery source; Grounding Mode-B stewardship remains an open behavioral proof rather than being invented as closed

## Interpretation Limits

- Does Not Prove: that VS Code 003 is accepted, that every historical Hygiene warning is repaired, or that a divergent developer checkout may be overwritten by Recovery
- Not Yet Used As: release/publish authority or permission for destructive landing
- Must Not Be Treated As: semantic authority to rewrite independent repository history

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-2-loom-to-anchor-recovery-major-001-recovery-integrity-return.trace.md](../001-1-2-loom-to-anchor-recovery-major-001-recovery-integrity-return.trace.md)
  - Value: m5FfQuKjw0oR2wfJUJl_6S8GKHBVBFdVpnATGGez4m4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: yW2MSDftpVx5w7p9lYp1bn4coR9I0vQB9sSm78C_fD4