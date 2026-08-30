# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:57:00
  - Trace: [Initiatives](001-initiatives.trace.md)
  - Origin:
    - [relative](001-initiatives.trace.md)
- Current
  - Current Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Authors: Anchor; Sigma
  - Why: Preserve Viewer as a first-class human product surface without allowing presentation needs to redefine Tiinex semantics or fork shared Tooling behavior.
  - Summary: Cross-repository Initiative for the human-facing Tiinex viewing and interaction surface built on the same artifact semantics and shared implementation as Tooling where practical.
  - Status: accepted/local

---

# Tiinex Viewer

## Project Identity

- Description: Tiinex Viewer is the Initiative for human navigation, reading, inspection, and interaction with Tiinex artifacts, lineage, provenance, workspaces, and current project surfaces.
- Boundary: Viewer owns human-facing presentation and interaction. It does not define canonical artifact semantics, replace Tooling qualification, or turn UI state into hidden project truth.

## Project Purpose And Scope

- Description: Make Tiinex understandable and useful to a person without requiring CLI expertise, while projecting the same explicit artifacts, provenance, boundaries, and qualified current state used by Tooling and LLMs.
- Boundary: Viewer follows shared semantics and should reuse shared Tooling/runtime code where practical. Viewer-specific affordances must not become undocumented semantic authority.

## Parties And Resources

- Relevant Parties: Sigma for human actual-path observation and usability judgment; Anchor for architecture and coherence; Loom for shared implementation; Axiom when presentation exposes semantic ambiguity.
- Relevant Resources: Tiinex Site/reference implementation, Viewer workspace material, shared Tooling/runtime code, canonical Docs semantics, and real Business/initiative artifacts as product dogfood.

## Coordination State

- Description: Viewer implementation remains less active than Tooling, but human-product comprehensibility is now an explicit foundation acceptance dimension. Historical strategy prioritized portable Tooling qualification before Viewer integration; current work therefore resumes from a concise human-observed product baseline rather than historical UI leaves.
- Boundary: Do not invent Viewer work merely for symmetry with Core or Tooling, and do not equate implementation activity with product importance. Work packages should correspond to meaningful human outcomes and shared integration needs.

## Milestones And Outcomes

- Description: Meaningful outcomes include clear active-frontier navigation, recognizable workspace/artifact patterns, visible Parent/lineage comprehension up to organizational context, shared Tooling-backed workspace operations, and a credible public provenance/reference experience.
- Boundary: A polished Viewer does not prove underlying semantic correctness, Tooling completeness, or project maturity.

## Interpretation Limits

- Does Not Prove: that Viewer is the whole Tiinex product, that displayed state is canonical, or that every Tooling capability must have a UI
- Must Not Be Treated As: the semantic authority for Tiinex, a replacement for CLI/Tooling, or a requirement that all project work be optimized for one interface

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Initiatives](001-initiatives.trace.md)
  - Value: ooAvsZ-ZLG6eafU4w8lMBq8-Zj5rrurJeLA_o2dMh0I

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Z9OpOKoRrUw36W8_jOf7E3_-Ec36pqymqyIHKtYWIYc
