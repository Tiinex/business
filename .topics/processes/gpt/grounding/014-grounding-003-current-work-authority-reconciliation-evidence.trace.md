# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-25 10:28:00
  - Trace: [012-2-1-1-anchor-to-anchor-prepare-return-source-authority-blocker-preserv.trace.md](012-2-1-1-anchor-to-anchor-prepare-return-source-authority-blocker-preserv.trace.md)
  - Origin:
    - [relative](012-2-1-1-anchor-to-anchor-prepare-return-source-authority-blocker-preserv.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-25 12:46:31
  - Authors: Anchor
  - Why: General Anchor succession exposed deterministic ambiguity between nearest-Task projection and exact selected-Handoff semantics; the defect and narrow repair must be durable before replay.
  - Summary: Record the independent two-replay Task 029 current-work conflict and the qualified selected-Handoff current-work authority repair.
  - Status: ready/local

---

# General Anchor Grounding — Current-Work Authority Reconciliation Evidence

## Supported Claim Or Question

- Supported Claim Or Question: does the routed grounding projection incorrectly promote the nearest nonterminal Task ancestor to current work when the exact selected Handoff explicitly controls different work artifacts?
- Evidence Role: independent two-replay diagnosis plus exact Core repair qualification.
- Supported Conclusion: yes. Two fresh Anchors independently reported the same conflict: the ground receipt promoted Task 029 as current work while the exact selected Handoff treated that Task as historical and transferred a different bounded blocker-preservation contract. The defect is now repaired so explicit selected-Handoff Controlling Artifact declarations determine current-work authority; nearest Task ancestry is context-only when it differs.

## Provenance

- Known Source: exact user-supplied two-replay silent video, exact `anchor-grounding-001-1-1-1-anchor-to-anchor.handoff-package.zip`, exact accepted frozen Core source reconstructed from `business-012-anchor-to-anchor.handoff-package.zip`, and deterministic post-repair test/black-box receipts.
- Preservation Basis: preserve the observed disagreement as a Tooling projection defect only; do not reinterpret source availability or defect identity beyond what the two fresh replays independently qualified.
- Provenance Limits: the replays establish deterministic current-work ambiguity, not a failure of Package V1 transport, Role authority, source-sufficiency semantics, or defect-root-cause identity.
- Controlling Handoff: [Prepare-Return Source-Authority Blocker Preservation Return](012-2-1-1-anchor-to-anchor-prepare-return-source-authority-blocker-preserv.trace.md).

## Evidence Material

- Material: exact replay outcomes, exact B-carrier grounding receipt before and after repair, repaired Core source/tests, and full gate receipts.
- Material Kind: independent behavioral diagnosis plus deterministic Core qualification.
- Replay A and Replay B both observed `currentWork.state = current-frontier-resolved`, Task 029 as the sole projected frontier, and `readiness.nextAction.target` pointing to Task 029.
- Both replays independently refused to classify Task 029 as unambiguously active because the exact selected Handoff and qualified Evidence/Decision material explicitly treated it as historical / not to be reactivated.
- Both replays independently classified authoritative current Core source/tests as not established / not carried / unresolved rather than positively absent.
- Both replays independently refused to qualify `endpoint.required` as the same defect as previously evidenced `endpoint-reference.required`; only repeated failure on the same bounded prepare-return surface was supported.
- Root cause in Tooling: current-work selection used nearest nonterminal Task Parent ancestry even when the exact selected Handoff declared explicit Controlling Artifact targets for different bounded work.
- Repair: selected-Handoff explicit Controlling Artifact targets now outrank nearest Task ancestry for current-work selection.
- If explicit controls resolve to exact-qualified nonterminal Task artifacts, those exact Tasks become the task frontier.
- If explicit controls resolve only to qualified non-Task artifacts, the selected Handoff itself is the bounded current-work contract and nearest Task ancestors remain context-only candidates.
- If any explicit current-work control target is unresolved, ambiguous, unqualified, or controls a Task that is not an exact-qualified nonterminal Task candidate, grounding fails closed rather than falling back to nearest ancestry.
- Compatibility: nearest Task ancestry remains available only when the selected Handoff declares no Controlling Artifact target.
- Exact B-carrier replay after repair: `readiness.state = grounded-to-act`; `currentWork.state = selected-handoff-bounded-work`; Task 029 appears only under context candidates; next action targets the selected Handoff.
- Full Core suite after repair: 274/274 tests passed.
- Portable smoke: passed.
- Embedded bootstrap qualification: passed.
- Retired Handoff Package V2 anti-drift: 3/3 passed.

## Remaining Unqualified Gates

- Run one fresh successor Anchor against a carrier built from the repaired Core and current Business grounding frontier.
- Confirm the fresh model no longer needs judgment to override a mechanically projected Task 029 frontier.
- Continue general Anchor succession testing only if that fresh replay is clean; do not reopen unrelated Core/Package V1 work.

## Preservation And Fidelity

- Preservation State: the original B carrier remains immutable behavioral evidence; the repair is carried only in a successor test carrier.
- Fidelity Notes: Package V1 shape, cache model, Role authority, source-sufficiency rules, carrier lineage and remote-write boundaries are unchanged.
- Known Losses: UI-level sandbox command expansion is not relied upon; diagnosis uses visible receipts, replay answers, exact carriers and deterministic Core tests.

## Interpretation Limits

- Does Not Prove: all general Anchor orchestration is complete, source authority is globally resolved, the two endpoint error strings are one implementation defect, or VS Code/reduction-redacting may begin.
- Must Not Be Treated As: permission to infer current work from arbitrary Handoff prose, filenames, lifecycle status alone, or nearest lineage position when explicit selected-Handoff control exists.
- Not Yet Used As: final general-grounding acceptance or authorization to open reduction/redacting or VS Code.
- Disposition: replay one fresh successor on the repaired carrier; if clean, resume multi-generation Anchor succession from the repaired grounding semantics.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [012-2-1-1-anchor-to-anchor-prepare-return-source-authority-blocker-preserv.trace.md](012-2-1-1-anchor-to-anchor-prepare-return-source-authority-blocker-preserv.trace.md)
  - Value: sgLCz_kQsS-Yuv_YeogOQRwaVu1zXg8Ynp9sH3VLG58

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: -LVXxgnKIlMRfm2Bt1EXML3ansdfLG6lb0FD1Nsc6Ro