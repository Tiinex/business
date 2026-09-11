# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 15:13:43
  - Trace: [004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md](004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
  - Origin:
    - [relative](004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 15:34:51
  - Authors: Anchor
  - Why: The failed Loom cold start proved that serially parenting a recovery checkpoint under an open delegation breaks selected-route leaf grounding; parallel recovery must branch as a sibling.
  - Summary: Preserve the corrected Loom delegation and current full frontier without making the open Loom Handoff non-leaf.
  - Status: ready/local

---

# Anchor full recovery after Loom route-leaf correction

## Handoff Parties

- Purpose: Preserve the current sixteen-Workspace Refactor frontier after correcting the Loom delegation route-leaf failure. This recovery is authored as a sibling of the Loom delegation under the same current recovery Parent so the Loom Handoff remains a valid selected lineage leaf.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
- To: Anchor
- To Kind: role
- To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Transfers

- loom-major-002-delegation-now-durable
  - Transfer Kind: responsibility
  - Description: Preserve the corrected Anchor-to-Loom Carrier Major 002 retry Handoff. The prior `002-2` Loom route remains durable evidence of a correct fail-closed grounding result because its selected Handoff had a declared child; the retry is a sibling-branch leaf and cold-grounded successfully before delivery.
  - Controlling Artifact: [Anchor to Loom Carrier Major 002 retry](004-1-1-1-1-1-anchor-to-loom-carrier-major-002-lineage-safety-hardening-retry.trace.md)
  - Boundary: Delegation does not imply Loom acceptance, completion, merge, release or carrier-Major closure.

- full-source-frontier-major-002
  - Transfer Kind: work-and-responsibility
  - Description: Adopt all sixteen complete Workspace snapshots carried by this recovery as the current Anchor integration frontier. Playthings remains additively merged from its previously qualified return. The Kodax VS Code return contributes only the six changed implementation files plus `docs/GIF-CAPTURE.md`; its newly authored return Handoff artifact is quarantined because its standalone Parent recovery locator is malformed.
  - Controlling Artifact: [Turn-2 stable full-source frontier](../001-turn-2-stable-full-source-frontier.trace.md)
  - Boundary: Source-byte reconciliation does not create release, semantic, human-acceptance, or repository-write authority.

- carrier-major-002-lineage-safety-hardening
  - Transfer Kind: work-and-responsibility
  - Description: Carrier Major 002 is the bounded safety checkpoint for proven parallel-lineage defects: cross-Workspace Parent authoring must preserve Workspace-qualified addresses, package validation must not mask an invalid standalone Parent recovery locator, and parallel carrier sibling allocation must not permit exact Carrier Dimension divergence across isolated runtimes.
  - Boundary: Carrier Major numbering is a transport/progress projection only. Artifact filename dimensions and semantic Parent lineages remain separate and must be audited independently.

- artifact-parent-root-reachability
  - Transfer Kind: responsibility
  - Description: Audit new durable artifacts so their declared Parent/Trace/Origin chains remain truthful, independently recoverable, and ultimately rooted in the Tiinex organization lineage. The Playthings qualification return satisfies this through its Playthings development lineage into Business Initiatives and `.topics/001-tiinex.trace.md`. The Kodax return intended the same Business-rooted chain, but its rendered cross-Workspace Parent locator fails the standalone recovery rule and is therefore not accepted as durable lineage.
  - Boundary: Reaching the organization root and revalidating every historical ancestor under today's newest schema are separate questions; historical schema-upgrade debt must not be silently rewritten.

- vscode-qualified-source-delta
  - Transfer Kind: work
  - Description: Preserve the accepted VS Code source delta exactly: `README.md`, `dist/operatorTrees.js`, `dist/operatorTrees.js.map`, `package.json`, `src/operatorTrees.ts`, `test/run.mjs`, and new `docs/GIF-CAPTURE.md`. Do not carry `.topics/refactor/operator/handoffs/010-kodax-to-anchor-vs-code-carrier-major-001-technical-tranche-retu.trace.md` into the merged durable frontier until shared Parent authoring is repaired and the return artifact can be re-authored truthfully.
  - Controlling Artifact: [VS Code return lineage audit](orchestration/vscode/001-1-vs-code-return-lineage-audit-and-qualified-source-merge.trace.md)
  - Boundary: This is a bounded source merge, not VS Code Major acceptance or release readiness.

- playthings-return-idempotence
  - Transfer Kind: responsibility
  - Description: Treat the repeated Playthings return as an idempotent duplicate because the exact Carrier Dimension and exact ZIP SHA-256 match the already-audited return byte-for-byte. Do not create another merge or progression from the duplicate alone.
  - Boundary: Same exact carrier identity with different bytes would instead be a hard integrity signal requiring fail-closed diagnosis.

- anchor-local-first-recovery-discipline
  - Transfer Kind: responsibility
  - Description: Continue using qualified Recovery Carriers as durable continuity checkpoints; treat runtime materializations as cache; audit incoming packages before merge; preserve newer current bytes; and refresh full recovery after meaningful accepted deltas or before context/fork risk.
  - Boundary: Remote sources are fallback/freshness mechanisms, not the first read path when exact qualified local recovery material is present.

## Parallel Route Leaf Invariant

- Delegation Handoffs that must be selected by cold grounding remain Parent-lineage leaves until consumed/returned.
- Recovery/checkpoint artifacts created while parallel delegations are active branch as siblings from the common qualified Parent rather than becoming children of a still-open delegation Handoff.
- This preserves parallel artifact lineage without conflating it with carrier allocation.

## Required Context

- app-workspace
  - Material: Complete current app source snapshot.
  - Material Reference: [app Workspace](app::.topics/.workspaces/tiinex-app.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- business-workspace
  - Material: Complete current Business snapshot including current orchestration and the VS Code return lineage audit Evidence.
  - Material Reference: [business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: Exact current coordination/recovery continuity.
  - Availability: available
- cli-workspace
  - Material: Complete current CLI source snapshot.
  - Material Reference: [cli Workspace](cli::.topics/.workspaces/tiinex-cli.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- core-workspace
  - Material: Complete current Core source snapshot containing the shared Tooling implementation that owns Parent rendering and carrier allocation.
  - Material Reference: [core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: Exact current safety-hardening source.
  - Availability: available
- docs-workspace
  - Material: Complete current Docs snapshot containing canonical Root, Handoff Package, Handoff and lineage semantics.
  - Material Reference: [docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: Canonical semantic/schema continuity.
  - Availability: available
- extension-chrome-workspace
  - Material: Complete current extension-chrome source snapshot.
  - Material Reference: [extension-chrome Workspace](extension-chrome::.topics/.workspaces/tiinex-extension-chrome.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- extension-vscode-workspace
  - Material: Complete merged extension-vscode snapshot containing only the accepted Kodax code/docs delta and excluding the malformed returned Handoff artifact.
  - Material Reference: [extension-vscode Workspace](extension-vscode::.topics/.workspaces/tiinex-extension-vscode.workspace.md)
  - Purpose: Exact current VS Code lane continuity.
  - Availability: available
- interop-native-workspace
  - Material: Complete current interop-native source snapshot.
  - Material Reference: [interop-native Workspace](interop-native::.topics/.workspaces/tiinex-interop-native.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- interop-openai-workspace
  - Material: Complete current interop-openai source snapshot.
  - Material Reference: [interop-openai Workspace](interop-openai::.topics/.workspaces/tiinex-interop-openai.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- provider-github-workspace
  - Material: Complete current provider-github source snapshot.
  - Material Reference: [provider-github Workspace](provider-github::.topics/.workspaces/tiinex-provider-github.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- provider-native-workspace
  - Material: Complete current provider-native source snapshot.
  - Material Reference: [provider-native Workspace](provider-native::.topics/.workspaces/tiinex-provider-native.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- runtime-native-workspace
  - Material: Complete current runtime-native source snapshot.
  - Material Reference: [runtime-native Workspace](runtime-native::.topics/.workspaces/tiinex-runtime-native.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- site-workspace
  - Material: Complete current Site source snapshot.
  - Material Reference: [site Workspace](site::.topics/.workspaces/tiinex-site.workspace.md)
  - Purpose: Exact browser-host integration continuity.
  - Availability: available
- verse-atlas-workspace
  - Material: Complete current verse-atlas source snapshot.
  - Material Reference: [verse-atlas Workspace](verse-atlas::.topics/.workspaces/tiinex-verse-atlas.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- verse-native-workspace
  - Material: Complete current verse-native source snapshot.
  - Material Reference: [verse-native Workspace](verse-native::.topics/.workspaces/tiinex-verse-native.workspace.md)
  - Purpose: Exact current source continuity.
  - Availability: available
- verse-playthings-workspace
  - Material: Complete current verse-playthings snapshot including the already-qualified Major 001 return evidence.
  - Material Reference: [verse-playthings Workspace](verse-playthings::.topics/.workspaces/tiinex-verse-playthings.workspace.md)
  - Purpose: Exact current Playthings technical-qualification continuity.
  - Availability: available

## Reference Context

- vscode-return-carrier
  - Material: `tiinex-vscode-001-1-1-1-2-3-3-3-3-2-2-2-4-1-1-1-4-3-4-2-kodax-to-anchor.handoff-package.zip`, SHA-256 `00b94524344f6353df0602b0273a5fe39990c8f23fb8888587011052bc1cc35b`.
  - Purpose: Exact received carrier used for package validation, Workspace comparison and artifact-level Parent audit.
  - Availability: available
- playthings-duplicate-carrier
  - Material: repeated Playthings return, exact SHA-256 `3a9c97baf50ab2fb76de34fee62e5b09ac60898275d48f1982af93df86b52042`, byte-identical to the previously audited return at the same Carrier Dimension.
  - Purpose: Preserve duplicate/idempotence disposition without creating new work.
  - Availability: available
- vscode-lineage-audit
  - Material: [VS Code return lineage audit](orchestration/vscode/001-1-vs-code-return-lineage-audit-and-qualified-source-merge.trace.md)
  - Purpose: Preserve exact split-merge disposition and the cross-Workspace Parent-authoring defect.
  - Availability: available
- stream-day-orchestration
  - Material: [Stream-Day Parallel Major 001 Orchestration](orchestration/001-stream-day-parallel-major-001-orchestration.trace.md)
  - Purpose: Preserve the plan that led to the audited parallel returns without conflating its artifact filename dimension with carrier progress.
  - Availability: available

## Retained Responsibilities

- carrier-and-parent-lineage-safety
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
  - Responsibility: Route the proven shared Tooling defects to the correct owner, centrally allocate parallel carrier children until allocation is hardened, compare exact Carrier Dimension plus ZIP content on ingress, and reject new artifacts whose Parent recovery locator is not independently truthful.
  - Boundary: Anchor coordinates and fails closed; it does not gain canonical semantic authority from this recovery.
- human-observation-and-acceptance
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-sigma-role.trace.md)
  - Responsibility: Perform bounded Windows/browser observation and subjective acceptance for user-facing lanes after technical prerequisites genuinely pass.
  - Boundary: Technical qualification is not human acceptance.
- implementation-and-semantic-ownership
  - Retained By: bounded repository/role owners
  - Responsibility: Shared Tooling implementation belongs with the shared mechanics owner; canonical semantics belong with Docs/Axiom; extension-local presentation belongs with its implementation lane.
  - Boundary: Cross-repository context is not mutation authority.

## Exclusions And Dependencies

- cross-workspace-parent-authoring-repair
  - Kind: unresolved-dependency
  - Description: Current common authoring can render a Workspace-qualified Parent such as `business::.topics/...` as a bogus local-relative path like `../../../../business::.topics/...`; this must be repaired and regression-tested before accepting newly produced artifacts with that defect.
  - Responsible Party Or Role: shared Core Tooling owner, with Axiom only if semantics require adjudication.
- parallel-carrier-allocation-hardening
  - Kind: unresolved-dependency
  - Description: sibling allocation state is filesystem-local to a parent package copy, so isolated parallel runtimes can independently allocate the same child Carrier Dimension. Until hardened, Anchor must centrally allocate and ingress-audit parallel children.
  - Responsible Party Or Role: shared Core Tooling owner / Anchor coordination.
- organization-github-repository-not-yet-carried
  - Kind: unresolved-dependency
  - Description: the current recovery still carries sixteen established Workspaces but not an exact qualified `Tiinex/.github` repository recovery representation.
  - Responsible Party Or Role: Anchor.
- playthings-full-browser-and-sigma-pass-pending
  - Kind: unresolved-dependency
  - Description: the full Site React/Vite Playthings browser path remains blocked by unavailable locked dependencies; Sigma experience testing follows a genuine technical browser PASS.
  - Responsible Party Or Role: Playthings technical lane / Sigma at later gate.
- vscode-windows-and-branding-pending
  - Kind: unresolved-dependency
  - Description: accepted VS Code source changes remain subject to Windows dogfood; exact main-logo branding remains blocked on qualified `.github/assets` source bytes.
  - Responsible Party Or Role: Sigma / Anchor / VS Code lane.
- viewer-poc-replacement-not-qualified
  - Kind: unresolved-dependency
  - Description: Viewer PoC replacement remains under local-first re-baseline and PoC retirement is not yet justified.
  - Responsible Party Or Role: Anchor / Viewer lane / Sigma.
- remote-mutation-and-release
  - Kind: excluded-scope
  - Description: No remote commit/push, Marketplace publication, Site deployment, package release/version bump or external mutation is authorized by this recovery.
  - Responsible Party Or Role: explicit owning roles and human gates.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: A successor Anchor recovers the sixteen-Workspace Carrier Major 002 frontier including the corrected, cold-grounded Loom safety delegation, preserves the quarantined malformed VS Code return Handoff and accepted source delta distinction, and continues only through audited carrier and artifact Parent progression.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Interpretation Limits

- Does Not Mean: Loom accepted or completed the delegated repair, the malformed Kodax return Handoff is accepted, Carrier Major 002 safety hardening is complete, Playthings full browser passed, VS Code Windows behavior is accepted, Viewer PoC is retired, `.github` recovery coverage is closed, historical schema debt is repaired, or any release/publication occurred.
- Must Not Be Used To Claim: carrier and artifact filename dimensions are equivalent; package validation alone proves standalone Parent recoverability; same-Major parallelism permits exact carrier identity divergence; child package recency overrides current Workspace bytes; or package membership creates semantic/source authority.
- Authority Limits: Anchor coordination/recovery authority only; canonical semantics, implementation, human acceptance and release remain separately owned.
- Transport Limits: This package is continuity transport. It does not create Parent, Origin, assignment, completion or acceptance authority by itself.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md](004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
  - Value: 5hqSjAWfnP-A03XwBKL2-1m4hMo7VSZIxi6o3Krx-2s

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 0j4-TtEoAW-aqCwb78kARR1WFGcUXZmsJ4TfpapN4x8