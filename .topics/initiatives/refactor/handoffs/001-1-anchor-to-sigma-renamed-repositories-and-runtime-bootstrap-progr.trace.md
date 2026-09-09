# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-09 15:57:30
  - Trace: [001-anchor-to-sigma-turn-2-commitable-full-source-progression.trace.md](001-anchor-to-sigma-turn-2-commitable-full-source-progression.trace.md)
  - Origin:
    - [relative](001-anchor-to-sigma-turn-2-commitable-full-source-progression.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-09 17:00:38
  - Authors: Anchor
  - Summary: Anchor to Sigma — renamed repositories and runtime bootstrap progression
  - Status: ready/local

---

# Anchor to Sigma — renamed repositories and runtime bootstrap progression

## Handoff Parties

- Purpose: deliver one reconciled full-source Refactor progression after the Extension/Interop renames and Runtime/Chrome frontier creation so Sigma can land/push the carried repositories and bootstrap the eligible npm packages.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](business::.topics/roles/001-4-sigma-role.trace.md)

## Transfers

- turn-2-renamed-source-progression
  - Transfer Kind: work
  - Description: land the exact carried repository source without overlaying stale predecessor Workspaces, then perform repository/npm operator bootstrap only for the explicitly eligible package frontiers.
  - Controlling Artifact: [Turn 2 repository decomposition frontier](.topics/initiatives/refactor/repositories/001-turn-2-repository-decomposition-frontier.trace.md)
  - Boundary: transport, landing and package-bootstrap operator work only; this progression is not final Turn-2 acceptance, release approval, or a transfer of Refactor architecture ownership.

## Required Context

- business-workspace
  - Material: current Business source with Turn-2 control lineage, repository/extension/interop/runtime initiatives, GPT processes and qualification evidence.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: controlling cross-repository continuity and bounded organizational/process context.
  - Availability: available

- docs-workspace
  - Material: current Docs source and canonical semantic/schema boundaries.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: semantic authority and contract review context.
  - Availability: available

- core-workspace
  - Material: current Core source including current portable Tooling, lineage, Handoff and package mechanics.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: shared mechanics and Tooling source.
  - Availability: available

- app-workspace
  - Material: current App source and Verse-host/application-data frontier.
  - Material Reference: [App Workspace](app::.topics/.workspaces/tiinex-app.workspace.md)
  - Purpose: shared application host/data-plane source before Verse extraction.
  - Availability: available

- site-workspace
  - Material: current thin Site source composed against `@tiinex/verse-playthings`.
  - Material Reference: [Site Workspace](site::.topics/.workspaces/tiinex-site.workspace.md)
  - Purpose: deployment integration source with explicit Verse Playthings registry dependency.
  - Availability: available

