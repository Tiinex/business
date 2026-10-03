# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-28 10:42:25
  - Trace: [016-1-1-anchor-to-sigma-vs-code-tree-projection-and-send-route-candidate.trace.md](016-1-1-anchor-to-sigma-vs-code-tree-projection-and-send-route-candidate.trace.md)
  - Origin:
    - [relative](016-1-1-anchor-to-sigma-vs-code-tree-projection-and-send-route-candidate.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-28 13:41:45
  - Authors: Anchor
  - Why: Return the final bounded VS Code polish and release-readiness candidate for Sigma real-host acceptance before automated Marketplace publishing is enabled.
  - Summary: Candidate 018 closes the remaining native VS Code UX polish seams and prepares a Marketplace-ready release surface without reopening Core.
  - Status: ready/local

---

## Handoff Parties

- Purpose: perform the final focused real Windows / VS Code acceptance pass on Candidate 018 and confirm the extension is ready to close the current VS Code stabilization frontier before Marketplace release automation is wired.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../../roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md)

## Transfers

- vscode-final-polish-and-marketplace-readiness-candidate-018
  - Transfer Kind: work-and-responsibility
  - Description: validate the exact carried Candidate 018 VS Code Workspace. This candidate preserves the accepted Candidate 016/017 correctness frontier, closes the remaining native UX polish seams, and prepares the repository/VSIX/Marketplace presentation surface for a subsequent automated release-flow phase.
  - Controlling Artifact: [Candidate 017](016-1-1-anchor-to-sigma-vs-code-tree-projection-and-send-route-candidate.trace.md)
  - Boundary: Core remains frozen. VS Code continues to project Core-owned route/pointer/participant/lineage semantics and explicit operator intent only. Candidate 018 adds no host-owned semantic resolver, alternate manufacture path, route grammar, slugification, participant authority, or Core replacement logic.

## Required Context

- vscode-candidate-workspace
  - Material: exact VS Code Workspace containing Candidate 018 source, built dist, Marketplace-ready README/support/changelog/manifest surface, release audit tooling, packaged VSIX, and focused regression evidence.
  - Material Reference: [VS Code Workspace](vscode::.topics/.workspaces/tiinex-vscode.workspace.md)
  - Purpose: exact candidate under acceptance. The carried Workspace is source authority; the included VSIX is a derived installable artifact from that same candidate, not a replacement semantic authority.
  - Availability: available

- frozen-core-workspace
  - Material: exact frozen Core Workspace inherited from the qualified Candidate 017 parent carrier.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: semantic and Tooling authority. Candidate 018 consumes existing Core projections and does not modify Core.
  - Availability: available

- app-workspace
  - Material: unchanged App Workspace inherited from the qualified Candidate 017 parent carrier.
  - Material Reference: [App Workspace](app::.topics/.workspaces/tiinex-app.workspace.md)
  - Purpose: preserve complete shared-consumer context without claiming an App delta.
  - Availability: available

- docs-workspace
  - Material: unchanged Docs Workspace inherited from the qualified Candidate 017 parent carrier.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: preserve canonical schema/validator context without claiming a Docs delta.
  - Availability: available

## Reference Context

- candidate-017-acceptance-frontier
  - Material: exact preceding Candidate 017 Handoff plus Sigma's real-Windows video disposition showing the major correctness seams remained healthy while exposing only bounded native UX/presentation polish issues.
  - Material Reference: [Candidate 017](016-1-1-anchor-to-sigma-vs-code-tree-projection-and-send-route-candidate.trace.md)
  - Purpose: preserve the accepted correctness frontier while narrowing Candidate 018 to final polish and release readiness.
  - Availability: available

## Retained Responsibilities

- bounded-final-recovery
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)
  - Responsibility: receive Sigma's disposition on this exact Candidate 018. If one concrete blocker remains, reproduce it against this exact carried Workspace and correct only at the demonstrated owner boundary.
  - Boundary: do not reopen Core, Transport, participant authority, Title/Slug, manufacture, or pointer semantics without new owner-level evidence.

## Candidate Delta

- native-action-icons
  - Change: Exclude Handoff Route and Detach Handoff use VS Code 1.95-supported Codicons instead of the unsupported `unlink` icon id.
  - Expected Effect: row actions render visible native icons while retaining the same commands and tooltips.
  - Boundary: command behavior and route state are unchanged.

