# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.evidence.v1
  - Created At: 2026-09-26 21:30:56
  - Trace: [005-vs-code-re-entry-shared-core-human-parity-bridge-merge-candidate.trace.md](../../processes/gpt/vscode-reentry/005-vs-code-re-entry-shared-core-human-parity-bridge-merge-candidate.trace.md)
  - Origin:
    - [relative](../../processes/gpt/vscode-reentry/005-vs-code-re-entry-shared-core-human-parity-bridge-merge-candidate.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-26 21:31:11
  - Authors: Anchor
  - Why: Deliver the exact locally qualified candidate to Sigma for real VS Code testing and merge disposition.
  - Summary: Full five-Workspace VS Code shared-Core bridge merge/test candidate for Sigma real-host acceptance.
  - Status: ready/local

---

# Anchor To Sigma — VS Code Shared-Core Human-Parity Merge Candidate

## Handoff Parties

- Purpose: deliver the exact full five-Workspace VS Code bridge candidate to Sigma for real VS Code Extension Host/manual TreeView acceptance and merge disposition after the bounded local shared-Core qualification passed.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)

## Transfers

- vscode-shared-core-human-parity-merge-candidate
  - Transfer Kind: work-and-responsibility
  - Description: inspect and test the exact carried VS Code bridge candidate against the exact carried frozen Core in a real VS Code host. The intended product boundary is one Core Tooling semantics path consumed by Tiinex/LLMs, human VS Code UI, and later native VS Code tool exposure; this Handoff does not authorize a parallel VS Code semantics path.
  - Controlling Artifact: [VS Code shared-Core merge candidate Evidence](../../processes/gpt/vscode-reentry/005-vs-code-re-entry-shared-core-human-parity-bridge-merge-candidate.trace.md)
  - Boundary: Sigma owns final product acceptance and merge/commit/push disposition. If testing reveals a concrete blocker, return that blocker without compensating in Core or reviving V2/legacy logic.

## Required Context

- qualification-evidence
  - Material: exact final local technical qualification and environment boundary for this VS Code candidate.
  - Material Reference: [VS Code shared-Core merge candidate Evidence](../../processes/gpt/vscode-reentry/005-vs-code-re-entry-shared-core-human-parity-bridge-merge-candidate.trace.md)
  - Purpose: tells Sigma exactly what was changed, what passed locally, what remains a real-host gate, and which semantic boundaries must remain intact.
  - Availability: available

- preceding-vscode-recovery
  - Material: immediately preceding Core-frozen VS Code grounding bridge recovery Handoff.
  - Material Reference: [preceding recovery](008-anchor-to-anchor-core-frozen-vs-code-grounding-bridge-recovery.trace.md)
  - Purpose: preserves the checkpoint lineage and explicit rule that Core blockers must be discussed with Sigma before Core modification.
  - Availability: available

- business-workspace
  - Material: exact current Business Workspace with orchestration/recovery lineage, final qualification Evidence, and this Handoff.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: durable recovery and work-control context.
  - Availability: available

- core-workspace
  - Material: exact frozen Core Workspace accepted after Package V1 topology, grounding, completion and return qualification hardening.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: semantic/tooling owner against which the VS Code bridge is tested; this candidate does not modify it.
  - Availability: available

- vscode-workspace
  - Material: exact current VS Code source candidate including endpoint authoring parity, Incoming grounding presentation, canonical fixtures, multi-route Pack correction, and updated acceptance coverage.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: source candidate Sigma may test and merge if accepted.
  - Availability: available

- app-workspace
  - Material: exact preserved App Workspace.
  - Material Reference: [App Workspace](app::.topics/.workspaces/tiinex-app.workspace.md)
  - Purpose: full recovery/shared-consumer context; no App implementation delta is claimed here.
  - Availability: available

- docs-workspace
  - Material: exact preserved Docs Workspace.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: canonical schema/validator context; no Docs implementation delta is claimed here.
  - Availability: available

## Reference Context

- core-closure
  - Material: qualified Core Package V1/return closure that remains frozen under this VS Code candidate.
  - Material Reference: [Core closure Evidence](../../processes/gpt/vscode-reentry/002-1-1-vs-code-re-entry-core-package-v1-topology-and-return-qualificati.trace.md)
  - Purpose: preserve why VS Code consumes Core rather than adding compatibility semantics.
  - Availability: available

## Retained Responsibilities

- anchor-blocker-recovery
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: investigate any concrete blocker Sigma returns from real-host testing, preserving the Core-frozen rule unless Sigma explicitly agrees that a demonstrated Core blocker justifies reopening it.
  - Boundary: Anchor does not infer acceptance or remote landing from delivery of this package.

## Exclusions And Dependencies

- core-frozen
  - Kind: excluded-scope
  - Description: do not change Core merely to accommodate VS Code legacy assumptions. A genuine Core blocker must be demonstrated and discussed with Sigma before Core changes.
  - Responsible Party Or Role: Anchor / Sigma

- no-v2-or-legacy-revival
  - Kind: excluded-scope
  - Description: do not restore Handoff Package V2, old host-owned package/lineage/grounding logic, compatibility fallbacks, label-to-reference inference, or duplicate semantic paths.
  - Responsible Party Or Role: Anchor / Sigma

- real-vscode-host-gate
  - Kind: unresolved-dependency
  - Description: run the candidate in a real VS Code host with the carried local Core. The automated host suite is `npm run test:extension-host -- --mode local --local-core ../core --restarts 2` after normal development dependencies are available; manual TreeView review should focus on Discovery, Incoming, Outgoing and Transport behavior and the human-parity flows represented there.
  - Responsible Party Or Role: Sigma

- merge-disposition
  - Kind: unresolved-dependency
  - Description: if the real-host/manual behavior is accepted, Sigma decides and performs the desired commit/merge/push. If not accepted, return one concrete reproducible blocker against this exact carried candidate.
  - Responsible Party Or Role: Sigma

## Completion Expectation

- Signal Kind: disposition
- Signal Meaning: Sigma tests this exact carried candidate in real VS Code, then either accepts it and performs the intended merge/commit/push disposition or returns one concrete blocker with the observed workflow and failure boundary so Anchor can resume from this full recovery without chat reconstruction.
- Return To: Anchor
- Return To Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: the candidate is already merged or pushed, published Core has been updated, real-host acceptance has already passed, future native Copilot tool exposure is implemented, or Sigma acceptance is implied by local tests.
- Must Not Be Used To Claim: remote mutation before Sigma performs it, permission to reopen Core without a concrete reviewed blocker, or permission to create a second Tiinex semantic/tooling path in VS Code.
- Transport Limits: normal delivery is this canonical five-Workspace Handoff Package plus its Tooling-projected transport text; generated VSIX/test receipts are not parallel source deliverables.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [005-vs-code-re-entry-shared-core-human-parity-bridge-merge-candidate.trace.md](../../processes/gpt/vscode-reentry/005-vs-code-re-entry-shared-core-human-parity-bridge-merge-candidate.trace.md)
  - Value: -tTDBBKbDH2ADd11p_QM3doXX-vrH_2RLevaXcNOj1Q

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: fbMhqa_Qnj0M8YtpuKsgxs-fhWzfgt_L77q77eM87OA