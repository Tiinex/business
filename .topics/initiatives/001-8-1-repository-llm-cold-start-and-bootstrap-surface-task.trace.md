# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-27 23:54:00
  - Trace: [Public Surfaces And Repository Hygiene](001-8-public-surfaces-and-repository-hygiene-task.trace.md)
  - Origin:
    - [relative](001-8-public-surfaces-and-repository-hygiene-task.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-29 10:09:00
  - Authors: Anchor; Sigma
  - Summary: Repository LLM Cold-Start And Bootstrap Surface
  - Status: accepted/local

---

# Repository LLM Cold-Start And Bootstrap Surface

## Objective

Make every public Tiinex repository a safe, bounded first-contact surface for a blank LLM or human reader: it should be possible to recover Tiinex identity, the repository's current role and status, the canonical orientation path, and a verified Tooling bootstrap route without hidden project context or unsafe code execution.

## Done Criteria

- Every public Tiinex repository exposes one obvious root-level route for LLM/machine readers, reachable from the ordinary README or equivalent first-contact surface.
- A consistent `llms.txt`-style router identifies the repository role/status, points to organization-level Tiinex identity, and names the next bounded reading step without redefining semantic authority.
- The public Tooling bootstrap has one machine-readable locator that names repository/path plus an explicit commit or release qualification boundary and a verification method; a moving branch alone is not presented as stable bootstrap authority.
- Cold-start guidance preserves the existing Tooling safety boundary: host-mediated fetch, no source mutation, no remote write, and no execution of received package code merely because it was discovered.
- A blank LLM given any one public Tiinex repository can state what Tiinex is, what that repository currently is, what is current versus historical, where to obtain bootstrap guidance, what it is not authorized to do, and where to continue for task-specific discovery.
- Historical or stale repositories route the reader toward current grounding instead of allowing old implementation claims to become current by proximity.
- Current `site` branch/publication policy is explicit enough that bootstrap routing does not silently conflate current source, default branch, public release qualification, and transport convenience.
- The solution remains small and vendor-neutral: ordinary human README guidance plus a common machine router and canonical manifest/pointer are preferred over a growing collection of model-provider-specific prompt files unless testing demonstrates a real need.

## Scope

- Business owns the public/cold-start acceptance requirement and repository first-contact policy.
- Existing Tooling work package `Portable Handoff, Cold-Start And LLM Ingress` owns bootstrap mechanics and qualification behavior.
- Repository README, `llms.txt`, orientation/context, manifest, bootstrap-pointer, release/package, and equivalent public projection surfaces are in scope.
- Do not start unrelated Tooling, Viewer, schema, or repository-cleanup work under this task.
- Do not create a new semantic schema merely to route an LLM; reuse readable public files and existing bootstrap semantics unless a demonstrated semantic gap remains.

## Dependencies

- [Public Surfaces And Repository Hygiene](001-8-public-surfaces-and-repository-hygiene-task.trace.md).
- [Portable Handoff, Cold-Start And LLM Ingress](../initiatives/001-2-2-portable-handoff-cold-start-ingress-task.trace.md).
- Current organization orientation/context in `Tiinex/.github`.
- Current `Tiinex/site` portable bootstrap Markdown and bootstrap pointer.
- Sigma review of the first cold-reader/ambassador model before public repository changes are propagated.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Public Surfaces And Repository Hygiene](001-8-public-surfaces-and-repository-hygiene-task.trace.md)
  - Value: 225g3JxSdVX1aAzXu1aN84JgQXKvijyvtHMhx1HN_i8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: W9ilLnXyCbsYd4_wCczszY87LLtPjEgULC5tmjA_Ikk