- modal-cancel-hygiene
  - Change: the Workspace-source replacement warning supplies only the affirmative action and lets VS Code provide the native modal cancel/dismiss affordance.
  - Expected Effect: the dialog shows one Cancel path instead of duplicated Cancel buttons.
  - Boundary: the warning condition and mutation gate are unchanged.

- lineage-presentation-boundary
  - Change: Leaves / Full Lineage controls only artifact membership. Pointer/reference/detail children no longer change merely because lineage mode changes.
  - Expected Effect: Leaves shows lineage leaves; Full Lineage shows those leaves plus their ancestors. Handoff/pointer/reference detail structure remains stable in both modes.
  - Boundary: Candidate 018 reuses the existing artifact-lineage helpers and existing Core-projected state. No VS Code lineage resolver or inferred ancestry is introduced.

- reveal-package-windows-behavior
  - Change: Reveal Package opens the containing directory instead of asking Windows shell to reveal/open the ZIP URI itself.
  - Expected Effect: File Explorer opens at the package directory so the `.handoff-package.zip` is visible as a file rather than entering the ZIP as a shell folder.
  - Boundary: package path, package bytes, transport state and carrier identity are unchanged.

- marketplace-presentation
  - Change: README is rewritten as a Marketplace-facing product/operator introduction while the deeper operator reference remains separate; CHANGELOG and SUPPORT are explicit; package metadata includes repository/homepage/issues, Apache-2.0 SPDX, searchable categories/keywords, free pricing, gallery banner, a 256x256 Tiinex PNG icon, and explicit untrusted/virtual Workspace capability boundaries.
  - Expected Effect: Marketplace installation presents a coherent public extension page rather than an internal engineering README, while users retain links to detailed operator material.
  - Boundary: documentation/manifest presentation only; no semantic authority moves into Marketplace metadata.

- vsix-runtime-projection
  - Change: the repository-owned VSIX packer now obtains the bundled `@tiinex/core` file list from npm's own local `pack --dry-run --json` projection instead of recursively copying the entire installed Core repository/package directory.
  - Expected Effect: the VSIX carries exactly the Core npm runtime projection and excludes Core `.topics`, tests, repository automation and other non-package material.
  - Boundary: this delegates package membership to Core's existing npm package contract; VS Code does not invent a second Core file-selection rule.

- release-readiness-surface
  - Change: `vscode:prepublish`, `release:audit`, `release:check`, Marketplace release notes/runbook and repository packaging checks are explicit and identity-neutral.
  - Expected Effect: a later release-automation phase can make validation/package/publish deterministic without embedding a long-lived publishing credential contract in the extension source.
  - Boundary: Candidate 018 does not publish to Marketplace and does not add a PAT-based publisher workflow. Publisher identity/credentials remain a later operational release concern.

## Machine Qualification

- bridge-regressions
  - Result: 124/124 VS Code bridge cases passed against the Candidate 018 emitted `dist`, including the new lineage-membership/native-UX regression.
  - Boundary: source/bridge regression evidence; native Windows Extension Host behavior remains a separate final gate.

- package-integration
  - Result: 6/6 package integration scenarios passed against frozen `@tiinex/core` 0.45.0, including routed multi-Handoff manufacture and physical Handoff/participant pointer ancestry.
  - Boundary: package integration does not substitute for TreeView interaction.

- release-audit
  - Result: `scripts/release-check.mjs` reports `ready` with zero errors and zero warnings for the current Marketplace surface.
  - Boundary: repository/Marketplace metadata and packaging policy audit only; no remote Marketplace publication was attempted.

- vsix-package
  - Result: `dist/tiinex-vscode-0.1.7.vsix` is 7,332,860 bytes with SHA-256 `550f011ab135ba7f69b81a65af3f554f60b904acae40df4d2c7123040ef1cfa0`. The archive contains 573 entries. The bundled Core runtime is `@tiinex/core` 0.45.0 with 508 npm-projected files and representation SHA-256 `ea30fe62a20f3f290feb7d6f4b4ea2037743abcbbfc5499980c223235e98501e`.
  - Boundary: derived installable release candidate from the exact carried Workspace.

- vsix-content-audit
  - Result: packaged README bytes are identical to the current Workspace README; required README/CHANGELOG/SUPPORT/LICENSE/NOTICE/icon/manifest/runtime files are present; extension source/tests/scripts/maps and Core `.topics`/tests/repository automation are absent from the VSIX.
  - Boundary: physical archive-content evidence only.

