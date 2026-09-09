# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-09 14:17:46
  - Trace: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Origin:
    - [relative](../001-turn-2-stable-full-source-frontier.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-09 16:47:24
  - Authors: Anchor
  - Why: Preserve provider-agnostic bootstrap and capability integration without making OpenAI or any other environment the generic Interop model.
  - Summary: Interop as namespace; interop-native as generic implementation; interop-openai as environment-specific augmentation.
  - Status: ready/local

---

# Native Interop repository frontier

## Objective

Treat Interop as an architecture namespace and `interop-native` as the first-party provider-agnostic implementation, while keeping environment-specific additions isolated.

## Repository identities

- `Tiinex/interop-native` / `@tiinex/interop-native`: generic bootstrap experience, grounding, external tool/capability contracts and automation integration.
- `Tiinex/interop-openai` / `@tiinex/interop-openai`: OpenAI-specific environment constraints, capability mapping, workarounds and optional grounding additions.

## Boundary

Generic Handoff/package mechanics remain in Core. Canonical semantic meaning remains with its owning Docs/semantic surfaces. Interop implementations may expose and adapt capabilities without becoming semantic authority.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Value: J7eMDpiRtxZpCqeB-lUxH-EtODAqs4XIYFcndqClJnI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: E_75-bJnUzn3grq_5lYrIaOUNSqkZP-oD_vonYRffHo