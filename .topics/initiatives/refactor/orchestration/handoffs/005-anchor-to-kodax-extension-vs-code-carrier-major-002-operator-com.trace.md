# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 15:34:51
  - Trace: [004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md](../../handoffs/004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md)
  - Origin:
    - [relative](../../handoffs/004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 15:44:02
  - Authors: Anchor
  - Why: Preserve the accepted Kodax source delta, correct the carrier-major boundary prospectively, and keep shared Handoff/carrier mechanics out of extension-local patches.
  - Summary: Continue bounded VS Code operator ergonomics under Carrier Major 002 while shared Tooling defects remain owned by Core Loom.
  - Status: ready/local

---

# Anchor to Kodax — Extension VS Code Carrier Major 002 Operator Completion Tranche

## Handoff Parties

- Purpose: continue the VS Code operator lane from the audited Kodax return under the correct Carrier Major 002 transport boundary, preserving the accepted code/docs delta while isolating shared Tooling defects already routed to Core Loom.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
- To: Kodax
- To Kind: role
- To Reference: [Kodax Role](business::.topics/roles/001-6-kodax-role.trace.md)

## Transfers

- current-state-reconciliation
  - Transfer Kind: work-and-responsibility
  - Description: re-audit the merged current `extension-vscode` source against Sigma's operator feedback and the accepted prior return. Mark each item PASS, still broken, untested, shared-blocked, or deferred before changing more code.
  - Controlling Artifact: [VS Code return lineage audit](../vscode/001-1-vs-code-return-lineage-audit-and-qualified-source-merge.trace.md)
  - Boundary: do not treat the quarantined malformed returned Handoff artifact as accepted source.
- extension-local-operator-repair
  - Transfer Kind: work
  - Description: continue only extension-local items that remain in scope: safe Pack UX/overwrite protection where host-local, auto-staging and commit ergonomics, identical Incoming/Local green-check behavior, consolidated display-options menu, Attach Handoff verification/repair where not blocked by shared authoring, and Marketplace-quality README/GIF capture support.
  - Boundary: cross-Workspace Parent authoring and carrier allocation mechanics are owned by Core Loom in Carrier Major 002; do not privately patch around them in VS Code.
- windows-test-card
  - Transfer Kind: work
  - Description: return a short ordered Sigma Windows dogfood card for the exact workflows that are technically ready, with expected visible outcomes and stop conditions.
  - Boundary: Kodax does not self-declare Sigma acceptance.

## Required Context

- extension-vscode-workspace
  - Material: Complete current merged extension-vscode Workspace containing the accepted prior Kodax code/docs delta.
  - Material Reference: [VS Code Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: Writable bounded implementation source.
  - Availability: available
- core-workspace
  - Material: Complete current Core Workspace.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: Read-only shared Tooling boundary while Loom repair is in flight.
  - Availability: available
- business-workspace
  - Material: Current VS Code audit, orchestration and role context.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: Exact accepted/quarantined split and Major scope.
  - Availability: available
- docs-workspace
  - Material: Current canonical semantic contracts.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: Read-only boundary for Handoff/Workspace/lineage behavior.
  - Availability: available

## Reference Context

- sigma-vscode-feedback
  - Material: The current ten-point Sigma operator feedback preserved in the prior VS Code Major task and accepted return lineage.
  - Purpose: Reconcile real operator expectations without treating feedback as automatic authority to expand shared semantics.
  - Availability: available
- prior-kodax-return
  - Material: Audited prior Kodax return carrier; accepted code/docs delta is merged while its malformed cross-Workspace Parent Handoff artifact remains quarantined.
  - Purpose: Preserve exact accepted-versus-quarantined state.
  - Availability: available

## Retained Responsibilities

- shared-tooling-defects
  - Retained By: Core Loom lane
  - Responsibility: repair cross-Workspace Parent rendering/qualification and parallel carrier allocation safety.
  - Boundary: VS Code must surface blockers rather than implement private competing semantics.
- carrier-and-scope-orchestration
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
  - Responsibility: audit returns, preserve exact carrier identities and decide Major progression.
  - Boundary: no silent scope growth.
- windows-human-acceptance
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-sigma-role.trace.md)
  - Responsibility: real Windows operator observation and subjective acceptance.
  - Boundary: technical tests are not human acceptance.

## Exclusions And Dependencies

- malformed-return-handoff
  - Kind: unresolved-dependency
  - Description: The prior Kodax return Handoff remains quarantined because its standalone cross-Workspace Parent locator is malformed. Do not copy or normalize it into source history.
  - Responsible Party Or Role: Core Loom repair / Anchor reconciliation.
- organization-brand-assets
  - Kind: unresolved-dependency
  - Description: Exact Tiinex organization `.github/assets` bytes are still not carried in the current full recovery. Branding work requiring them remains blocked rather than guessed.
  - Responsible Party Or Role: Anchor recovery coverage.
- release-and-remote-mutation
  - Kind: excluded-scope
  - Description: No Marketplace release, version bump, remote push or publication is authorized.
  - Responsible Party Or Role: later explicit gate.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: Return one normal Handoff to Anchor with a current feedback-status matrix, bounded extension-local fixes and tests, exact shared blockers, and a concise Windows test card for Sigma.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Interpretation Limits

- Does Not Mean: Core Tooling bugs are fixed, Windows behavior is accepted, branding is complete, release is ready, or Carrier Major 002 maps to artifact filename 002.
- Must Not Be Used To Claim: extension-local code may redefine shared Handoff/carrier semantics or that a successful test substitutes for Sigma observation.
- Authority Limits: bounded `extension-vscode` implementation/qualification only.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md](../../handoffs/004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md)
  - Value: 0j4-TtEoAW-aqCwb78kARR1WFGcUXZmsJ4TfpapN4x8

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: mNwcPDLbT3kEGZ206OvSjYZUPpx0mJ2bZ_Mlavq65MA