# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-08 23:38:17
  - Trace: [001-3-6-4-repository-frontiers-lineage-stabilization-turn2-task.trace.md](001-3-6-4-repository-frontiers-lineage-stabilization-turn2-task.trace.md)
  - Origin:
    - [relative](001-3-6-4-repository-frontiers-lineage-stabilization-turn2-task.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-09 01:31:00
  - Authors: Anchor
  - Summary: Freeze the post-extraction repository and bootstrap ownership boundaries without fabricating absent hosts.
  - Status: ready/local

---

# Repository and bootstrap responsibility boundary

This decision records the post-extraction repository responsibility map used by Turn 2. Repository placement is implementation/distribution topology, not semantic authority.

## Decision

- `Tiinex/docs` remains canonical authority for Tiinex schemas, validators, semantic contracts and maintained interpretation notes.
- `Tiinex/business` remains the organizational, initiative, Role, priority and human-gate surface.
- `Tiinex/core` owns shared host-neutral implementation mechanics: artifact/schema interpretation runtime, validation, provenance/lineage, grounding, Handoff/package manufacture, deterministic projections, companion resolution and the carrier/tooling bootstrap required for a Handoff to cold-start without another Tiinex package.
- `Tiinex/app` owns the reusable Viewer/application layer above Core: shared application data, Viewer, React infrastructure, Verse hosting and host-neutral application composition.
- `Tiinex/site` is the official thin web deployment over App/Core and owns deployment configuration, web hosting, deployment overrides/providers and public-site integration only.
- `Tiinex/playthings` remains a separately owned Verse package consuming App/Core contracts; its world/presentation implementation does not confer Tiinex semantic authority.
- A future `Tiinex/cli` is the dedicated ordinary command-line host over Core. Until its actual Workspace is supplied or explicitly bootstrapped, Core may retain the existing portable executable as transitional distribution mechanics.
- A future `Tiinex/interop` owns external-assistant/automation interoperability: external bootstrap experiences/instructions, portable tool contracts and environment adapters. Core's current `tiinex.llm.bootstrap.md` and pointer are classified as transitional Interop-facing material; they are not moved or deleted until an actual Interop Workspace and consumer migration are qualified.
- A future `Tiinex/chrome` is a bounded browser host over App/Core. Historical Chrome-extension mechanics do not define its current contract.
- VS Code remains a separate host lane. Its preparatory Anchor may consume already-stable Core contracts but may not freeze CLI/Interop contracts before this Turn-2 frontier is returned.

## Basis

Turn 1 separated the monolithic Site implementation into Core, App and a thin Site. Current Core still contains both self-contained Handoff bootstrap mechanics and external LLM-facing bootstrap material, which made the word `bootstrap` appear to imply one owner. The former is intrinsic to portable Handoff/package execution; the latter is an interoperability experience. Docs authority is independent of both. Business already defines Tooling and Viewer initiatives separately and explicitly states that repository location does not define semantic ownership.

The supplied Turn-2 carrier contains current Business, Docs, Core, App, Site and Playthings Workspaces. It does not contain current CLI, Interop or Chrome Workspaces. Their absence is therefore preserved as an unresolved source boundary rather than reconstructed from assumptions.

## Consequences

- Core may continue to ship the embedded portable Tooling runtime and schema-material projections needed to verify/cold-start its carriers; those bytes do not become canonical schema authority.
- External-assistant bootstrap language may be documented as transitional inside Core but should migrate to Interop when that repository is established and qualified.
- CLI extraction must reuse Core instead of copying portable implementation; Core's current executable is a transitional compatibility surface, not proof that Core is the final CLI host.
- Site may remove duplicated App/Core documentation, Tooling copies and historical implementation debris after exact recovery/reduction evidence is established.
- Docs first-contact material should describe this repository map and stop routing ordinary Tooling bootstrap through a historical Site commit.
- No current CLI, Interop or Chrome implementation is claimed by this decision. Sigma must supply those Workspaces if they already exist; otherwise a separate explicit bootstrap decision is required before new repositories are created.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-3-6-4-repository-frontiers-lineage-stabilization-turn2-task.trace.md](001-3-6-4-repository-frontiers-lineage-stabilization-turn2-task.trace.md)
  - Value: Z-8KDTRtswJDhg820T7a-hH1kHqlQimQNPz1HECJQSM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: uFWIINQMVouGY_KTCdHOAoyuPD2_f4elpB6NaFPnILM