- extension-vscode-workspace
  - Material: current renamed Extension VS Code source plus repo-local Turn-2 and Runtime bridge Tasks; predecessor VS Code artifacts remain only where truthful recovery/history requires them.
  - Material Reference: [Extension VS Code Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: highest-priority editor host lane source; VSIX/product versioning remains separate and no 0.1.8 release claim is transferred.
  - Availability: available

- extension-chrome-workspace
  - Material: initial thin Chrome extension source frontier with repository-local host-contract and qualification Tasks.
  - Material Reference: [Extension Chrome Workspace](extension-chrome::.topics/.workspaces/tiinex-extension-chrome.workspace.md)
  - Purpose: establish a bounded browser host without baking provider/interop-specific logic into the host.
  - Availability: available

- verse-playthings-workspace
  - Material: current renamed Verse Playthings source and Turn-2 integration/qualification lineage.
  - Material Reference: [Verse Playthings Workspace](verse-playthings::.topics/.workspaces/tiinex-verse-playthings.workspace.md)
  - Purpose: current Playthings Verse and multi-Workspace presentation frontier.
  - Availability: available

- provider-native-workspace
  - Material: initial Native provider package/release frontier and repository-local Task/Subtasks.
  - Material Reference: [Provider Native Workspace](provider-native::.topics/.workspaces/tiinex-provider-native.workspace.md)
  - Purpose: make local/native source resolution use the same provider-neutral contracts as external providers.
  - Availability: available

- provider-github-workspace
  - Material: initial GitHub provider package/release frontier and repository-local Task/Subtasks.
  - Material Reference: [Provider GitHub Workspace](provider-github::.topics/.workspaces/tiinex-provider-github.workspace.md)
  - Purpose: isolate GitHub-family browse/git/discovery/publication behavior from shared Core/App.
  - Availability: available

- verse-native-workspace
  - Material: initial Native Verse package/release frontier and Viewer extraction/value-recovery Tasks.
  - Material Reference: [Verse Native Workspace](verse-native::.topics/.workspaces/tiinex-verse-native.workspace.md)
  - Purpose: make the standard Tiinex presentation independently evolvable from App.
  - Availability: available

- verse-atlas-workspace
  - Material: initial Atlas Verse package/release frontier and isolated spatial exploration Tasks.
  - Material Reference: [Verse Atlas Workspace](verse-atlas::.topics/.workspaces/tiinex-verse-atlas.workspace.md)
  - Purpose: keep large-scale spatial exploration independently scalable from Native/App.
  - Availability: available

- interop-native-workspace
  - Material: current renamed Native Interop package/release frontier with generic bootstrap, grounding and external capability Tasks; predecessor Interop artifacts remain truthful recovery/history context where required.
  - Material Reference: [Interop Native Workspace](interop-native::.topics/.workspaces/tiinex-interop-native.workspace.md)
  - Purpose: keep generic bootstrap/interop provider- and environment-agnostic.
  - Availability: available

- interop-openai-workspace
  - Material: initial OpenAI-specific Interop package/release frontier and environment-grounding/capability Tasks.
  - Material Reference: [Interop OpenAI Workspace](interop-openai::.topics/.workspaces/tiinex-interop-openai.workspace.md)
  - Purpose: isolate OpenAI-specific constraints, capabilities and workarounds from generic Interop/Core.
  - Availability: available

- runtime-native-workspace
  - Material: initial portable headless Runtime package/release frontier with execution, capability, provider/interop, recovery and qualification Tasks.
  - Material Reference: [Runtime Native Workspace](runtime-native::.topics/.workspaces/tiinex-runtime-native.workspace.md)
  - Purpose: establish Tiinex's provider-, environment- and host-agnostic orchestration frontier without claiming the runtime implementation is complete.
  - Availability: available

## Reference Context

- none

## Retained Responsibilities

- refactor-anchor-leadership
  - Retained By: Anchor
  - Responsibility: reconcile the landed source, continue Turn-2 architecture, audit child returns, qualify shared boundaries, control destructive Reduction gates and manufacture later canonical Handoffs.
  - Boundary: Sigma landing/publishing this progression does not transfer project, technical or semantic authority.

- open-turn-2-frontiers
  - Retained By: Anchor
  - Responsibility: provider/Verse extraction, Viewer value recovery, final Extension VS Code integration, Chrome/Runtime implementation, browser qualification, Site Reduction, CLI establishment and final Turn-2 stability.
  - Boundary: open work remains explicit rather than fabricated as complete.

## Exclusions And Dependencies

- npm-bootstrap-operator-step
  - Kind: unresolved-dependency
  - Description: `@tiinex/provider-native`, `@tiinex/provider-github`, `@tiinex/verse-native`, `@tiinex/verse-atlas`, `@tiinex/verse-playthings`, `@tiinex/interop-native`, `@tiinex/interop-openai`, and `@tiinex/runtime-native` have local source/workflow prerequisites for `publish:bootstrap`, but actual GitHub landing, npm Trusted Publisher configuration and registry publication are not proven by this carrier.
  - Responsible Party Or Role: Sigma for repository/npm operator transport; Anchor retains qualification interpretation.

- verse-playthings-before-site-install
  - Kind: unresolved-dependency
  - Description: Site declares `@tiinex/verse-playthings@0.1.0`; bootstrap/publish Verse Playthings before expecting a clean registry-backed Site install/deploy.
  - Responsible Party Or Role: Sigma for operator sequence.

- extension-release-boundaries
  - Kind: excluded-scope
  - Description: Extension VS Code remains VSIX-distributed and must not be treated as npm-bootstrap work or as 0.1.8 release-ready; Extension Chrome is an initial source scaffold and is not npm/package-store qualified.
  - Responsible Party Or Role: Anchor

- final-product-qualification
  - Kind: excluded-scope
  - Description: this progression does not claim final browser E2E, Viewer parity, completed provider/Verse/Interop extraction, Site historical Reduction, completed Runtime/Chrome implementation, Marketplace/Chrome Store readiness or final Turn-2 stability.
  - Responsible Party Or Role: Anchor

- cli-frontier
  - Kind: unresolved-dependency
  - Description: CLI remains not source-established in this Refactor frontier and is not fabricated into the carrier.
  - Responsible Party Or Role: Anchor

## Completion Expectation

- Signal Kind: return
- Signal Meaning: Sigma lands/pushes the carried repositories as the current source progression, bootstraps only the eligible npm packages after their real repository/Trusted-Publisher prerequisites are ready, and reports any local divergence or bootstrap failure before Anchor resumes broad implementation/delegation.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Interpretation Limits

- Does Not Mean: final Turn-2 acceptance, npm publication success, human product acceptance, extension release approval, completed Runtime, or broad delegation readiness.
- Must Not Be Used To Claim: that GitHub metadata is source authority; that a new repository scaffold freezes its future public API; that package-readiness equals publication; or that tests not stated in carried evidence passed.
- Authority Limits: transport/landing/operator-bootstrap work only; Refactor Anchor leadership and canonical semantic/role authorities remain separate.
- Transport Limits: this Handoff carrier is canonical for this delivery. Older Handoffs, recovery checkpoints and child-lane carriers are provenance/recovery inputs, not competing current source.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-anchor-to-sigma-turn-2-commitable-full-source-progression.trace.md](001-anchor-to-sigma-turn-2-commitable-full-source-progression.trace.md)
  - Value: mJCiWwdVk_kIuq1fv5LzhxewCGHS--RAV1taYhKXIbc

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: cUI8bCKlercjyMbqZQkaLt_msNWkQfVtPyqREunHdaU