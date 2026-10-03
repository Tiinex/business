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
  - Created At: 2026-10-02 14:23:24
  - Authors: Anchor
  - Why: The current grounding/recovery tranche reproduced a shared Core validity defect where repository-tip freshness could create artificial schema/reference churn; durable Evidence is required before recovery transfer.
  - Summary: Verified Core material-equivalence semantics now prevent commit-freshness-only schema churn across published sync, reference qualification, editor/audit and manufacture preflight while preserving actual-change and historical-Parent boundaries.
  - Status: ready/local

---

# Core Material Identity And Commit-Freshness Qualification Evidence

## Supported Claim Or Question

- Supported Claim Or Question: whether Tiinex Core can distinguish exact schema material identity from repository-tip commit freshness so that an older immutable schema locator remains semantically valid when it still denotes the exact intended material, while actual material change still produces a qualified mismatch and update path
- Evidence Role: bounded implementation and regression evidence for the current Anchor grounding/recovery task; establishes the verified Core behavior reached in this tranche without claiming broader Artifact Maintenance process acceptance or host-product acceptance

## Provenance

- Known Source: exact Core, Docs and Business Workspaces carried by `tiinex-011.handoff-package.zip`; direct local inspection and execution against the carried Core source; a pristine Core extraction from the same carrier used for regression classification; the prior Anchor recovery note and Sigma video were treated only as non-authoritative hypothesis/grounding aids and are not needed to support the verified implementation claims recorded here
- Preservation Basis: the implementation delta was made only in the carried Core Workspace; baseline behavior was reproduced against the pristine carried Core where needed; qualification was executed against the modified carried Core without remote mutation or repository-tip inference
- Provenance Limits: no remote Git publication, merge, push, Marketplace action, Sigma acceptance or independent fresh-successor acceptance occurred in this tranche; a single-invocation `npm test` run exceeded the local execution time boundary and is not represented as a completed full-suite run

## Evidence Material

- Material: Core now owns one cryptographic material-equivalence predicate for schema material and uses it across published schema synchronization, schema-reference qualification, editor/audit projection and Handoff manufacture preflight. Published schema synchronization preserves a previously qualified immutable publication binding when repository/path and exact material remain equivalent despite a newer Docs commit; actual schema-byte change rebinds the changed schema while unchanged siblings preserve their prior valid immutable bindings. An older immutable schema locator can qualify as equivalent only when explicit resolution evidence proves matching cryptographic material at the same canonical repository/source path; equivalent bytes at a different canonical source coordinate remain blocked. Historical Parent semantics remain separate and continue to preserve the exact inherited Parent representation rather than upgrading to a newer same-path revision.
- Material Kind: Core implementation, regression and qualification evidence

### Reproduced Baseline Defect

- Published Schema Sync Baseline: with unchanged schema bytes and a newer Docs commit, the carried Core rebound publication metadata/permalinks to the newer commit even though material identity was unchanged
- Candidate Validation Baseline: shared schema-reference candidate qualification recognized only the registry authority's current exact target, so an older immutable same-material locator could remain `target-unqualified` even when editor-side host resolution independently proved byte identity and therefore offered no stale Repair
- Consequence: commit freshness could create artificial publication/reference churn and split editor, validator and manufacture behavior around the same semantic material

### Core-Owned Invariant

- Invariant: repository commit freshness is not semantic validity; exact qualified material identity is the deciding evidence once canonical repository/source-path identity is preserved
- Shared Predicate: schema material equivalence compares cryptographic identity evidence while deliberately excluding commit freshness from equivalence
- Authority Guardrail: byte identity alone cannot authorize an arbitrary copy; equivalent-locator qualification requires the observed immutable locator to preserve the canonical repository and source path before material equivalence can qualify it
- Authoring Boundary: a preferred/current locator may still be used for new authoring, while an older immutable locator that continues to denote the exact intended material is not stale or repairable merely because a newer commit exists
- Parent Boundary: this schema-material rule does not upgrade historical Parent Trace references; a child remains bound to the exact historical Parent representation it inherited

### Implementation Surface

