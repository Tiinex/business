# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-27 00:08:00
  - Trace: [Anchor Consolidation Of Axiom Disposition And Loom Routing](../business-development/005-anchor-axiom-disposition-consolidation-and-loom-routing-decision.trace.md)
  - Origin:
    - [relative](../business-development/005-anchor-axiom-disposition-consolidation-and-loom-routing-decision.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-08-27 00:08:00
  - Authors: Anchor
  - Why: Route the implementation blockers accepted by Axiom and consolidated by Anchor to Loom before Business lineage repair and the first stabilization checkpoint.
  - Summary: Anchor-to-Loom implementation and qualification of truthful local Parent Origin support, recipient-v2 carrier artifact purity, Handoff closure/workspace hygiene, and carrier-dimension prefix regression coverage.
  - Status: active/local

---

# Tiinex Business Development — Loom Root And Handoff Carrier Repair

## Handoff Parties

- Purpose: Implement and qualify the minimum Tooling corrections required before Anchor can repair the current Business graph truthfully and prepare the stabilization checkpoint.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-anchor-role.trace.md)
- To: Loom
- To Kind: role
- To Reference: [Loom Role](../roles/001-loom-role.trace.md)

## Transfers

- root-local-parent-origin
  - Transfer Kind: work
  - Description: Implement the Axiom-accepted Root/validator/runtime correction so a local unpublished Parent is valid when the Parent target is directly recoverable from the same qualified workspace/materialization. A qualified `relative` locator must be sufficient for same-workspace local continuity; `browse + git` is required only when that forge/commit recovery claim is actually true.
  - Boundary: Preserve Parent as direct continuity ancestry. Do not weaken unresolved-Parent failure, fabricate forge locators, infer publication, or let Task/Handoff descendants silently re-impose `browse + git`.
  - Qualification Evidence: local-relative Parent pass; commit-pinned published Parent pass; unresolved Parent fail; fabricated/unresolvable forge origin fail; cold-recipient Handoff qualification carrying local Parent bytes.

- recipient-v2-carrier-purity
  - Transfer Kind: work
  - Description: Remove repeated transport-private `TIINEX-RECIPIENT-V2-FACTS` JSON from visible human-readable carrier artifacts and move/derive the necessary package topology, byte-map, route, and transport projection facts from one explicitly transport-owned control/manifest/evidence surface.
  - Boundary: Do not expand `tiinex.handoff.v1` semantic scope. Orientation, route qualification, exact byte identity, context audit, and roundtrip recovery must remain independently qualified.
  - Qualification Evidence: fresh-recipient package whose visible semantic carrier artifacts contain no duplicated opaque transport facts while preferred cold-start orientation, route grounding, context audit, and roundtrip still pass.

- handoff-closure-workspace-hygiene
  - Transfer Kind: work
  - Description: Ensure Handoff required closure can be carried and resolved from package-owned material without writing closure-only predecessor copies into a durable source Workspace `.topics/.cache` hierarchy. Preserve historical package/workspace bytes and recovery semantics.
  - Boundary: Do not delete or rewrite historical Handoff/package bytes. Do not claim current Business `.topics/.cache` is safe to remove until Anchor has independent recovery proof after the stabilization checkpoint.
  - Qualification Evidence: old package remains byte-recoverable; new manufacture resolves required context without creating new source-workspace `.topics/.cache` closure residue; context audit accounts for detached closure material; historical relative references are not silently broken.

- carrier-dimension-fixed-width-regression
  - Transfer Kind: work
  - Description: Add or demonstrate regression coverage that Tooling-owned carrier dimensions preserve their fixed-width numeric segments such as `001` and do not normalize them to `1` across child continuation and explicit major manufacture.
  - Boundary: This transfer records a user-observed risk, not a reproduced defect in the current package lineage. Do not claim a prior prefix-loss defect unless evidence reproduces it.
  - Qualification Evidence: representative continuation and major manufacture outputs preserve exact fixed-width segment formatting and orientation reports the same dimensions.

## Required Context

- axiom-semantic-disposition
  - Material: accepted Axiom semantic disposition for the current Business lineage/composition tranche
  - Material Reference: [Axiom Business Lineage And Composition Gap Disposition](../decisions/001-axiom-business-lineage-and-composition-gap-disposition.trace.md)
  - Purpose: authoritative semantic target for the Loom implementation work in this transfer
  - Availability: available

- anchor-consolidation
  - Material: Anchor consolidation and sequencing decision
  - Material Reference: [Anchor Consolidation Of Axiom Disposition And Loom Routing](../business-development/005-anchor-axiom-disposition-consolidation-and-loom-routing-decision.trace.md)
  - Purpose: ground the accepted implementation sequence and retained responsibilities
  - Availability: available

