# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 15:29:46
  - Trace: [001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md](001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 15:32:03
  - Authors: Anchor
  - Why: The Core tranche is accepted; the remaining architecture-recovery implementation is host-owned and must be completed without recreating shared semantics or using Sigma as debugger.
  - Summary: Delegate the final implementation-ready VS Code host tranche against the accepted Core frontier, requiring real controller and Extension Host machine acceptance before Sigma.
  - Status: ready/local

---

# Anchor To Kodax — VS Code Core-Boundary Recovery And Extension Host Acceptance

## Handoff Parties

- Purpose: transfer the final implementation-ready architecture-recovery host tranche to Kodax against the exact Anchor-accepted Core frontier, with Sigma deliberately excluded until machine acceptance is complete.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- vscode-host-boundary-repair
  - Transfer Kind: work-and-responsibility
  - Description: implement the controlling Task in the carried Extension VS Code Workspace so the real Incoming/Replace/Outgoing/Attach/participant/Pack/Transport path consumes one Core-owned semantic/mechanical truth path, removes host-local participant weakening, and preserves fail-closed behavior.
  - Controlling Artifact: [VS Code Core-Boundary Recovery And Extension Host Acceptance](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
  - Boundary: Extension VS Code source and host-owned integration/test harness only; no Core or Docs semantic implementation is transferred.

- bounded-controller-decomposition
  - Transfer Kind: work
  - Description: reduce the operator controller hotspot only by extracting genuine VS Code-owned controllers/lifecycle responsibilities while removing duplicated shared semantic/mechanical rules from the host path.
  - Controlling Artifact: [VS Code Core-Boundary Recovery And Extension Host Acceptance](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
  - Boundary: no broad rewrite or file-size refactor detached from observable ownership/test improvements.

- machine-acceptance
  - Transfer Kind: work-and-responsibility
  - Description: establish controller-level and true VS Code Extension Host acceptance for the repaired Local and Published flows, including restart/requalification and negative fail-fast cases, and return blocked rather than synthesizing PASS if the real Extension Host gate cannot execute.
  - Controlling Artifact: [VS Code Core-Boundary Recovery And Extension Host Acceptance](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
  - Boundary: technical candidate qualification only; Kodax does not perform Sigma acceptance or release.

- return-evidence
  - Transfer Kind: responsibility
  - Description: return exact changed Extension VS Code source, qualified Evidence, exact test/Extension-Host receipts, residual risks, and one Kodax-to-Anchor Handoff declaring either candidate-for-anchor-reconciliation or blocked.
  - Controlling Artifact: [VS Code Core-Boundary Recovery And Extension Host Acceptance](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
  - Boundary: no remote mutation and no Sigma Handoff from Kodax.

## Required Context

- controlling-task
  - Material: exact current VS Code Core-Boundary Recovery And Extension Host Acceptance Task
  - Material Reference: [Controlling Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
  - Purpose: exact objective, Done Criteria, scope and boundaries
  - Availability: available

- core-acceptance
  - Material: Anchor Core Tranche Acceptance Decision
  - Material Reference: [Core Acceptance](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-anchor-core-tranche-acceptance.trace.md)
  - Purpose: exact accepted Core behavior and retained limitations that the host must consume without reinterpretation
  - Availability: available

- architecture-reconciliation
  - Material: Anchor Architecture Recovery Reconciliation Decision
  - Material Reference: [Architecture Reconciliation](business::.topics/processes/gpt/grounding/001-1-4-1-3-4-anchor-architecture-recovery-reconciliation.trace.md)
  - Purpose: accepted semantic/Core/host ownership split and sequencing boundary
  - Availability: available

- prior-kodax-audit
  - Material: Independent VS Code Host Boundary Audit returned by Kodax
  - Material Reference: [Kodax Host Audit](business::.topics/processes/gpt/grounding/001-1-4-1-3-3-1-independent-vs-code-host-boundary-audit-kodax-evidence.trace.md)
  - Purpose: independently observed host defects, architecture hotspots and missing acceptance coverage
  - Availability: available

- business-workspace
  - Material: reconciled current Business full-source Workspace carrying controlling authority and audit/acceptance lineage
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: coordination authority plus bounded Evidence/return-Handoff authoring surface
  - Availability: available

- core-workspace
  - Material: exact Anchor-accepted Core full-source Workspace returned by Loom
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: read-only shared Tooling/runtime source for Local binding and exact host contract
  - Availability: available

- extension-vscode-workspace
  - Material: exact current Extension VS Code full-source Workspace baseline
  - Material Reference: [Extension VS Code Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: writable implementation/test source for this Kodax tranche
  - Availability: available

- docs-workspace
  - Material: exact canonical Docs full-source Workspace
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: read-only canonical semantic/schema authority; do not reinterpret it in the host
  - Availability: available

## Reference Context

- loom-return-evidence
  - Material: Loom Core participant/preflight/carriage inspectability Evidence
  - Material Reference: [Loom Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-1-core-participant-preflight-and-carriage-inspectability-repair-lo.trace.md)
  - Purpose: technical details of the accepted Core changes and explicit full-suite limitation
  - Availability: available

- previous-sigma-signal
  - Material: durable prior host-flow Signal/Feedback already present in the Extension VS Code Workspace
  - Purpose: historical operator observations useful for regression targeting, not current acceptance authority
  - Availability: available

## Retained Responsibilities

- cross-return-reconciliation
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: compare the Kodax return against this exact carried source frontier, reconcile technical evidence with prior audits/Core acceptance, and decide whether a Sigma candidate exists.
  - Boundary: Kodax technical PASS does not self-promote to product acceptance.

- shared-core-semantics
  - Retained By: Loom / Axiom / Docs owners as applicable
  - Responsibility: shared Core mechanics and canonical semantic authority remain outside Kodax scope unless an exact capability gap is returned and separately delegated.
  - Boundary: Kodax must stop rather than privately recreate missing shared semantics.

- human-gate
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)
  - Responsibility: perform the later real operator/UX acceptance only after Anchor machine reconciliation.
  - Boundary: Sigma is not an implementation debugger in this tranche.

## Exclusions And Dependencies

- no-core-or-docs-mutation
  - Kind: excluded-scope
  - Description: Core and Docs are exact read-only dependencies in this Kodax lane; capability gaps return to Anchor rather than being patched privately.
  - Responsible Party Or Role: Anchor for rerouting; Loom/Axiom/Docs owners when separately delegated.

- real-extension-host-required
  - Kind: unresolved-dependency
  - Description: the environment must support a true VS Code Extension Host acceptance attempt for Sigma-candidate status; if it cannot, preserve the exact blocker and return `blocked` rather than substituting unit/package tests.
  - Responsible Party Or Role: Kodax for attempt/evidence; Anchor for disposition if environment prevents execution.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no push, release, publication, deployment or remote source mutation is authorized.
  - Responsible Party Or Role: Anchor / owning release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return one self-contained Kodax-to-Anchor carrier with exact changed Extension VS Code source, qualified technical Evidence, exact controller/Extension-Host acceptance receipts, known residual risks, and an explicit `candidate-for-anchor-reconciliation` or `blocked` disposition.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Kodax owns shared semantics, current tests are already sufficient, Extension Host acceptance may be simulated, Sigma is delegated, release is authorized, or a technical return is automatically accepted.
- Must Not Be Used To Claim: host-local participant edits create authority, persisted host state creates semantic truth, transport presentation may invent Handoff routing, Local mode may substitute Published binding, or narrow test PASS overrides the real controller/Extension Host gate.
- Authority Limits: exact bounded Extension VS Code implementation and technical qualification only; Anchor retains reconciliation/sequencing, Axiom/Docs retain semantics, Loom retains shared Core mechanics, Sigma retains the human gate.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md](001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
  - Value: hP5Nf8xrog4gwgHMk2jQPu1qbB22vEsxABza35ElMgs

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 8h0QIShLdoE6087nDYOC5KD2hGArStmcLyGKJanc3H4