- Schema Sync: published sync reuses materially equivalent existing bindings for generic and specialized schemas and propagates preserved bindings through runtime schema projections; whole-snapshot source commit is preserved only when the full schema snapshot is materially unchanged
- Schema Material Identity: shared Core predicate normalizes SHA-256 and Git blob identity evidence, rejects contradictory shared evidence and rejects schema-identity contradiction
- Schema Reference Qualification: explicit resolution evidence can augment a qualified authority with one equivalent older immutable target only when canonical repository/path and cryptographic material identity agree
- Audit And Editor Assistance: shared audit receives the same explicit schema-reference resolutions used by editor assistance, preventing editor-clean / validator-blocked divergence for proven equivalent material
- Handoff Manufacture Preflight: manufacture preflight can consume the same explicit schema-reference resolution evidence; it does not invent material-equivalence evidence when none is supplied

### Regression Qualification

- Published Sync / Reference / Editor / Manufacture Targeted Tests: 38 of 38 passed after the final authority guardrail and manufacture-preflight alignment
- Wider Package / Endpoint / Source-Frontier / Historical-Parent Regression Group: 99 of 99 passed
- Core Test Files: all 49 `test/*.test.mjs` files completed with green results across deterministic batches
- Portable Smoke: `npm run test:portable` passed
- Bootstrap Self-Check: `npm run test:bootstrap` passed with embedded-qualified status
- Package Dry Run: `npm run pack:check` passed and produced a valid dry-run package projection
- Single-Invocation Full Suite Boundary: one `npm test` invocation ran without observed failure until the environment time limit while still progressing; it is not counted as completed full-suite evidence because it did not terminate normally

### Pre-Existing 011 Test Classification

- Observed Failure: `test/recipient-return-ux.test.mjs` expected shell presentation with quotes around a safe temporary path while current Tooling projected the same structured invocation without unnecessary quotes
- Baseline Verification: the identical failure reproduced in the pristine Core extracted from `tiinex-011`, proving it was pre-existing rather than introduced by the material-identity delta
- Maintenance Delta: the test now asserts the structured invocation arguments and current safe CLI projection; no Tooling runtime behavior changed for this maintenance correction

### Process Disposition

- Current Work Form: bounded proto-process under the controlling Anchor grounding/recovery task: invariant -> reproduction -> regression -> minimal Core fix -> qualification -> Handoff Package
- Existing Process Precedent: historical Artifact Hygiene / Forward Authoring Guardrails material is useful precedent but its completed lane is not reactivated by similarity alone
- Durable Process Status: no new Artifact Maintenance or Process Development process is established by this Evidence; this tranche is one real dogfood instance that may contribute to such a process only if the lifecycle repeats stably across additional artifact families

## Preservation And Fidelity

- Preservation State: exact implementation and tests are present in the carried Core Workspace that will be included in the recovery Handoff Package; this Evidence is authored into the Business Workspace as the durable decision-relevant record
- Fidelity Notes: verified implementation claims are separated from the non-authoritative recovery hypotheses that motivated discovery; full-file test completion is reported separately from the timed-out single-invocation suite run
- Known Losses: no independent fresh successor has yet been used to verify that the improved invariant and surrounding process reduce grounding correction turns; no remote CI run is represented here

## Interpretation Limits

- Does Not Prove: that all durable-reference classes share identical material-equivalence semantics, that `workspace::` representation leakage is resolved, that every fixture/reference churn source is eliminated, that an Artifact Maintenance process is ready for adoption, that Entry/Session Entry grounding is accepted, or that any VS Code/Marketplace candidate has human acceptance
- Not Yet Used As: acceptance of the next `workspace::` representation-leakage tranche, a reason to mass-rewrite historical artifacts, or authority to refresh historical Parent references to newer revisions
- Must Not Be Treated As: permission to equate byte identity with authority across different repositories/paths, proof that repository-tip freshness is irrelevant for all authoring choices, or permission to bypass qualified Tiinex Handoff Package transport

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md](002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
  - Value: u5Eeneq_nOYGUxMTRXZf3vIU3fNICFT6SPDH--OYZJA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: mklRTRNBV0X1GfSEClO_fXPwkBtDZhpk7fKvehLOewA