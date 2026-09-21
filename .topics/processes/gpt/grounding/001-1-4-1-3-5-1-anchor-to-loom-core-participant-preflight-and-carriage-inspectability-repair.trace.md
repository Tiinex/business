# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 14:32:55
  - Trace: [001-1-4-1-3-5-core-participant-preflight-and-carriage-inspectability-repair.trace.md](001-1-4-1-3-5-core-participant-preflight-and-carriage-inspectability-repair.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-core-participant-preflight-and-carriage-inspectability-repair.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 14:33:37
  - Authors: Anchor
  - Why: Independent audits are reconciled and the first implementation tranche is now bounded to shared Core mechanics with explicit semantic and host exclusions.
  - Summary: Delegate the reconciled Core participant-integrity, fail-fast preflight, and detached-material inspectability tranche to Loom.
  - Status: ready/local

---

# Anchor To Loom — Core Participant, Preflight, And Carriage Inspectability Repair

## Handoff Parties

- Purpose: implement the first Core-owned architecture-recovery tranche after independent Axiom/Loom/Kodax reconciliation, without semantic widening or VS Code mutation.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Loom
- To Kind: role
- To Reference: [Loom Role](business::.topics/roles/001-3-1-loom-canonical-holder-cutover-role.trace.md)

## Transfers

- core-participant-authority-repair
  - Transfer Kind: work-and-responsibility
  - Description: make semantic participant derivation depend on exact qualified current-work Task schema and self-integrity; stale, tampered, or otherwise unqualified Task material must yield no semantic participant requirement and an explicit blocking finding.
  - Controlling Artifact: [Core Repair Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-core-participant-preflight-and-carriage-inspectability-repair.trace.md)
  - Boundary: do not broaden participant authority; manual input, Role/cache inventory, endpoint labels, package proximity, filenames, and host state remain non-authoritative.

- core-fail-fast-preflight
  - Transfer Kind: work
  - Description: hoist blocking selected-Handoff/current-work/material qualification ahead of bootstrap archive construction and recipient package assembly wherever the same facts are already available, with seam-level proof that blocked inputs do not enter expensive builders.
  - Controlling Artifact: [Core Repair Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-core-participant-preflight-and-carriage-inspectability-repair.trace.md)
  - Boundary: failure timing only; package success semantics and Required-versus-Reference Context behavior must not change.

- detached-material-inspectability
  - Transfer Kind: work
  - Description: improve recipient inspectability of detached textual carried material using deterministic safe source-shaped entry identities/media representation or an equivalent transparent projection while preserving exact bytes, digest, provenance, bounded scope, deduplication, and semantic non-authority.
  - Controlling Artifact: [Anchor Reconciliation](business::.topics/processes/gpt/grounding/001-1-4-1-3-4-anchor-architecture-recovery-reconciliation.trace.md)
  - Boundary: no cache-to-Workspace-Representation semantic reclassification, no new Handoff semantics, and no Party Capacity closure widening.

## Required Context

- core-repair-task
  - Material: Core Participant, Preflight, And Carriage Inspectability Repair Task.
  - Material Reference: [Core Repair Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-core-participant-preflight-and-carriage-inspectability-repair.trace.md)
  - Purpose: exact implementation scope, done criteria, exclusions, and acceptance boundary.
  - Availability: available

- anchor-reconciliation
  - Material: Anchor Architecture Recovery Reconciliation Decision.
  - Material Reference: [Anchor Reconciliation](business::.topics/processes/gpt/grounding/001-1-4-1-3-4-anchor-architecture-recovery-reconciliation.trace.md)
  - Purpose: authoritative reconciliation of Axiom/Loom/Kodax audit results and sequencing constraints.
  - Availability: available

- axiom-semantic-disposition
  - Material: Axiom Semantic Boundary Disposition — Handoff Endpoints, References, And Carried Material.
  - Material Reference: [Axiom Disposition](business::.topics/processes/gpt/grounding/001-1-4-1-3-1-1-axiom-semantic-boundary-disposition-handoff-endpoints-references.trace.md)
  - Purpose: canonical semantic boundaries that Core implementation must preserve.
  - Availability: available

- loom-audit-evidence
  - Material: Independent Core Material And Packing Audit — Loom Evidence.
  - Material Reference: [Loom Audit Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-2-1-independent-core-material-and-packing-audit-loom-evidence.trace.md)
  - Purpose: exact source-proven defect, fail-timing seam, non-defects, and minimum acceptance surface.
  - Availability: available

- core-workspace
  - Material: exact current Core full source snapshot carried from the qualified Loom audit return.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: writable implementation source for the delegated Loom tranche.
  - Availability: available

- docs-workspace
  - Material: exact current canonical Docs snapshot carried from the qualified Loom audit return.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: read-only semantic/schema authority while preserving the accepted no-schema-change boundary.
  - Availability: available

## Reference Context

- kodax-host-audit
  - Material: Kodax VS Code Host Boundary Audit Evidence.
  - Material Reference: [Kodax Audit Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-3-1-kodax-vs-code-host-boundary-audit-evidence.trace.md)
  - Purpose: explains downstream host seams that Core must not accidentally absorb while repairing shared mechanics.
  - Availability: available

## Retained Responsibilities

- architecture-reconciliation
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: consume Loom return, verify exact source/evidence against this Task, and decide whether the Core tranche is accepted before any Kodax implementation proceeds.
  - Boundary: Loom implementation qualification does not become program acceptance automatically.

- vscode-host-correction
  - Retained By: Kodax
  - Retained By Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)
  - Responsibility: VS Code participant immutability, controller thinning, restart/requalification contract, and real Extension Host acceptance after Anchor accepts the Core return.
  - Boundary: not active in this Handoff.

- human-gate
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)
  - Responsibility: final real operator/UX gate only after cross-layer machine acceptance.
  - Boundary: Sigma is not an implementation debugger for this tranche.

## Exclusions And Dependencies

- no-docs-schema-change
  - Kind: excluded-scope
  - Description: no canonical Handoff endpoint/kind, resolver-state, capacity, package, or Workspace Representation schema mutation is authorized.

- no-party-capacity-closure-widening
  - Kind: excluded-scope
  - Description: do not make Party Capacity/Capacity Reference material automatically mandatory for package closure.

- no-vscode-mutation
  - Kind: excluded-scope
  - Description: Extension VS Code remains frozen until Anchor reconciles the Loom return.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no release, publication, deployment, push, or other remote mutation is authorized.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return one qualified Loom-to-Anchor Handoff carrying exact changed Core source, tests, evidence, stated environment limitations, and any blocker that prevents the Task Done Criteria from qualifying.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Axiom semantics may be revised, `.bin` presence is itself a semantic defect, every detached material item must become a Workspace Representation, Party Capacity closure must widen, VS Code may be edited, or successful focused tests imply program acceptance.
- Must Not Be Used To Claim: participant authority from transport/cache presence, durable semantic References from internal binding keys, semantic applicability from exact carried bytes, host acceptance, Sigma acceptance, release readiness, or remote write authority.
- Authority Limits: bounded Loom/Core implementation under the exact Task and Anchor reconciliation only; canonical semantics, host implementation, cross-return acceptance, and human gate remain with their declared owners.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-core-participant-preflight-and-carriage-inspectability-repair.trace.md](001-1-4-1-3-5-core-participant-preflight-and-carriage-inspectability-repair.trace.md)
  - Value: VqWQSVmQhbxUP-q5_9C6Lo-Wvtx8b9uQCpoOt8U9Crs

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: tlw-pgxfi98q591KT2IJsJfkSw1RdghEXugvAu1EN_E