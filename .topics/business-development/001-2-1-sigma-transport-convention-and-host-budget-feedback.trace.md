# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/8f568f14658a48500e2fa4d0d72a58620eaae759/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.feedback.v1](https://github.com/Tiinex/docs/blob/8f568f14658a48500e2fa4d0d72a58620eaae759/.topics/.schemas/core/feedback/tiinex.feedback.v1.schema.md)
  - Created At: 2026-08-31 00:18:00
  - Trace: [Sigma Foundation Workflow Feedback](001-2-sigma-foundation-workflow-feedback.trace.md)
  - Origin:
    - [relative](001-2-sigma-foundation-workflow-feedback.trace.md)
- Current
  - Current Schema: [tiinex.feedback.v1](https://github.com/Tiinex/docs/blob/8f568f14658a48500e2fa4d0d72a58620eaae759/.topics/.schemas/core/feedback/tiinex.feedback.v1.schema.md)
  - Created At: 2026-08-31 21:00:00
  - Authors: Sigma; Anchor
  - Why: Make transport-shape consistency and the observed host execution budget hard Foundation workflow inputs instead of repeatedly relearning them after broken cold starts.
  - Summary: Sigma feedback requiring one recognizable Tiinex transport convention, ZIP-bounded physical carriage, and iteration-efficiency work that keeps ordinary role turns away from repeated host-checkpoint exhaustion.
  - Status: accepted/local

---

# Sigma Transport Convention And Host-Budget Feedback

## Observed Signal

- Repeated cold-start and return failures are eroding workflow trust because physically similar deliveries have represented different semantics: canonical Tiinex carriers, Site-only carriers, loose durable records, and arbitrary ZIP wrappers have all appeared during the same Foundation collaboration.

## Source

- Source: direct Sigma workflow observation during repeated Anchor/Loom transport attempts and ChatGPT-hosted role turns on 2026-08-31.

## Interpretation

- Interpretation: transport consistency is an A-and-O Foundation requirement for human legibility. Another human should be able to recognize the same routine from every role-to-role delivery without learning hidden exceptions from chat history.

## Feedback Target

- Target: Foundation inter-role Handoff transport convention, cold-start/bootstrap qualification, validation/test orchestration, and Anchor/Loom pre-send behavior.

## Feedback Received

- Canonical transport shape: a ZIP is not a Tiinex transport merely because it contains an instruction or artifact. A role-to-role delivery represented as transport must use the canonical Tiinex Handoff-carrier structure and routing convention.
- Human recognizability: transport conventions and deliveries must not be mixed in ways that force a new human reader to infer which ZIP shape is routine and which is an exception.
- Physical upload boundary: one logical role-to-role transport should normally require one uploaded ZIP. This is operationally important because the current host imposes a finite attachment allowance; Tiinex must not require dozens of separate source-file uploads for one logical turn.
- Non-transport boundary: a plain instruction, feedback note, patch note, or other loose artifact may be useful, but it must remain visibly non-transport and must not be wrapped in a ZIP and presented as if it were a canonical Handoff package.
- Pre-send expectation: Anchor and specialist roles should qualify the carrier through canonical Tooling before exposing it to the human transporter. Transport-format correctness must be checked before handoff rather than discovered by the next cold start.
- Full-source Foundation continuity: the existing Business Cross-Repository Work Turn 3/3 rule remains the current Foundation operating invariant. A narrow work scope does not justify a narrow carrier when the process requires complete Business, Docs, and Site source.
- Major-bump expectation: a major carrier bump requires full-source plus stable qualification. Retry/progression suffixes must preserve continuity without inventing a new semantic major merely because transport failed.
- Host timing observation: ordinary productive work is generally expected in roughly the 1–10 minute range. Turns stretching beyond roughly 20 minutes have repeatedly coincided with additional host safety-checkpoint friction, and affected runs have been observed to lose useful continuation budget around 25–26 minutes.
- Safety boundary: these timings are observations, not authority to bypass or evade host safeguards. The preferred response is to reduce Tiinex-owned repeated test cost, false-positive host-sensitive test shapes, broad automatic validation, and avoidable bootstrap/manufacture retries.
- Loom priority: first reduce tests that repeatedly create unnecessary host-checkpoint pressure while preserving the actual invariant; second minimize ordinary automatic validation to a small meaningful regression spine; third make bootstrap/manufacture deterministically preserve ZIP shape, role material, role relations, workspace closure, and predecessor continuity.
- Parallelism: independent efficiency/transport lanes may proceed in parallel when they remain independently returnable and do not require one broad atomic refactor.

## Disposition

- State: accepted
- Follow-Up: Anchor treats canonical carrier qualification as a hard pre-send gate and routes the test/profile/bootstrap efficiency work to Loom before the remaining large static-debt tranche. Any recovery exception must remain explicitly labeled as recovery while preserving the same canonical outer transport shape.

## Limits

- Fidelity: condensed durable summary of Sigma's direct statements and screenshots from the active collaboration.
- Boundary: the host timing observations do not prove internal safety-trigger logic or a guaranteed timeout. This feedback does not authorize safety bypass, weaker semantic validation, or labeling an arbitrary ZIP as a Tiinex carrier.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Sigma Foundation Workflow Feedback](001-2-sigma-foundation-workflow-feedback.trace.md)
  - Value: NBeR7FsrkElEfzlQoUZE1dU9TPJthmtiidzD7eeK77g

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:zdiSNiVXYtTM98FZC1JqotRDZJU7e4Px6dbtqNVj518
