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
  - Why: Make Tooling the primary operational consumption surface while preserving shared semantics and reusable implementation for Viewer and other hosts.
  - Summary: Cross-repository Initiative for the shared CLI and portable Tooling mechanics used by humans and LLMs to discover, resolve, validate, repair, package, project, and continue Tiinex work.
  - Status: accepted/local

---

# Tiinex Tooling

## Project Identity

- Description: Tiinex Tooling is the Initiative for portable and shared operational mechanics: CLI, Discovery, schema capability resolution, validation, integrity, repair, Handoff manufacture, packaging, projection, host binding, and evidence return.
- Boundary: Tooling implements and exposes semantics but does not invent canonical schema meaning, human acceptance, business priority, or Viewer-specific presentation authority.

## Project Purpose And Scope

- Description: Give humans and LLMs the same explicit, recoverable operational path through Tiinex material, minimizing hidden memory, manual archaeology, provider assumptions, and duplicated host-specific logic.
- Boundary: CLI/Tooling is the primary implementation target; Viewer should reuse shared code where appropriate rather than drive Tooling semantics backward.

## Parties And Resources

- Relevant Parties: Loom for implementation and qualification; Axiom for semantic authority gaps; Anchor for architecture and acceptance boundaries; Sigma for human actual-path observation and priorities.
- Relevant Resources: Portable Tooling runtime, Site source and historical dogfood corpus, Docs schemas, Business operating artifacts, fresh-recipient tests, host capability adapters, and repository workspaces.

## Coordination State

- Description: Foundation activity is intentionally narrow: measure iteration efficiency and make the stable recovery/cold-start contract explicit. Existing qualified Tooling may be used; broad new Tooling feature expansion remains held.
- Boundary: Historical density is not a reason to reactivate old leaves. New technical Tasks belong close to implementation and must connect upward to a current work-package outcome a human maintainer can understand.

## Milestones And Outcomes

- Description: Meaningful outcomes include reliable active-frontier Discovery, clean portable cold-start and Handoff, integrity/repair tooling, broad authoring/schema capability coverage, and a shared host-neutral runtime that Viewer can consume.
- Boundary: Passing internal tests does not alone prove human usability, semantic correctness, or product acceptance.

## Interpretation Limits

- Does Not Prove: that current Tooling covers every schema, host, repository, artifact shape, or failure mode
- Must Not Be Treated As: canonical schema authority, a Viewer roadmap, an autonomous agent framework, or proof that a generated package is semantically correct merely because it was emitted

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Initiatives](001-initiatives.trace.md)
  - Value: R5Fv3xeMg51j9bQuSnDRgao6IgM-lVHZ55dHGoNcIDU

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: r9jB8WC2FVPxtL4hQGcU0buUznxvGHkwK-mT_SdGQ3I
