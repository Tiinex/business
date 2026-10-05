# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 15:04:00
  - Trace: [001-business-lineage-structure-decision.trace.md](001-business-lineage-structure-decision.trace.md)
  - Origin:
    - [relative](001-business-lineage-structure-decision.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-10-05 19:21:14
  - Authors: Anchor; Sigma
  - Why: Make the human-readable structure match existing ownership semantics before Tooling or migration encodes another implicit convention.
  - Summary: Establish what/where Entry discovery, Workspace-local work areas, reduction discoverability and provider-specific placement without turning directories into semantic authority.
  - Status: ready/local

---

## Decision

- State: accepted
- Subject: Entry what/where composition, Workspace-local work areas, terminal reduction discoverability, and provider-specific placement
- Decision: Tiinex reusable entry composition uses the human/discovery dimensions `what` and `where` beneath `.topics/.entries/` while qualified schema/artifact material remains the semantic truth. Purpose/session Entries answer what the receiver is trying to do; Target Entries answer where that Entry is interpreted or performed. Provider- or host-specific Target Entries, process profiles, host adaptation and related durable work belong in their semantically owning interop/host Workspace. Bounded implementation work should be grouped into descriptive Workspace-local work-area directories beneath `.topics/work/`, while Business retains organizational why, cross-Workspace coordination, acceptance and disposition. Terminal work areas should be distilled through Reduction surfaces rather than leaving long execution lineages looking active. Directory shape is a discovery projection and must never replace Parent, Project/Task, Handoff, lifecycle, Role, Process applicability or other semantic authority.

## Basis

- Human readers can recognize healthy and unhealthy work shape more reliably when one bounded subject owns a visible work-area directory instead of sharing one indefinitely growing flat journal.
- Workspace-local execution prevents specialist Roles from needing Business write authority merely to perform implementation work in another repository.
- Purpose Entry and environment Target Entry are orthogonal dimensions; nesting targets under each purpose Entry would duplicate the same host knowledge and couple provider-specific material to portable Entry definitions.
- OpenAI/GPT-specific behavior belongs in `interop-openai`, including Target Entries, provider-specific Process material, host adaptation and provider-specific work, rather than Core or portable Native.
- Existing Process and Work Lifecycle material already distinguishes organizational coordination from natural Workspace implementation ownership; this Decision makes the corresponding directory/discovery projection explicit.
- Markdown artifacts must remain sufficient for emergency/cold grounding without requiring Viewer or Tooling interpretation of folder names as hidden authority.

## Consequences

- Preferred Entry layout is `.topics/.entries/what/<entry-handle>/` for reusable purpose Entries and `.topics/.entries/where/<target-handle>/` for environment Target Entries.
- Entry discovery must classify by qualified schema/material. `what/` and `where/` are human/discovery hints, not semantic type authority.
- Target Entry selection is optional unless the environment materially affects the bounded activity. Pointerless orientation may discover/select a target locally after the purpose Entry is chosen.
- Formal Handoffs may require or recommend purpose Entries and may pin an exact Target Entry when the host is part of the bounded work. Handoff/Role/qualified relations remain the authority/work-transfer surface; Entries do not grant authority.
- Implementation work belongs in `.topics/work/<work-area-handle>/` in the natural owning Workspace. Work-area handles are descriptive scope labels, not semantic Parent or Project identity.
- Long same-area lineages are diagnostic signals that disposition/reduction should be reviewed. They are not automatically invalid solely because of length.
- A terminal work area may be distilled under `.topics/reductions/work/<work-area-handle>/`; Reduction semantics come from the qualified artifact/lifecycle authority, not the directory name.
- Process roots should remain one artifact only when genuinely atomic. Durable independently followable phases, branches, recovery boundaries and human gates should be represented as separate artifacts within the owning process directory.
- This Decision does not decide whether Tiinex should introduce a dedicated `tiinex.process.v1` schema. Process schema typing remains a separate schema-development decision; decomposition and directory readability must not wait on or prejudge that choice.
- Existing flat Entry/Work/Reduction layouts remain valid source material until a separately qualified migration plan moves them. No broad migration is authorized by this Decision.

## Review Conditions

- Review if a dedicated Process schema or Entry composition schema supersedes these structural conventions.
- Review if capability-based Target compatibility requires a richer portable contract than `tiinex.entry.target.v1` provides.
- Review if real Workspace migration demonstrates that work-area handles need stronger machine identity than human/discovery scope labels.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-business-lineage-structure-decision.trace.md](001-business-lineage-structure-decision.trace.md)
  - Value: yrgTdisjDp_Msb0sv69J9Agpr_x478fLFG6qSNnpxhI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: rvEKaBdQ8YjpfmiD6bOibLvBOVXTYIOzJ4PtR5lB67w