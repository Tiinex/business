# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Tooling](002-tooling-project.trace.md)
  - Origin:
    - [relative](002-tooling-project.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-27 12:26:00
  - Authors: Anchor; Sigma
  - Why: Preserve the agreed transport-access ladder so browser assistance, manual transport, and authenticated connectors can evolve without conflating convenience, authentication, delegation, or authority.
  - Summary: Tiinex transport uses three bounded access levels: manual unauthenticated Level 0, user-approved semi-automatic browser-assisted Level 1, and explicitly authenticated connector/API Level 2.
  - Status: accepted/local

---

# Transport Access Level Model Decision

## Decision

- State: accepted
- Subject: Tiinex transport and host-access capability levels
- Decision: Use a three-level access model. Level 0 is manual transport plus unauthenticated/public reads and fetches. Level 1 is assisted or semi-automatic operation through a user-controlled local/browser adapter under an explicit bounded delegation; it may observe and perform only the approved interaction class, must not automatically route to a human role, and must stop after the configured turn/transition budget or earlier on ambiguity, policy, authority, or safety boundaries until the human actively reauthorizes. Level 2 uses explicitly authenticated APIs/connectors or equivalent authorized adapters and only the exact authority actually granted. Access level describes available transport/access capability, not trustworthiness, role seniority, correctness, or permission to exceed the governing artifact/role boundary.

## Basis

- Manual Handoff transport is reliable but creates repeated human friction and does not scale well across parallel non-human role work.
- A browser extension can operate inside a user-controlled session and improve ergonomics without implying the broader authorization semantics of an authenticated API integration.
- Authenticated APIs/connectors have materially different authority and audit characteristics and should therefore remain a distinct level.
- Human-in-the-loop automation is safest and most legible when delegation is explicit, bounded, expiring, and interruptible rather than represented as a global agent-mode toggle.

## Consequences

- Browser Companion work is Level 1 by default and must implement visible delegation budgets and circuit breakers.
- Level 1 may observe authenticated browser UI state only within the user-approved local adapter boundary; it must not reinterpret ambient browser login as general Level 2 API authority.
- Future transport adapters must state their access level and any narrower capability/authority boundary explicitly.
- The access ladder may be refined from real adapter evidence, but any change that widens automatic authority requires a new explicit Decision rather than silent implementation drift.

## Review Conditions

- Review after the first Level-1 browser implementation produces real user/host evidence.
- Review before any adapter claims a new capability that does not fit Levels 0–2 cleanly.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Tooling](002-tooling-project.trace.md)
  - Value: ttGDyrDpEo9mqBL7armC42aip4IaNFsx2NjAVwTP66Y

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:dLhgs_knwsTDvp5UmC685rkboajZsWWpx70_lWkvMGg
