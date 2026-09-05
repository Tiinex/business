# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-06 00:12:00
  - Trace: [Generate Bounded Visual Source Candidate](004-1-1-generate-bounded-visual-source-candidate.trace.md)
  - Origin:
    - [relative](004-1-1-generate-bounded-visual-source-candidate.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-06 00:13:00
  - Authors: Anchor; Sigma
  - Why: Preserve one coherent accepted source boundary instead of allowing later local repair to silently redefine generated identity or composition.
  - Summary: Process step for atomically rejecting a source candidate or freezing the exact accepted source bytes.
  - Status: candidate/local

---

# Accept Or Reject And Freeze Visual Source

## Current Read

A generated candidate is either rejected as source or accepted as one frozen source boundary. Acceptance means the exact bytes become the canonical input for deterministic downstream work; it does not mean every derived asset, interpretation, or product use is accepted.

## Design Direction

Record source identity, provenance, acceptance boundary, and known limitations. Avoid per-region or per-frame generative rescue after acceptance when that would create a mixed source whose coherence and provenance are no longer judgeable as one candidate.

## Next Artifacts

- [Deterministically Transform Frozen Visual Source](004-1-1-1-1-deterministically-transform-frozen-visual-source.trace.md)

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Generate Bounded Visual Source Candidate](004-1-1-generate-bounded-visual-source-candidate.trace.md)
  - Value: r5hXzEh_GWOM_Og7wEC0K9Rwy1rtSN1LePz8k_BAt4w

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:RSRJh_roAfVMJ1OsGzegJwQEQcXOSP0U0VZb69ZH1Rw
