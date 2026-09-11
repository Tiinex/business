# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-11 16:59:13
  - Trace: [001-1-repository-boundary-placement-correction.trace.md](../001-1-repository-boundary-placement-correction.trace.md)
  - Origin:
    - [relative](../001-1-repository-boundary-placement-correction.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 17:02:49
  - Authors: Anchor
  - Why: Preserve corrected repository ownership and the current parallel lane state in one recoverable carrier.
  - Summary: Full recovery after repository-boundary placement correction.
  - Status: ready/local

---

# Anchor Full Recovery — Carrier Major 002 Repository-Boundary Correction

## Handoff Parties

- Purpose: preserve the current audited sixteen-Workspace frontier after correcting prospective specialist artifact placement from Business-default continuity into repository-owned lineages.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Transfers

- full-recovery-continuity
  - Transfer Kind: work-and-responsibility
  - Description: recover the complete current sixteen-Workspace source frontier and continue orchestration from this exact carrier.
  - Boundary: this carrier preserves continuity/source state and does not create authority over sibling repositories.
- repository-boundary-correction
  - Transfer Kind: work
  - Description: preserve the new repository-local orchestration frontier artifacts in Core, App, Site, Verse Playthings, VS Code and Chrome while Business remains coordination, Role, priority and human-gate context.
  - Controlling Artifact: [Repository-boundary placement correction](../001-1-repository-boundary-placement-correction.trace.md)
  - Boundary: historical Business-local specialist artifacts remain preserved; no mass rewrite or silent relocation is authorized.
- return-ingress-audit
  - Transfer Kind: work-and-responsibility
  - Description: audit every specialist return for exact Carrier Dimension/content identity, repository ownership, artifact filename-lineage hygiene, semantic Parent recovery, integrity and reachability to the Tiinex organization root before merge.
  - Boundary: quarantine malformed or ambiguous returns rather than normalizing them silently.

## Required Context

- app-workspace
  - Material: Complete current App Workspace including the repository-local orchestration frontier.
  - Material Reference: [App Workspace](app::.topics/.workspaces/tiinex-app.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- business-workspace
  - Material: Complete current Business Workspace including repository-boundary correction, Roles and recovery lineage.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: Exact orchestration and recovery continuity.
  - Availability: available
- cli-workspace
  - Material: Complete current CLI Workspace.
  - Material Reference: [CLI Workspace](cli::.topics/.workspaces/tiinex-cli.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- core-workspace
  - Material: Complete current Core Workspace including accepted Loom lineage-safety repair and repository-local orchestration frontier.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: Exact current Tooling/source continuity.
  - Availability: available
- docs-workspace
  - Material: Complete current Docs Workspace.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: Canonical semantic continuity.
  - Availability: available
- extension-chrome-workspace
  - Material: Complete current extension-chrome Workspace including accepted Kodax delta and repository-local orchestration/human-test frontier.
  - Material Reference: [Chrome Workspace](extension-chrome::.topics/.workspaces/tiinex-extension-chrome.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- extension-vscode-workspace
  - Material: Complete current extension-vscode Workspace including repository-local orchestration frontier; current Kodax implementation lane remains in progress.
  - Material Reference: [VS Code Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- interop-native-workspace
  - Material: Complete current interop-native Workspace.
  - Material Reference: [Interop Native Workspace](interop-native::.topics/.workspaces/tiinex-interop-native.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- interop-openai-workspace
  - Material: Complete current interop-openai Workspace.
  - Material Reference: [Interop OpenAI Workspace](interop-openai::.topics/.workspaces/tiinex-interop-openai.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- provider-github-workspace
  - Material: Complete current provider-github Workspace.
  - Material Reference: [Provider GitHub Workspace](provider-github::.topics/.workspaces/tiinex-provider-github.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- provider-native-workspace
  - Material: Complete current provider-native Workspace.
  - Material Reference: [Provider Native Workspace](provider-native::.topics/.workspaces/tiinex-provider-native.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- runtime-native-workspace
  - Material: Complete current runtime-native Workspace.
  - Material Reference: [Runtime Native Workspace](runtime-native::.topics/.workspaces/tiinex-runtime-native.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- site-workspace
  - Material: Complete current Site Workspace including repository-local Viewer orchestration and corrected Site-owned Kodax Handoff.
  - Material Reference: [Site Workspace](site::.topics/.workspaces/tiinex-site.workspace.md)
  - Purpose: Exact current Viewer/web-host continuity.
  - Availability: available
- verse-atlas-workspace
  - Material: Complete current verse-atlas Workspace.
  - Material Reference: [Verse Atlas Workspace](verse-atlas::.topics/.workspaces/tiinex-verse-atlas.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- verse-native-workspace
  - Material: Complete current verse-native Workspace.
  - Material Reference: [Verse Native Workspace](verse-native::.topics/.workspaces/tiinex-verse-native.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- verse-playthings-workspace
  - Material: Complete current verse-playthings Workspace including accepted Prism return and repository-local orchestration frontier.
  - Material Reference: [Verse Playthings Workspace](verse-playthings::.topics/.workspaces/tiinex-verse-playthings.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available

## Reference Context

- repository-boundary-rule
  - Material: Business owns cross-repository orchestration, Roles, priorities and human gates; specialist implementation continuity belongs in the actual owning repository.
  - Purpose: Prevent future default placement of specialist Tasks/Handoffs into Business.
  - Availability: available
- corrected-viewer-lane
  - Material: Site-owned Kodax carrier manufactured as a clean descendant of the current Anchor recovery carrier and cold-grounded to act readiness.
  - Purpose: Replace the blocked Business-local Viewer return path prospectively without rewriting historical carriers.
  - Availability: available
- chrome-human-test-lane
  - Material: Extension-Chrome-owned Sigma human-test carrier manufactured as a sibling descendant and cold-grounded to act readiness.
  - Purpose: Collect human evidence from the owning repository lineage.
  - Availability: available

## Retained Responsibilities

- orchestration-and-merge-audit
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
  - Responsibility: coordinate carrier sibling allocation, repository-boundary ownership, return audits and full recovery refreshes.
  - Boundary: Anchor does not gain canonical semantic or human acceptance authority.
- human-acceptance
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-sigma-role.trace.md)
  - Responsibility: human/browser/Windows acceptance where applicable.
  - Boundary: technical qualification is not human acceptance.

## Exclusions And Dependencies

- organization-github-recovery-gap
  - Kind: unresolved-dependency
  - Description: Current recovery still preserves the sixteen established Workspaces but does not yet carry an exact qualified `Tiinex/.github` repository recovery representation.
  - Responsible Party Or Role: Anchor.
- playthings-browser-host-blocker
  - Kind: unresolved-dependency
  - Description: Playthings remains blocked before full Site React/Vite browser startup by unavailable locked dependencies in the current execution host; no Sigma test is requested yet.
  - Responsible Party Or Role: Prism/Anchor when a dependency-capable host is available.
- vscode-active-lane
  - Kind: unresolved-dependency
  - Description: VS Code Kodax remains actively working; do not infer completion or relocate its in-flight historical carrier. Apply repository-local continuation on the next descendant after its return audit.
  - Responsible Party Or Role: Extension VS Code Kodax / Anchor.
- historical-lineage-cleanup
  - Kind: excluded-scope
  - Description: Do not mass-rewrite historical artifact filename dimensions or Parent edges; stop new debt first and schedule later hygiene explicitly if justified.
  - Responsible Party Or Role: future explicit owner.
- release-and-remote-mutation
  - Kind: excluded-scope
  - Description: No release, deployment, publication or remote repository mutation is authorized by this recovery.
  - Responsible Party Or Role: explicit later gates.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: A successor Anchor recovers this exact sixteen-Workspace Carrier Major 002 frontier, understands the repository-boundary placement rule, uses repo-local specialist continuation, preserves Business as orchestration/recovery authority, and continues only through audited carrier and semantic Parent progression.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Interpretation Limits

- Does Not Mean: Carrier Major 002 is complete, Viewer PoC is retired, VS Code Kodax has returned, Playthings browser qualification passed, historical malformed Parents are repaired, or any release is approved.
- Must Not Be Used To Claim: Carrier Major maps to artifact filename major; Business context implies Business artifact ownership; package namespace defines semantic authority; or historical placement must be rewritten to match current policy.
- Authority Limits: Anchor recovery/orchestration only.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-repository-boundary-placement-correction.trace.md](../001-1-repository-boundary-placement-correction.trace.md)
  - Value: N6aESXBT7gissKfKMn5ju7hVnpb-y3o1kA0SpXsCcLg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: DlJjYcC_uzyR_PBIJ0U1FAUbIfl0kgnElcCQUnScf4Y