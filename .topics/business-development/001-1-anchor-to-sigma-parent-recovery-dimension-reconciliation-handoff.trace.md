# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Business Development](001-business-development-project.trace.md)
  - Origin:
    - [relative](001-business-development-project.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-08-30 23:35:00
  - Authors: Anchor
  - Why: Deliver one full-source Business/Docs/Site candidate after Axiom recovery reconciliation, local dimension repair, `.tiinex` removal, and bounded Loom runtime qualification, so Sigma can inspect and land the candidate without chat-only context.
  - Summary: Anchor-to-Sigma full-source handoff for Parent recovery, local dimension, carrier policy, and Tooling reconciliation.
  - Status: ready/local

---

# Parent Recovery And Dimension Reconciliation — Sigma Handoff

## Handoff Parties

- Purpose: transfer the complete qualified local candidate to Sigma for human review, repository landing, and later Viewer observation while Anchor retains cross-role reconciliation and any follow-up repair routing
- From: Anchor
- From Kind: role
- To: Sigma
- To Kind: role

## Transfers

- candidate-source-review-and-landing
  - Transfer Kind: work-and-responsibility
  - Description: inspect the carried full-source Business, Docs, and Site workspaces; apply/commit/push the candidate if acceptable; preserve the supplied source boundaries and report any landing mismatch rather than silently repairing semantics during commit
  - Controlling Artifact: [Business Development](001-business-development-project.trace.md)
  - Boundary: Sigma owns the human apply/landing decision for this candidate; canonical schema meaning remains Axiom-owned, shared Tooling implementation remains Loom-owned, and Anchor retains architectural return review

- viewer-observation-after-landing
  - Transfer Kind: work
  - Description: after the source candidate is landed enough to test, compare the refactored Viewer and old PoC on the repaired cross-repository lineage/recovery behavior and return human observations
  - Boundary: Viewer observation is intentionally deferred until the recovery/dimension candidate is landed; this Handoff does not pre-claim product acceptance

## Required Context

- tiinex-business-full-source
  - Material: complete candidate `Tiinex/business` workspace, including repaired lineage/dimension decision, Handoff/cold-start task, and this Sigma Handoff
  - Purpose: organizational intent, local dimension/carrier policy, and final transfer authority
  - Availability: available

- tiinex-docs-full-source
  - Material: complete candidate `Tiinex/docs` workspace, including the corrected local Root schema, Axiom recovery discovery, renamed role-authority discovery, and removal of temporary `.tiinex` Parent copies
  - Purpose: canonical semantic candidate and exact Docs source for review/landing
  - Availability: available

- tiinex-site-full-source
  - Material: complete candidate `Tiinex/site` workspace, including local dimension repair, removal of temporary `.tiinex` Parent copies, local Root runtime projection, exact-authoring recovery mode, route conformance updates, and Loom completion Task
  - Purpose: shared Tooling/Viewer source plus focused qualification evidence
  - Availability: available

- focused-qualification
  - Material: candidate receipts from qualified-local Root runtime, runtime contract reconciliation, exact authoring, Parent authority coherence, local lineage authoring, route conformance, cross-repository source recovery, material closure, and multi-root manufacture tests
  - Purpose: prove the bounded semantic/runtime changes passed the focused relevant checks before Sigma transport
  - Availability: available

## Reference Context

- published-business-parent-baseline
  - Material: Business commit `3dac3b7ad41f307b1a3dcb70f0933f9e44a4fcd0`, used as the exact immutable Parent representation for repaired existing Docs/Site cross-repository children
  - Material Reference: [Business baseline](https://github.com/Tiinex/business/tree/3dac3b7ad41f307b1a3dcb70f0933f9e44a4fcd0)
  - Purpose: verify that repaired external Parent recovery points to already-published exact bytes rather than future/uncommitted authority
  - Availability: available

- current-publication-baselines
  - Material: Docs master baseline `9d849dc733753dddc09cef7192373698e1310ab5` and Site refactor baseline `e258f0b4792620c7ae16f6471e78af2e693c64ac`
  - Purpose: identify the source revisions from which this local candidate was prepared
  - Availability: available

## Retained Responsibilities

- cross-role-reconciliation
  - Retained By: Anchor
  - Responsibility: review Sigma return/landing evidence, reconcile any mismatch across Business, Docs, and Site, and route bounded semantic or Tooling follow-up to Axiom/Loom
  - Boundary: Anchor does not replace Sigma human acceptance or silently mutate remote repositories

- schema-semantics
  - Retained By: Axiom
  - Responsibility: own any further canonical Root/schema semantic correction exposed by landing or Viewer tests
  - Boundary: Sigma and Anchor may report evidence but do not redefine schema meaning during application

- shared-tooling
  - Retained By: Loom
  - Responsibility: own any further shared Tooling implementation correction exposed by the candidate or later scoped-export work
  - Boundary: current candidate deliberately does not claim scoped-export boundary augmentation is implemented

## Exclusions And Dependencies

- remote-mutation-by-anchor
  - Kind: excluded-scope
  - Description: Anchor must not use GitHub connector mutation as a substitute for Sigma-controlled local review/commit/push of this source candidate
  - Responsible Party Or Role: Anchor

- scoped-export-augmentation
  - Kind: unresolved-dependency
  - Description: future bounded artifact export must close any omitted Parent boundary through carried material, qualified version-stable recovery, scope expansion, or fail closed; the current recipient-v2 manufacture still carries complete workspace archives and does not claim this smaller-scope augmentation feature
  - Responsible Party Or Role: Loom

- viewer-product-acceptance
  - Kind: unresolved-dependency
  - Description: old PoC/refactored Viewer comparison and human product judgment happen after the recovery/dimension source is landed
  - Responsible Party Or Role: Sigma

## Completion Expectation

- Signal Kind: result
- Signal Meaning: return either landed commit/revision evidence for Business, Docs, and Site plus the requested Viewer observations when performed, or one concrete mismatch/blocker that prevents safe landing; do not treat package delivery alone as acceptance
- Return To: Anchor

## Interpretation Limits

- Does Not Mean: that the carried local Root candidate is already published, that historical published schema-source bindings were repinned, that scoped-export boundary augmentation is implemented, that Viewer behavior is accepted, or that Sigma must accept the candidate merely because focused tests passed
- Must Not Be Used To Claim: that local dimension coordinates replace Parent ancestry, that external Parent recovery requires vendored `.tiinex` copies, that all ordinary artifacts require `browse + git`, that a new carrier needs prior global carrier history, or that transport membership upgrades source bytes into canonical publication authority

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Business Development](001-business-development-project.trace.md)
  - Value: Q_HGxWfcvNP1KAiHfRXZr5Cmsju_6ouqUnvjOEeNJD4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: X2y0yWv7q_7NO2OUsb23SH7pmq5aVUTVht4fBXtPi7U
