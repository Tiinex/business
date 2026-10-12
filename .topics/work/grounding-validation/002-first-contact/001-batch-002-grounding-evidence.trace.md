# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.feedback.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/feedback/tiinex.feedback.v1.schema.md)
  - Created At: 2026-10-12 23:09:50
  - Trace: [001-1-batch-001-grounding-feedback.trace.md](../001-initial-testing/001-1-batch-001-grounding-feedback.trace.md)
  - Origin:
    - [relative](../001-initial-testing/001-1-batch-001-grounding-feedback.trace.md)
- Current
  - Current Schema: [tiinex.evidence.v1](https://github.com/Tiinex/docs/blob/9ef3c2caed38152b1948c93cb45c985786660d91/.topics/.schemas/core/evidence/tiinex.evidence.v1.schema.md)
  - Created At: 2026-10-12 23:10:08
  - Authors: Anchor
  - Summary: External batch 002 evidence and limits
  - Status: ready/local

---

# Grounding Test Batch 002 — Preserved Experimental Evidence

## Supported Claim Or Question

- Supported Claim Or Question: What does batch 002 actually demonstrate about grounding, qualified tool use, semantic judgment, and continuity?
- Evidence Role: tests and contextualizes the reported outcomes; not an acceptance record.

## Provenance

- Known Source: Sigma-supplied `002-completed-tests.zip` (locally available exact archive, 15711147 bytes, SHA-256 `973d334042c47418a848c096d4fad6d7e5c2ac597a9b889d576089ab891f2940`).
- Preservation Basis: Original batch archive is held separately from Tiinex Workspaces; Sigma additionally supplied a Google Drive archive link.
- Provenance Limits: Local ZIP SHA-256 and CRC were checked. The remote Google Drive bytes have **not** been independently fetched or compared. Assignment of this Drive link to batch 002 is inferred from the order of Sigma's three links and remains pending explicit verification. The archive may not preserve full platform-internal execution traces.

## Evidence Material

- Batch archive
  - Material: [Sigma's external archive candidate for batch 002](https://drive.google.com/file/d/1McSD782jm96kqQYUZtqM2erp5Pg_EdSn/view?usp=sharing)
  - Material Kind: application/zip (externally stored full test archive)
  - Description: Human first-contact / Viewer source-path review; six cold-start runs with two retros each.
- Locally checked reference identity
  - Material: `002-completed-tests.zip` — SHA-256 `973d334042c47418a848c096d4fad6d7e5c2ac597a9b889d576089ab891f2940`; exact local byte size `15711147`.
  - Material Kind: ZIP byte identity and checksum
  - Description: Identifies the verified local copy, not the as-yet-unverified remote Drive object.

## Preservation And Fidelity

- Preservation State: Preserved user-provided ZIP available outside Workspace lineages; an external Drive preservation location was supplied but not byte-qualified here.
- Fidelity Notes: The original local ZIP passed ZIP CRC verification; exact SHA-256 and byte size are recorded above.
- Known Losses: Any information omitted by the capture process (for example inaccessible platform-internal traces) remains unavailable, and the three Drive mappings have not been independently checked.

## Interpretation Limits

- Does Not Prove: That every reported model configuration executed exactly as selected, that semantic conclusions are correct, or that any task or human acceptance gate completed.
- Must Not Be Treated As: An independent evaluator's expected answer, permission to publish or edit other Workspaces, a raw ZIP imported into the codebase, or a replacement for the qualified carrier/Tooling route.
- Not Yet Used As: A governing acceptance or canonical result; this evidence is still subject to bounded assessment.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-batch-001-grounding-feedback.trace.md](../001-initial-testing/001-1-batch-001-grounding-feedback.trace.md)
  - Value: saU7SLO-GoVU6RNi4szdBuTprgjtyipVbI59uXLJxAg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: oDZAB5siSq2itDjRmNHDqRCQiYhZQ3BC3b5PJ_Ta8Co