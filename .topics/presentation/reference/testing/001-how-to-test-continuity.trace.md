# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 17:41:51
  - Trace: [001-presentation.trace.md](../../001-presentation.trace.md)
  - Origin:
    - [relative](../../001-presentation.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:51
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: Test matrix, measured limits and portable representation rationale.
  - Status: approved-for-publication

---

# How to test a Tiinex continuity claim

Earlier demonstrations included real viewer interaction, ZIP generation and fresh-entry experiments, but their outcomes remain bounded to specific hosts, context and available evidence. This document supplies a general review method rather than claiming that any one demonstration proves the whole system.

## Define the test before running it

Before testing, write down the claim, the environment, the expected outcome and what would count as failure. Keep the raw prompt, exact inputs, output artifact, version and human assessment together. A non-leading prompt is useful, but it **does not replace explicit pass/fail criteria**.

**Check 1 — Package integrity**

- **Setup:** Hold the package bytes fixed. Inspect its declared entry, root and route.
- **Failure or uncertainty:** A tampered package qualifies, or required evidence is missing but silently accepted.

**Check 2 — Cold entry**

- **Setup:** Use a fresh supported environment, the same transport guidance and no previous project narrative.
- **Failure or uncertainty:** The recipient invents context or permissions, or cannot locate the available evidence.

**Check 3 — Actual continuation**

- **Setup:** Give one authorized, bounded task and preserve the before-and-after artifacts.
- **Failure or uncertainty:** Incorrect Parent, mutated original source or unsupported authority claim.

**Check 4 — Cross-host portability**

- **Setup:** Repeat the *same scoped task* on a second genuinely supported host.
- **Failure or uncertainty:** Changed meaning, missing capabilities or incomparable setup hidden by a success claim.

**Check 5 — Warranted interpretation**

- **Setup:** Give reviewers the same evidence; ask them to distinguish observed facts from inference.
- **Failure or uncertainty:** Unsupported certainty, attribution mistakes or overlooked contradictory evidence.

**Result discipline:** Use **passed**, **failed** or **unverified**, with the exact observed basis. Missing tools or evidence mean **unverified**, never passed.

## What has and has not been proved

The linked [bounded Package V1 decision](https://github.com/Tiinex/business/blob/26e818e244ea096255ac621e6b6dece997649505/.topics/decisions/002-tooling-major-008-core-llm-direct-package-v1-freeze.trace.md) documents one important recipient/return qualification boundary. It is not proof that every model, host, malformed package, or semantic interpretation has passed.

## Markdown versus Python

Markdown carries readable source artifacts and declared relationships; JavaScript and Python are possible *mechanical* runtimes and validators. Replacing all Markdown with a Python data model would be a different design choice, not a requirement to use Python for the very act of storing portable prose. Schema-implementation parity must still be tested rather than assumed.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-presentation.trace.md](../../001-presentation.trace.md)
  - Value: rQAv5mT-ztwlZEsx6QN5VXKAPxNELbz64VSHsduTF_E

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: dUNUECO9lexNrE-rDc_cS4gCeECZ-ysZYpttw96STeQ
