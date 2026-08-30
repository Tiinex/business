# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Viewer](001-3-viewer-project.trace.md)
  - Origin:
    - [relative](001-3-viewer-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-26 22:30:00
  - Authors: Anchor; Sigma
  - Summary: Human Navigation And Active Frontier Experience
  - Status: draft/local

---

# Human Navigation And Active Frontier Experience

## Objective

Give a human a clear way to enter Tiinex, recognize where they are, understand what is current versus historical, move across Initiatives/workspaces/lineages, and reach the active frontier without LLM assistance or internal repository archaeology. Preserve the strongest human-observed PoC interaction qualities while allowing deliberate improvements rather than requiring pixel parity.

## Done Criteria

- Viewer can present declared current/historical boundaries and active Initiative/work-package context.
- A person can recognize workspace context and common artifact/action patterns before needing to read full prose; color may support recognition but is reinforced by text, icon, position, or shape rather than carrying meaning alone.
- Feed, Tree, and Lineage remain meaningfully distinct views: what is present, where material is arranged, and how declared continuity/Parent relationships connect it.
- Navigation follows qualified artifact relations and workspace entrypoints rather than hidden UI state.
- From a current local organizational Task, a human contributor can follow visible Parent context upward to its Project/Initiative and ultimately the Tiinex organization root where that lineage applies.
- Progressive disclosure keeps ordinary navigation calm while full Markdown, provenance, diagnostics, and advanced controls remain available on demand.
- Current, historical/time-view, loading, degraded, and mismatch states are visibly distinguishable.
- A person can move from portfolio-level context to relevant cross-repository work and back without losing provenance.
- Historical dogfood remains inspectable without dominating the default current experience.
- A PoC behavior that materially mattered to human comprehension is either recovered, intentionally changed with a stated reason, or explicitly rejected; it is not silently lost during refactor.

## Scope

- Do not invent active state from UI heuristics when artifacts disagree.
- Do not require every Tooling capability or diagnostic to be exposed at once; internal truth can remain available behind progressive detail rather than competing with the primary human task.
- Preserve visual pattern consistency as a usability contract, but do not treat the historical PoC layout as immutable pixel authority.
- Keep the underlying artifact/permalink and Parent path visible enough for recovery.

## Dependencies

- Tooling Discovery/frontier epic.
- Business Initiatives and later operating overview.
- Site historical cutoff decision.
- Human-observed PoC demonstration reviewed during the 2026-08-29 foundation reconciliation as product evidence for workspace context, repeated visual grammar, Feed/Tree/Lineage separation, progressive disclosure, and visible lineage-to-root behavior.

## Foundation Operating Read

- This work package is Active during the foundation phase as a human-product baseline and acceptance lane, not as permission for broad Viewer feature expansion.
- The PoC is product evidence rather than semantic authority: current implementation may improve it, but a lost human value needs an explicit disposition.
- Human comprehensibility is a foundation gate alongside provenance correctness because a technically correct Tiinex that requires an LLM or repository archaeology for routine orientation has not met the intended product outcome.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Viewer](001-3-viewer-project.trace.md)
  - Value: Z9OpOKoRrUw36W8_jOf7E3_-Ec36pqymqyIHKtYWIYc

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: c2gj0xBCFuLGxc6cF68wG_J55LEeNtc18wrCK1wjKqc
