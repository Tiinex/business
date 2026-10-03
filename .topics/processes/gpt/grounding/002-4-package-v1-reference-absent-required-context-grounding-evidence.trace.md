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
  - Created At: 2026-10-02 14:53:51
  - Authors: Anchor
  - Why: Durable-reference discovery found a Package V1 roundtrip gap inside existing Handoff and package contracts; preserve the reproduced defect, minimal Core fix and targeted qualification.
  - Summary: Qualified Core evidence that exact carried-Workspace Required Context can remain source-reference-free while Package V1 preserves its explicit package-local binding.
  - Status: ready/local

---

# Package V1 Reference-Absent Required Context Grounding Evidence

## Supported Claim Or Question

- Supported Claim Or Question: whether Package V1 can preserve an exact explicitly supplied carried-Workspace binding for Required Context when the source Handoff intentionally has no public `Material Reference`, without leaking Workspace-qualified runtime coordinates into the durable source artifact or inferring authority from package placement
- Evidence Role: bounded Core implementation and regression evidence for the durable-reference representation tranche under the Anchor grounding/recovery task; establishes this transport behavior only and does not establish a general Artifact Maintenance process

## Provenance

- Known Source: exact Business, Core and Docs Workspaces carried by `tiinex-011.handoff-package.zip`; the qualified `tiinex-011-1-anchor-to-anchor.handoff-package.zip` checkpoint manufactured earlier in this session; direct local inspection and execution against the carried modified Core source; no remote repository source was used as implementation authority
- Preservation Basis: the defect was reproduced in Package V1 manufacture/roundtrip behavior, the implementation delta was made only in the carried Core Workspace, and qualification used the targeted Package V1 test file plus physical roundtrip inspection
- Provenance Limits: no remote Git publication, merge, push, Marketplace action, Sigma acceptance or fresh-successor acceptance occurred in this tranche; broader Core qualification from the previous checkpoint was not rerun for this narrow representation delta

## Evidence Material

- Material: Package V1 now preserves exact explicitly bound Required Context even when the source Handoff has no `Material Reference`, by projecting a package-local grounding pointer whose public `Reference` remains empty and whose target is the exact carried Workspace/archive material. Package placement alone remains insufficient; an unbound reference-absent requirement still blocks. Existing Required Context with a real public reference retains the previous behavior and does not gain a redundant root grounding pointer.
- Material Kind: Core Package V1 implementation, regression and physical-roundtrip evidence

### Reproduced Representation Gap

- Previous Checkpoint Symptom: the prior Anchor recovery Handoff had to use `core::...` and `docs::...` `Material Reference` values solely so Package V1 could recover the exact carried Workspace bindings after physical roundtrip
- Semantic Concern: those values are useful runtime/material resolver coordinates but are not truthful durable repository authority and therefore should not be required in artifact-facing Handoff Markdown merely to express package carriage
- Root Cause: ordinary Required Context without a public reference did not receive a pre-Handoff grounding pointer even when manufacture input already contained an exact qualified material binding; only existing Process/Policy/runbook-like pre-Handoff categories were automatically projected

### Contract Classification

- Handoff Contract: `tiinex.handoff.v1` already permits Required Context without `Material Reference`
- Package Contract: Package V1 manufacture already accepts explicit qualified material bindings and Package V1 grounding pointers already carry `Requirement Id` plus exact package-local target identity
- Disposition: no schema expansion or new locator syntax is required for this case; the defect is a Core manufacture/roundtrip implementation gap inside existing contracts

### Core Delta

- Projection Rule: a package-local grounding pointer is added when and only when the Required Context has no public `Material Reference` and exact qualified material is already bound to that requirement
- Public Reference Boundary: the generated pointer keeps its public `Reference` empty; the exact package-local Workspace/archive target and integrity carry the transport grounding
- No Inference Rule: reference-absent Required Context without an exact explicit material binding remains blocked; package placement, Workspace id and filename do not become semantic authority
- Existing Reference Boundary: Required Context with a durable/public source reference retains previous closure behavior and does not gain a redundant root pointer merely because its material is carried

### Targeted Qualification

- Command: `node --test test/handoff-package-v1.test.mjs`
- Result: 42 of 42 tests passed; 0 failed
- New Positive Regression: reference-absent Required Context with an explicit carried-Workspace binding survives manufacture, inspection and physical roundtrip with empty public `Reference` and exact package-local target identity
- New Negative Regression: the same reference-absent Required Context remains blocked when no exact binding is supplied; package placement is not used to infer it
- Existing Boundary Regressions: ordinary durable-reference Required Context remains non-root closure material; Package V1 continues to reject Workspace-qualified coordinates as public Pointer Reference values

### Process Dogfood

- Current Work Form: bounded proto-process `invariant -> reproduction -> regression -> smallest owning-boundary fix -> targeted qualification -> Handoff Package`
- Repetition Signal: this is a second concrete maintenance-style tranche using essentially the same lifecycle after the material-identity tranche
- Durable Process Status: the repetition is evidence for a future maintenance routine, but this Evidence does not itself establish or name a new Process

## Preservation And Fidelity

- Preservation State: the implementation and tests are present in the carried Core Workspace; this Evidence is intended to be authored into the Business Workspace and included in the next recovery Handoff Package
- Fidelity Notes: runtime carriage coordinates are distinguished from durable artifact authority; package-local grounding is recorded as transport evidence rather than rewritten into a new public locator scheme
- Known Losses: historical `workspace::` occurrences outside this exact Package V1 case remain unclassified; no mass Repair has been attempted and no broader artifact-family acceptance is claimed

## Interpretation Limits

- Does Not Prove: that every `workspace::` occurrence is invalid, that all durable-reference classes should omit `Material Reference`, that a new durable locator scheme exists, that package placement establishes authority, or that the wider grounding program has passed cold-successor acceptance
- Not Yet Used As: authority to mass-rewrite historical Workspaces, a reason to alter Handoff schemas, or acceptance of a general Artifact Maintenance process
- Must Not Be Treated As: permission to infer Required Context bindings from filenames/package placement, permission to expose package-local Workspace coordinates as public Pointer Reference values, or a substitute for canonical Handoff Package transport

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md](002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
  - Value: jTVFgwCW8ZihcSXR6y7vNZDtvpyMCtrgznqd_tVN5vk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 60KfNvffrPtbj0yCPkv2P6fLZ2xhwIp0BqdmXVwQ_kk