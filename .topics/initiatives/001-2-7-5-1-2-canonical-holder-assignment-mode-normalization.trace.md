# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 11:45:02
  - Trace: [001-2-7-5-1-blank-workspace-qualified-delegation-acceptance.trace.md](001-2-7-5-1-blank-workspace-qualified-delegation-acceptance.trace.md)
  - Origin:
    - [relative](001-2-7-5-1-blank-workspace-qualified-delegation-acceptance.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 17:24:06
  - Authors: Anchor
  - Why: Kodax is blocked despite an explicit-session Holder Relationship because Core matches a small set of exact prose variants.
  - Summary: Normalize qualified Role holder-assignment semantics so explicit-session authorization is not an exact-prose whitelist.
  - Status: ready/local

---

# Canonical Holder Assignment Mode Normalization

## Objective

Close the production-blocking holder-authorization defect in which semantically legitimate Role Holder Relationship values are accepted or rejected according to exact prose variants instead of canonical assignment meaning.

The current Core implementation recognizes only a small whitelist of whole Holder State strings. This makes Anchor/Axiom and Loom behave differently from Kodax even when all of them explicitly permit bounded session assignment. The fix must preserve the existing safety separation between a session Role assertion, qualified Role assignment authority, and durable holder identity.

## Done Criteria

- Axiom defines the canonical semantic model for Role holder-assignment modes using existing primitives where sufficient and identifies whether any schema/structured representation is actually missing.
- Equivalent qualified Role declarations that authorize explicit bounded session assignment project the same assignment authorization without heuristic interpretation of arbitrary prose.
- Anchor, Axiom, Loom, Kodax and at least one additional existing Role variant are covered by acceptance evidence.
- Session binding remains explicit and does not become durable holder identity, participation, process applicability, source authority or acceptance.
- Unknown/unqualified Holder Relationship wording fails closed with an exact reason rather than being permissively parsed.
- Loom later consumes the accepted semantic result structurally/normalistically rather than by expanding an exact-prose whitelist.

## Scope

Holder assignment semantics and the Core authorization projection only. No broad Role redesign, identity system, participant semantics, delegation semantics or product work.

## Dependencies

- existing Holder Binding Authorization Gate;
- observed Kodax `session-holder-role-binding-authorization-unresolved` production blocker;
- current qualified Anchor/Axiom/Loom/Kodax Role artifacts.

## Boundaries

- Do not repair this by rewriting Kodax prose to one currently whitelisted sentence.
- Do not authorize assignment from Handoff endpoint names, project/chat labels, package placement or session self-assertion alone.
- Do not create heuristic natural-language parsing of arbitrary Holder Relationship prose.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-7-5-1-blank-workspace-qualified-delegation-acceptance.trace.md](001-2-7-5-1-blank-workspace-qualified-delegation-acceptance.trace.md)
  - Value: yesQil2Qu4qHbmcJYHGIWacZMcpqZ3-inxvGoa5W-mE

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: sHcRIrW-bE0NbTMBahP5wbeJg3VVtpaeU5wqWGajp_0