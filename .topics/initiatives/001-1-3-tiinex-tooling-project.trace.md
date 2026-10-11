# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-10-03 22:13:00
  - Trace: [006-tiinex-project.trace.md](006-tiinex-project.trace.md)
  - Origin:
    - [relative](006-tiinex-project.trace.md)
- Current
  - Current Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-10-03 22:13:35
  - Authors: Anchor; Sigma
  - Why: Re-establish the durable Tooling direction and give future host-neutral operations a truthful Project boundary independent of repository layout.
  - Summary: Tooling Project sibling for portable shared operational mechanics consumed by humans, LLMs, CLI, IDE, and Viewer hosts.
  - Status: ready/local

---

# Tiinex Tooling

## Project Identity

- Description: Project for portable shared operational mechanics that let humans and LLMs discover, qualify, author, validate, repair, move, package, hand off, and continue Tiinex work deterministically across hosts.
- Boundary: Tooling implements and exposes Tiinex semantics but does not invent canonical semantic meaning, Business priority, human acceptance, or Viewer-specific presentation authority.
- Related Project: [Deterministic Lineage Maintenance](../initiatives/004-deterministic-lineage-maintenance-project.trace.md)

## Project Purpose And Scope

- Description: Provide one host-neutral operational contract wherever practical so CLI, LLM, VS Code, Viewer, and future hosts do not fork semantic behavior or rely on manual filesystem improvisation.
- Boundary: Host UX may live in host-specific Workspaces while sharing qualified Core mechanics. Workspace ownership and package boundaries do not make each Workspace a separate Project.

## Parties And Resources

- Relevant Parties: Sigma for operator intent/usability and qualified architecture, Tooling, host, and review Roles according to bounded work.
- Relevant Resources: portable Core tooling/runtime, CLI and host adapters, VS Code integration, lineage/integrity mechanics, Handoff manufacture, schema capability resolution, and real project dogfood.

## Coordination State

- Description: Tooling is re-established as a current direction Project without reviving stale pre-reduction execution. Existing `004 Deterministic Lineage Maintenance` is a current pre-portfolio transition Project related to this direction and retains its already-published ancestry while its Core Task is repaired to that Project.
- Boundary: New Tooling execution should use Tasks/subtasks for ordinary decomposition and child Projects only for independently meaningful coordinated outcomes.

## Milestones And Outcomes

- Description: Deterministic cold-start/handoff, authoring, integrity/repair, lineage maintenance, project/work projection, host-neutral operation contracts, and safe host integrations that reuse shared mechanics.
- Boundary: Tooling completeness is not equivalent to semantic correctness, human usability, Viewer completeness, or product acceptance.

## Interpretation Limits

- Does Not Prove: coverage of every schema, host, repository, artifact shape, filesystem operation, or failure mode.
- Must Not Be Treated As: canonical schema authority, an autonomous-agent framework, or permission for hosts to bypass shared qualification contracts.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [006-tiinex-project.trace.md](006-tiinex-project.trace.md)
  - Value: sC3A3zCR8C1mKNGERm0cj4lFbA33bthZMoEumdGLjOk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 9ar_KyxmeMb7Sd6ZrHvQ5qUxgt6YR9AO-1Xdx7Exro0