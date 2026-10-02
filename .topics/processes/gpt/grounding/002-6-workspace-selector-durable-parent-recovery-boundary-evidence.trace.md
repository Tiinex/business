# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-12 19:09:24
  - Trace: [002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md](002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
  - Origin:
    - [relative](002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
- Current
  - Current Schema: [tiinex.evidence.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/evidence/tiinex.evidence.v1.schema.md)
  - Created At: 2026-10-02 15:24:49
  - Authors: Anchor
  - Why: The transferred workspace-selector representation tranche is now grounded against the existing Root contract and targeted-qualified in Core; preserve the exact invariant, implementation delta, regressions and process-dogfood result.
  - Summary: Qualified evidence separating runtime Workspace selectors from durable Parent recovery for new candidates while preserving historical material without fabricated Repair.
  - Status: ready/local

---

# Workspace Selector And Durable Parent Recovery Boundary Evidence

## Supported Claim Or Question

- Supported Claim Or Question: whether a Workspace-qualified coordinate such as `business::path` may be persisted as the truthful durable Parent recovery locator for a newly authored cross-Workspace artifact, or whether it must remain runtime/material selection identity while durable recovery uses a separate qualified version-stable locator
- Evidence Role: bounded Core implementation and process-dogfood evidence completing the `workspace::path` representation tranche transferred by the preceding Anchor checkpoint

## Provenance

- Known Source: exact Business, Core and Docs Workspaces carried through the qualified `tiinex-011-1-1-anchor-to-anchor.handoff-package.zip` checkpoint; current local Core implementation and tests; current Docs Root schema and Schema Development process; no remote repository state is used as implementation authority for this tranche
- Preservation Basis: the semantic boundary was recovered from current Docs contract before implementation, stale Core authoring/Repair behavior was reproduced, the smallest prospective Core owners were changed, and qualification used only directly affected regression files plus CLI dogfood
- Provenance Limits: no historical artifact mass rewrite, remote Git publication, merge, push, Marketplace action, cold-successor acceptance or full Core-suite rerun occurred in this tranche

## Evidence Material

- Material: new cross-Workspace authoring now treats `workspace::path` as runtime/material selection identity only; persisted Parent recovery requires an explicit qualified version-stable locator. Candidate validation blocks source artifacts that persist Workspace-qualified Parent recovery, while historical audit remains preservation-oriented. Editor assistance no longer fabricates a deterministic Repair from malformed `../../workspace::path` to `workspace::path` when no exact durable replacement is proven.
- Material Kind: Docs-contract reconciliation, Core authoring/validation/Repair implementation, targeted regression and CLI-dogfood evidence

### Process Classification

- Existing Process: Tiinex Schema Development was used to determine whether the representation conflict required a Root schema revision
- Recovered Contract: Root already requires `relative` Parent recovery to be directly recoverable in the same qualified materialization and source scope; otherwise a qualified version-stable recovery locator is required. Transport/package closure may augment recovery but must not forge source Parent authority.
- Process Disposition: stop before schema authoring because the current Root contract already expresses the required invariant; no Docs schema revision or new locator syntax is justified
- Implementation Owner: Core forward-authoring, candidate qualification and deterministic Repair behavior under the existing contract

### Reproduced Core Divergence

- Shared/Editor Authoring: `projectPortableAuthoringParent` previously accepted a Workspace-qualified selector as `recoveryMode: workspace-qualified`, allowing the selector to be rendered into Parent Trace/Origin
- Common CLI: already required `--parent-reference` for cross-Workspace Parent authoring and rendered the supplied immutable external recovery locator
- Candidate Qualification: historical Root validation rejected malformed mixed forms such as `../../business::...` but did not distinguish a valid runtime Workspace selector from a truthful durable recovery locator for a new persisted candidate
- Editor Repair: deterministic reference hygiene stripped relative prefixes from malformed Workspace-qualified Parent targets and offered the resulting runtime selector as if it were a durable repair

### Core Delta

- Shared Parent Projection: Workspace-qualified Parent selection now requires an explicit qualified version-stable published recovery reference; otherwise projection blocks with `portable.authoring-parent.published-reference.required`
- Durable Rendering: with exact published recovery supplied, selection identity may remain `business::path` internally while `recoveryMode` is `external-versioned` and the rendered Parent Trace/Origin use only the immutable recovery locator
- Candidate Guardrail: `validateArtifact(..., schemaReferenceContext: 'candidate')` now emits `root.parent.recovery.workspace-qualified.non-durable` for persisted Workspace-qualified Parent Trace/Origin; historical context does not add that prospective finding
- Repair Boundary: deterministic editor reference hygiene no longer rewrites malformed Workspace-qualified Parent recovery into a runtime selector. Historical malformed debt remains diagnosable but receives no deterministic Parent replacement absent exact durable recovery evidence
- Shared Version-Stable Predicate: CLI and editor authoring use one Core-owned commit-pinned GitHub recovery-locator predicate rather than independent local checks

### Targeted Qualification

- Direct Regression: `node --test test/authoring-target-parent.test.mjs` passed 17 of 17 tests
- Impact Batch: `node --test test/authoring-target-parent.test.mjs test/canonical-role-authoring-cutover.test.mjs test/identifier-only-historical-role-parent-authoring.test.mjs test/manufacture-hygiene.test.mjs` passed 42 of 42 tests
- Positive Authoring Regression: Workspace selector plus immutable recovery locator produces a clean child whose persisted Parent recovery contains the immutable locator and no `business::` token
- Negative Authoring Regression: the same Workspace selector without durable recovery locator is blocked before authoring
- Candidate Regression: manually preserved historical Workspace-qualified recovery remains non-destructively readable historically but is blocking when evaluated as a new candidate
- Repair Regression: malformed historical Workspace-qualified Parent recovery remains visible as debt and no longer receives the old `repair-qualified-references-and-self-integrity` normalization action solely by stripping path prefixes
- Historical Role Regression: real identifier-only and pre-migration Role Parent continuation remains qualified when exact Parent bytes and explicit durable Parent reference are supplied

### CLI Dogfood

- Without Durable Locator: `project-authoring-parent` on the current Business Handoff using a `business::...` selector returned `blocked` with `portable.authoring-parent.published-reference.required`
- With Durable Locator: the same exact Parent bytes and selector plus a commit-pinned `--parent-reference` returned `ready`, preserved the Workspace selector only as internal Parent identity/path, and projected `recoveryMode: external-versioned`
- Boundary: CLI dogfood used local carried bytes and a syntactically qualified test permalink to exercise projection semantics; it did not claim remote publication of the local checkpoint

### Process Dogfood

- Repeated Lifecycle: invariant recovery -> reproduce conflicting paths -> test prospective/historical asymmetry -> smallest Core-owner fix -> direct regression -> narrow impact batch -> canonical Handoff Package checkpoint
- Efficiency Observation: direct tests were run during implementation and the broader 42-test batch was deferred until the tranche gate; the full Core suite was intentionally not rerun
- Process Signal: material-identity, Package V1 carriage and durable Parent-recovery work have now repeated substantially the same maintenance lifecycle across distinct Core artifact/reference families; this is stronger evidence for a future bounded maintenance routine, but does not itself create or accept one

## Preservation And Fidelity

- Preservation State: exact implementation and regression bytes are carried in the Core Workspace; current Business coordination artifacts and Docs contract/process context remain in their respective Workspaces
- Fidelity Notes: runtime/material selection, durable source recovery, package-local carriage and historical preservation are kept as distinct concepts; no one representation is promoted into another by convenience
- Known Losses: existing historical `workspace::` references across carried Workspaces remain unclassified individually; some may be legitimate historical representation debt and some may have exact provable replacements, but no bulk disposition is claimed here

## Interpretation Limits

- Does Not Prove: that all historical `workspace::` occurrences are invalid, that every external Parent must use GitHub specifically in perpetuity, that package-local pointers are source authority, or that a general Artifact Maintenance Process has been accepted
- Not Yet Used As: authority to mass-rewrite historical Business/Core/Docs artifacts, delete old carrier lineage, or infer immutable recovery locators without exact evidence
- Must Not Be Treated As: a reason to revalidate historical bytes under prospective candidate rules, a host-local semantic fork, or a substitute for canonical Handoff Package transport

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md](002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
  - Value: mK4JerPYAZOZ_kE5IiYaXyvvMaJG088uZtuBc-a9VBw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: iQgxKk60oQIKRjTpgxMTQ4gBgjAFzWTBqwfg3KvAT20