- typescript-environment-note
  - Result: Candidate 018 TypeScript source was rebuilt before the final release-only documentation/packaging changes and the emitted code is the code exercised by 124/124 regressions. A later sandbox attempt to perform a fresh `npm ci --include=dev` was blocked by temporary npm-registry DNS availability and removed the local dev-only packages; no TypeScript source changed after the successful Candidate 018 build.
  - Boundary: do not represent the transient registry failure as a candidate correctness failure or as proof of a fresh clean-install build. Sigma's ordinary Windows dependency install/build remains the exact final clean-host confirmation.

## Focused Sigma Acceptance

- native-actions
  - Verify: Exclude Handoff Route and Detach Handoff show visible native icons and retain their existing behavior/tooltips.

- modal-dialog
  - Verify: changing a Workspace source produces one native Cancel path, not duplicated Cancel buttons.

- lineage
  - Verify: with an artifact chain such as `001 -> 001-1 -> 001-1-1`, Leaves shows only the leaf while Full Lineage shows leaf plus ancestors. Expanding the same Handoff/pointer/reference rows should expose the same detail structure in both lineage modes.

- reveal-package
  - Verify: Reveal Package opens File Explorer at the containing directory with the `.handoff-package.zip` visible, rather than entering the ZIP file.

- regression-preservation
  - Verify: Candidate 017 behavior remains healthy: Outgoing/Incoming pointer-oriented logical projection, zero-participant expansion, row-level Send to Transport, package-root Transport, Title/Slug/H1 authoring, native 0..n participant QuickPick, physical pointer targets, Pack to Transport and reload persistence.

- marketplace-surface
  - Verify: install the carried `dist/tiinex-vscode-0.1.7.vsix` or build/package from the exact Workspace; confirm the extension details page presents the Tiinex icon, concise README, changelog/support links and expected metadata without requiring any release credential.

## Exclusions And Dependencies

- core-frozen
  - Kind: excluded-scope
  - Description: no Core change is part of Candidate 018. Core is reopened only with separate owner-level evidence that the exact carried host candidate cannot satisfy an existing contract.
  - Responsible Party Or Role: Anchor / Sigma

- no-parallel-vscode-semantics
  - Kind: excluded-scope
  - Description: do not add host-owned route IDs, endpoint discovery, participant authority, pointer relationship inference, lineage inference, slugification, carrier lineage/allocation or alternate manufacture/Transport paths.
  - Responsible Party Or Role: Anchor / Sigma

- marketplace-publication-deferred
  - Kind: unresolved-dependency
  - Description: actual Marketplace publisher authentication and automated publish workflow are intentionally deferred until Candidate 018 real-host acceptance closes the extension frontier. The follow-up should prefer Microsoft's current workload-identity/Entra direction rather than binding the repository to a legacy long-lived PAT-first contract.
  - Responsible Party Or Role: Anchor

## Completion Expectation

- Signal Kind: disposition
- Signal Meaning: Sigma either accepts the exact carried Candidate 018 as the final VS Code extension stabilization candidate, enabling the Marketplace automated release-flow phase, or returns one concrete reproducible blocker with visual evidence sufficient for bounded owner-level recovery.
- Return To: Anchor
- Return To Reference: [Anchor Role](../../roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md)

## Interpretation Limits

- Does Not Mean: Core was changed, Marketplace publication already occurred, a clean Windows dependency install is already established by this sandbox, or Marketplace metadata grants semantic authority.
- Must Not Be Used To Claim: permission to infer semantic relationships from VS Code inventory, synthesize route/pointer/participant/lineage identity, broaden scope without a concrete blocker, or replace the canonical Handoff Package with loose files.
- Transport Limits: normal completion is one canonical Handoff Package plus the exact routing text projected by Core.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [016-1-1-anchor-to-sigma-vs-code-tree-projection-and-send-route-candidate.trace.md](016-1-1-anchor-to-sigma-vs-code-tree-projection-and-send-route-candidate.trace.md)
  - Value: VmEf-szZY7DsCAsGlfoEIPlYMszj5xg_REv59VMcUKk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: AT0d1V7Gct4ZSyYQlM_yL4v8NDZBtub1h6qlzT6cUzM