# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 16:23:10
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 16:24:46
  - Authors: Anchor
  - Why: The bounded host repair is accepted for continuation, but the current Extension Host suite is unexecuted and insufficiently broad for Sigma-candidate status.
  - Summary: Delegate only the remaining real Local/Published VS Code Extension Host machine-acceptance gate before Sigma.
  - Status: ready/local

---

# Anchor To Kodax — Extension Host End-To-End Acceptance Completion

## Handoff Parties

- Purpose: complete the single remaining pre-Sigma machine-acceptance gap for the already-accepted VS Code host repair without reopening general implementation scope.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md)

## Transfers

- extension-host-machine-gate
  - Transfer Kind: work-and-responsibility
  - Description: complete and execute the real VS Code Extension Host operator-flow acceptance under exact Local Core and lock-qualified Published Core, using the already-accepted Kodax host repair as the candidate source.
  - Controlling Artifact: [Extension Host End-To-End Acceptance Completion](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md)
  - Boundary: acceptance completion first; mutate product source only when the real host gate exposes one exact bounded host defect.

- acceptance-harness-correction
  - Transfer Kind: work
  - Description: replace the current shallow Extension Host proof surface with a repository-owned gate that exercises the production controller/registered-command path across the exact full operator sequence and required negative cases.
  - Controlling Artifact: [Anchor Gate Disposition](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-anchor-kodax-host-repair-acceptance-and-machine-gate-disposition.trace.md)
  - Boundary: test fixtures/adapters may exist only at legitimate VS Code-owned seams and must not bypass the host into Core helpers.

- return-machine-evidence
  - Transfer Kind: responsibility
  - Description: return exact machine receipts, exact candidate source delta, residual risks and one Kodax-to-Anchor Handoff marked candidate-for-anchor-reconciliation only when every required machine gate actually passes; otherwise return blocked at the first exact unresolved gate.
  - Controlling Artifact: [Extension Host End-To-End Acceptance Completion](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md)
  - Boundary: no Sigma gate, release or remote mutation from Kodax.

## Required Context

- controlling-task
  - Material: exact current Extension Host End-To-End Acceptance Completion Task
  - Material Reference: [Controlling Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md)
  - Purpose: objective, Done Criteria, scope and boundaries for the remaining machine gate
  - Availability: available

- anchor-disposition
  - Material: Anchor acceptance of the bounded host repair and rejection of the incomplete machine gate
  - Material Reference: [Anchor Gate Disposition](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-anchor-kodax-host-repair-acceptance-and-machine-gate-disposition.trace.md)
  - Purpose: preserve exactly what is accepted versus still blocked
  - Availability: available

- prior-kodax-evidence
  - Material: Kodax VS Code Core-boundary repair and blocked acceptance Evidence
  - Material Reference: [Kodax Repair Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-kodax-vs-code-core-boundary-repair-and-acceptance-evidence.trace.md)
  - Purpose: exact implemented repair, prior test receipts and environment blocker history
  - Availability: available

- extension-vscode-candidate
  - Material: exact current complete Extension VS Code candidate source returned by Kodax
  - Material Reference: [Extension VS Code Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: writable candidate and acceptance harness source
  - Availability: available

- accepted-core
  - Material: exact Anchor-accepted Core source from the preceding Loom tranche
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: Local-mode Core source and shared mechanical authority
  - Availability: available

- canonical-docs
  - Material: exact canonical Docs source carried read-only
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: semantic/schema authority if acceptance interpretation requires confirmation
  - Availability: available

- business-workspace
  - Material: exact current Business continuation including Anchor disposition and controlling Task
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: work authority plus bounded Evidence/return authoring
  - Availability: available

## Reference Context

- previous-controller-task
  - Material: prior VS Code Core-Boundary Recovery And Extension Host Acceptance Task
  - Material Reference: [Prior Host Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-vs-code-core-boundary-recovery-and-extension-host-acceptance.trace.md)
  - Purpose: historical broader Done Criteria now narrowed to the remaining machine-acceptance gap
  - Availability: available

## Retained Responsibilities

- anchor-reconciliation
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: reconcile Kodax's next return against the exact current source frontier and decide whether the Sigma gate may be manufactured.
  - Boundary: Kodax cannot self-promote machine evidence into Sigma/product acceptance.

- human-operator-gate
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)
  - Responsibility: perform the later real operator/UX acceptance only after Anchor accepts the machine gate.
  - Boundary: Sigma remains excluded from debugging and machine-gate completion.

## Exclusions And Dependencies

- no-shared-semantic-mutation
  - Kind: excluded-scope
  - Description: no Core or Docs mutation, no Handoff/participant/cache/material semantic widening and no private recreation of shared mechanics in VS Code.
  - Responsible Party Or Role: Kodax must stop and return any exact shared capability gap to Anchor.

- no-general-refactor
  - Kind: excluded-scope
  - Description: the accepted host repair is preserved; broad controller/monolith cleanup is outside this tranche unless the real gate exposes one exact bounded host-owned defect that requires it.
  - Responsible Party Or Role: Kodax.

- real-extension-host-runner
  - Kind: unresolved-dependency
  - Description: a real VS Code Extension Host runner must execute the repository-owned Local and Published gate. If unavailable, return blocked with the exact runnable gate and environment blocker rather than synthetic acceptance.
  - Responsible Party Or Role: Kodax for execution/evidence; Anchor for later disposition.

- no-remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release or deployment is authorized.
  - Responsible Party Or Role: Anchor / owning release authority.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return exact machine-acceptance Evidence and current Extension VS Code source to Anchor, with candidate-for-anchor-reconciliation only if every required real Extension Host Local/Published and dependency-backed gate passes; otherwise return blocked with the first exact unresolved gate.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: current shallow Extension Host checks are accepted, product source must change, Kodax owns shared semantics, Sigma is delegated, or release/publication is authorized.
- Must Not Be Used To Claim: Node mocks, source assertions, command registration, refresh-only Extension Host execution, package-only tests or direct Core helper invocation satisfy the required real operator-flow gate.
- Authority Limits: exact bounded machine-acceptance completion and only directly exposed host corrections; Anchor retains reconciliation/sequencing and Sigma retains the human gate.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md)
  - Value: HIyLNM3rktvNX_DXoMaWo4Mftpi0WigERKHKyvCezpY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: NDXxB15RbQCCqk7HYE2a1w0gsXjB96hUV57-HhvtawA