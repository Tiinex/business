# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-10-04 02:20:00
  - Trace: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Origin:
    - [relative](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-04 21:36:02
  - Authors: Anchor; Sigma
  - Why: Remove the last observed workflow deviations without reopening accepted lineage, Workspace, or Package V1 semantics.
  - Summary: Close continuation naming, transport-text hygiene, Handoff preview, and byte-identical embedded-source preference before the stable Major.
  - Status: ready/local

---

# Finish Handoff Package Transport And VS Code Presentation Polish Before Stable Major

## Objective

Close the remaining non-blocking regressions around Handoff Package transport naming, CLI sidecar hygiene, VS Code Handoff presentation, and deterministic byte-identical source preference so the repaired workflow can be accepted and promoted to a real stable Major.

This Task is deliberately narrow. It does not reopen the already accepted/fixed Major allocation, Workspace Replace/Initialize, artifact lineage, carrier Parent semantics, or Package V1 internal topology.

## Observed Regressions

After the repaired standard workflow and carrier Major allocation were confirmed, four remaining edges were observed:

1. A normal continuation transport name advanced after the semantic route slug, producing names shaped like `...-anchor-to-sigma-1.handoff-package.zip` instead of extending the carrier dimension before the slug.
2. Calling manufacture with the common spelling `--transport-text true` was parsed as the literal path `true`, creating a `true` file containing routing text in the current Core directory. That file was also carried by the previous full recovery carrier.
3. Clicking a Handoff artifact opened raw Markdown source by default even though the existing VS Code Markdown Preview surface is the preferable read-first presentation and already allows switching back to source.
4. When a selected local Workspace and an embedded Incoming Workspace are byte-identical, Outgoing source resolution could still keep the local source because source order favored Local. Byte-identical candidates should deterministically prefer the embedded carried bytes; changed local material must continue to win only when it is not byte-identical.

## Candidate Changes

### Carrier continuation transport naming

Core's transport-only continuation projection now:

- parses the transport Major/prefix from the parent filename;
- preserves the existing carrier dimension suffix;
- appends the continuation ordinal to that dimension;
- preserves any semantic route slug after the dimension.

Example:

`tiinex-018-1-1-1-anchor-to-sigma.handoff-package.zip`

becomes:

`tiinex-018-1-1-1-1-anchor-to-sigma.handoff-package.zip`

The change is transport filename projection only. It does not alter qualified carrier lineage, artifact lineage, semantic Parent ancestry, route identity, or Package V1 content topology.

### Transport sidecar hygiene

Core CLI now normalizes the optional `--transport-text` value:

- bare `--transport-text` and `--transport-text true` both mean “write the canonical adjacent `.transport.txt` sidecar”;
- `--transport-text false` disables sidecar output;
- any other non-empty value remains an explicit path.

The leaked `core/true` file is removed from the candidate Workspace and therefore from the next full recovery carrier. No `.gitignore` masking is added because the actual parser/sidecar footgun was identified and repaired.

### Handoff presentation

VS Code artifact navigation keeps source-backed material authority unchanged, but a Handoff artifact now opens through the built-in `markdown.showPreview` command first. If preview is unavailable, navigation falls back to the exact Markdown source. Ordinary non-Handoff Markdown navigation remains source-first.

### Byte-identical embedded source preference

For Outgoing Workspace source selection, VS Code qualifies exactness through the existing shared Core comparison. When a selected Local source has an exact byte-identical embedded Incoming source for the same Workspace, selection is normalized to the embedded source. Non-identical/changed Local material is not replaced by embedded material.

This is a deterministic source-selection rule only; Workspace identity and qualification remain Core-owned.

## Anchor Acceptance Evidence

- Core focused regression suite: 19/19 passing across transport naming, collision projection, Major frontier behavior, manufacture hygiene, and package projection.
- Public Core operation projected `tiinex-018-1-1-1-1-anchor-to-sigma.handoff-package.zip` from parent `tiinex-018-1-1-1-anchor-to-sigma.handoff-package.zip` with continuation ordinal `1`.
- Real Core manufacture using `--transport-text true` completed ready, wrote `tiinex-001.transport.txt` adjacent to its package, and did not create `core/true`.
- VS Code modified TypeScript files transpile successfully.
- A direct source-selection regression check proved byte-identical embedded `core` replaces selected Local `core`, while changed/non-identical `docs` remains Local.
- The previous full carrier was inspected and confirmed to contain `core/true`; the candidate Core Workspace does not contain that file.

## Scope

- Core transport-only continuation filename projection.
- Core CLI transport-text optional-value hygiene and removal of the leaked `true` file.
- VS Code default Handoff read presentation through built-in Markdown Preview.
- VS Code byte-identical Local/Incoming duplicate resolution in Outgoing source selection.
- One final Sigma real-host acceptance before creating the real stable Major.

## Dependencies

- [Grounding And Continuity Readiness](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- [Align Handoff Package Carrier Major Allocation](006-align-handoff-package-carrier-major-allocation-task.trace.md)
- Current Core, VS Code, Native, Business, and OpenAI Interop Workspaces carried by the resulting Handoff Package.
- Existing Session Grounding And Continuity / recipient-transfer guidance.

## Done Criteria

- Continuation transport filenames extend the carrier dimension before the route slug.
- `--transport-text true` cannot create a literal `true` output file and canonical sidecar output still works.
- The next full recovery carrier no longer contains `core/true`.
- Handoff artifact clicks open built-in Markdown Preview by default with source fallback preserved.
- Byte-identical Local versus embedded Incoming candidates resolve to embedded deterministically; non-identical local changes are preserved.
- Existing Major allocation, Replace, Initialize, and Package V1 roundtrip behavior remain intact.
- Sigma can perform the final host observations without debugging implementation and can then create the real stable Major if all checks pass.

## Boundaries

- No artifact lineage, artifact filename convention, semantic Parent ancestry, or artifact authority changes.
- No carrier Parent or Package V1 internal archive topology changes.
- No Workspace identity/discovery, Replace, Initialize, or Major allocation rule changes.
- The continuation transport filename projection is explicitly transport-only and does not become semantic authority.
- No commit, push, publication, release, deployment, or other remote mutation is authorized by this Task.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: NPCAHRoAI1kXK9R9tmKMBnHvI2MnknEtszfSuZZlrd4