- stabilization-quality-gate
  - Material: accepted stabilization commit and working-set retention decision
  - Material Reference: [Stabilization Commit And Working-Set Retention Decision](../business-development/004-stabilization-commit-and-working-set-retention-decision.trace.md)
  - Purpose: constrain the return to implementation/qualification and preserve the later Anchor/Sigma gates
  - Availability: available

- tooling-initiative
  - Material: current Tiinex Tooling Project
  - Material Reference: [Tiinex Tooling](../initiatives/002-tooling-project.trace.md)
  - Purpose: ground the Initiative boundary for this implementation work
  - Availability: available

- practitioner-baseline
  - Material: current Tiinex Practitioner Role baseline
  - Material Reference: [Tiinex Practitioner Role](../roles/001-practitioner-role.trace.md)
  - Purpose: preserve the shared obligation to surface meaningful friction and human/LLM asymmetry as improvement evidence
  - Availability: available

- loom-role
  - Material: current Loom Role
  - Material Reference: [Loom Role](../roles/001-loom-role.trace.md)
  - Purpose: constrain implementation authority and evidence-return responsibilities
  - Availability: available

## Reference Context

- current-business-workspace
  - Material: current full-source tiinex/business working snapshot
  - Purpose: reproduce the accidental-root and `.topics/.cache` observations without treating cosmetic hierarchy as semantic authority
  - Availability: available

- carried-docs-workspace
  - Material: current full-source tiinex/docs working snapshot
  - Purpose: schema and validator authority for Root/Handoff qualification
  - Availability: available

- carried-site-workspace
  - Material: current full-source tiinex/site working snapshot
  - Purpose: Tooling implementation source, historical dogfood, and prior Handoff/carrier behavior
  - Availability: available

- axiom-return-package
  - Material: qualified Axiom-to-Anchor return carrier `axiom-return-002-1-axiom-to-anchor.handoff-package.zip`
  - Purpose: exact evidence for the accepted disposition and carrier-lineage parent of this continuation
  - Availability: available

## Retained Responsibilities

- business-graph-repair
  - Retained By: Anchor
  - Responsibility: repair Project-to-epic, Business Development, Role-version, typed-relation, Decision/Research/Handoff continuity, and final Discovery/audit only after Loom returns qualified blocker evidence
  - Boundary: Loom must not make Business portfolio hierarchy look tidy by inventing Parent edges.

- schema-authority-followups
  - Retained By: Axiom
  - Responsibility: exact schema amendments for Schedule composition, canonical Workspace/operating-overview semantics, and first-class Role baseline specialization when sequenced by Anchor
  - Boundary: Loom may identify implementation needs but must not silently become canonical schema authority.

- sigma-durability
  - Retained By: Sigma
  - Responsibility: decide and execute the actual Git durability checkpoint after semantic/tooling/Anchor review gates pass
  - Boundary: no commit, push, merge, publication, or funding/business authority is transferred here.

## Exclusions And Dependencies

- no-business-lineage-rewrite
  - Kind: excluded-scope
  - Description: do not rewrite the current Business epic/Project/Role/Decision/Handoff graph in this Loom tranche.

- no-roadmap-or-process-authoring
  - Kind: excluded-scope
  - Description: do not author Roadmap, Milestone timing, operating Process, or funding/governance artifacts in this tranche.

- no-cache-cleanup
  - Kind: excluded-scope
  - Description: do not delete current Business `.topics/.cache` or predecessor artifacts before Anchor has post-checkpoint recovery evidence.

- preserve-provider-neutrality
  - Kind: unresolved-dependency
  - Description: Git/GitHub is the current adapter in many examples but must not become the only semantic recovery model.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return qualified implementation evidence for local Parent Origin support, recipient-v2 carrier purity, Handoff closure/workspace hygiene, and fixed-width carrier-dimension regression coverage; explicitly list any blocked item requiring Axiom schema authority before implementation can qualify.
- Return To: Anchor

## Interpretation Limits

- Does Not Mean: Business is merge-ready, `.topics/.cache` may now be deleted, Roadmap/Process should be authored, or Axiom schema amendments are complete.
- Must Not Be Used To Claim: repository publication, Git mutation, human acceptance, holder identity, or implementation outside the transferred Tooling scope.
- Authority Limits: Loom owns bounded shared/portable Tooling implementation and evidence return; Anchor retains architecture/review and Business graph repair; Axiom retains canonical schema semantics; Sigma retains human structural judgment and repository durability decisions.
- Transport Limits: package/workspace carriage is evidence and working context, not publication authority.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Anchor Consolidation Of Axiom Disposition And Loom Routing](../business-development/005-anchor-axiom-disposition-consolidation-and-loom-routing-decision.trace.md)
  - Value: tm2Q-2gre4AtvG61H8jPT5JlSQhDc78sacwdh_NffbE

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:gF41rfIfxYNZDJlmIV6L5irszVYGnkun8lpgpdu5l9o
