# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: tiinex.decision.v1
  - Created At: 2026-09-21 17:49:18
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-anchor-sigma-real-host-gate-sequencing-disposition.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-anchor-sigma-real-host-gate-sequencing-disposition.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-anchor-sigma-real-host-gate-sequencing-disposition.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 17:49:43
  - Authors: Anchor
  - Why: The remaining acceptance blocker is access to a real VS Code/dependency environment, which Sigma can provide without taking implementation authority or requiring a non-Tiinex intermediate format.
  - Summary: Execute the real VS Code machine gate first on the exact carried candidate; stop on the first blocker or continue directly to Sigma human acceptance only after a complete machine PASS.
  - Status: ready/local

---

## Handoff Parties

- Purpose: execute the final real-host machine qualification and, only if it passes completely, continue directly into Sigma human operator acceptance on the exact carried Tiinex candidate without using Sigma as a debugger.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](business::.topics/roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)

## Transfers

- real-host-machine-gate
  - Transfer Kind: work
  - Description: execute the repository-owned real VS Code Extension Host acceptance using the exact carried Extension VS Code candidate and exact carried accepted Local Core. Restore the candidate's lock-qualified npm dependency tree, run dependency-backed typecheck and existing repository/package regressions, then execute the Local + Published full-flow host gate.
  - Controlling Artifact: [Extension Host End-To-End Acceptance Completion](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md)
  - Boundary: if any required machine stage fails, stop at the first exact blocker and return it to Anchor without debugging, patching, product mutation, or continuing into human acceptance.

- sigma-human-acceptance
  - Transfer Kind: work
  - Description: only after the complete machine phase passes, exercise the resulting candidate through the real VS Code operator workflow as Sigma and determine whether the experience and behavior are acceptable at the human gate.
  - Controlling Artifact: [Anchor Sigma Gate Sequencing Decision](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-anchor-sigma-real-host-gate-sequencing-disposition.trace.md)
  - Boundary: machine PASS is only entry to the human gate, not acceptance itself; Sigma observes and returns, and does not repair implementation.

## Required Context

- machine-gate-evidence
  - Material: Kodax machine-gate Evidence containing the complete repository-owned real-host harness, exact encoded coverage, source delta, and prior environment blocker.
  - Material Reference: [Kodax Machine-Gate Evidence](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-kodax-extension-host-end-to-end-machine-gate-evidence.trace.md)
  - Purpose: exact machine acceptance basis and interpretation limits.
  - Availability: available

- extension-vscode-candidate
  - Material: exact modified Extension VS Code Workspace returned by Kodax.
  - Material Reference: [Extension VS Code Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: candidate source to restore dependencies, build, test, and run in real VS Code.
  - Availability: available

- accepted-local-core
  - Material: exact Anchor-accepted Local Core Workspace carried through the Kodax return unchanged.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: exact Local-mode Core source required by the repository-owned host gate.
  - Availability: available

- controlling-task
  - Material: Extension Host End-To-End Acceptance Completion Task.
  - Material Reference: [Controlling Task](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-extension-host-end-to-end-acceptance-completion.trace.md)
  - Purpose: preserve the exact Done Criteria and fail-closed boundary.
  - Availability: available

## Reference Context

- kodax-return
  - Material: blocked Kodax return preserving the exact candidate and unavailable-environment disposition.
  - Material Reference: [Kodax Return](business::.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-kodax-to-anchor-extension-host-end-to-end-machine-gate-return.trace.md)
  - Purpose: provenance for why the real-host phase remains unexecuted.
  - Availability: available

## Retained Responsibilities

- reconciliation
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: reconcile Sigma's blocker or acceptance result, decide subsequent work, and preserve the durable frontier.
  - Boundary: Sigma does not inherit implementation orchestration or release authority.

## Exclusions And Dependencies

- implementation-debugging
  - Kind: excluded-scope
  - Description: Sigma must not diagnose through source edits, patch the extension/Core, weaken tests, change fixtures to obtain PASS, or continue past the first machine blocker.
  - Responsible Party Or Role: Anchor and the appropriate specialist after return.

- remote-mutation
  - Kind: excluded-scope
  - Description: no commit, push, publication, release, deployment, or other remote mutation is authorized.
  - Responsible Party Or Role: Anchor.

- real-vscode-environment
  - Kind: unresolved-dependency
  - Description: the gate requires a real compatible VS Code runtime/CLI and the ability to restore the exact package-lock-qualified dependency tree, including the declared Published Core dependency.
  - Responsible Party Or Role: Sigma as operator environment only.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return exactly one bounded result to Anchor: either the first exact machine blocker with the stage/observable failure, or a Sigma human acceptance result after a complete Local + Published real-host machine PASS. Do not return a synthetic or partial PASS.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Sigma has implementation authority, a machine PASS equals human acceptance, a machine failure proves product rejection, or remote mutation is authorized.
- Must Not Be Used To Claim: unit/package/source assertions substitute for real VS Code execution; Local mode substitutes for Published mode; Published mode substitutes for Local mode; or a partially completed host sequence qualifies the gate.
- Authority Limits: bounded real-host verification and human operator acceptance only.
- Transport Limits: use the carried Tiinex Workspaces and qualified Handoff route; do not replace them with repository-global reconstruction or manually repackaged source.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-anchor-sigma-real-host-gate-sequencing-disposition.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-anchor-sigma-real-host-gate-sequencing-disposition.trace.md)
  - Value: EIWkIxhzvtotc9YaT9sZvcTwnFNL5wGuiY17XPub1sA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 8fJfdgCx3ZtsNj3wtIf9a28cvyHQ_AFMW0gmnEYVstQ