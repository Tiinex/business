# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 15:08:46
  - Trace: [004-1-1-anchor-full-recovery-carrier-major-002-lineage-safety-checkpoint.trace.md](004-1-1-anchor-full-recovery-carrier-major-002-lineage-safety-checkpoint.trace.md)
  - Origin:
    - [relative](004-1-1-anchor-full-recovery-carrier-major-002-lineage-safety-checkpoint.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-11 15:13:43
  - Authors: Anchor
  - Why: Audited parallel returns exposed two shared safety blind spots that must fail closed before further unguarded parallel manufacture.
  - Summary: Delegate the proven cross-Workspace Parent-authoring and parallel carrier-identity safety defects to shared Core Tooling without expanding semantics or rewriting history.
  - Status: ready/local

---

# Anchor to Loom — Carrier Major 002 lineage-safety hardening

## Handoff Parties

- Purpose: Repair the two shared Tooling blind spots proven by audited parallel returns before Anchor permits further unguarded parallel carrier manufacture or cross-Workspace Parent authoring.
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
- To: Loom
- To Kind: role
- To Reference: [Loom Role](business::.topics/roles/001-3-loom-role.trace.md)

## Transfers

- cross-workspace-parent-authoring-repair
  - Transfer Kind: work-and-responsibility
  - Description: Reproduce and repair common-path `author` behavior where a qualified Parent address such as `business::.topics/...` plus exact `--parent-source` is rendered as a bogus local-relative target like `../../../../business::.topics/...`. Preserve the Workspace-qualified address as the truthful recovery locator and add regression coverage at the common-author/render/qualification boundary.
  - Controlling Artifact: [VS Code return lineage audit](../orchestration/vscode/001-1-vs-code-return-lineage-audit-and-qualified-source-merge.trace.md)
  - Boundary: Do not redesign Root/Parent semantics unless current canonical Docs prove a semantic gap. This tranche is shared Tooling mechanics first.

- package-validation-parent-recovery-guard
  - Transfer Kind: work-and-responsibility
  - Description: Add the smallest shared qualification guard needed so Required Context/package closure cannot make a syntactically or semantically malformed standalone Parent recovery locator appear fully qualified. The reproduced `../../../../business::.topics/...` form must fail closed even when exact Parent bytes are carried elsewhere in the package.
  - Controlling Artifact: [VS Code return lineage audit](../orchestration/vscode/001-1-vs-code-return-lineage-audit-and-qualified-source-merge.trace.md)
  - Boundary: Package closure may preserve/augment an already truthful Parent edge; it must not manufacture Parent validity.

- parallel-carrier-allocation-safety
  - Transfer Kind: work-and-responsibility
  - Description: Audit current sibling reservation, prove the isolated-runtime collision mode, and harden Tooling or its explicit manufacture contract so parallel work cannot silently create the same exact Carrier Dimension with different package content. Preserve valid same-Major parallelism and valid byte-identical duplicate transport.
  - Controlling Artifact: [Carrier Major 002 recovery checkpoint](004-1-1-anchor-full-recovery-carrier-major-002-lineage-safety-checkpoint.trace.md)
  - Boundary: Carrier lineage is independent from artifact filename lineage. Do not solve collisions by deriving carrier identity from artifact filenames or by silently inventing a suffix after divergence has occurred.

- regression-evidence-and-return
  - Transfer Kind: work
  - Description: Return bounded implementation Evidence plus one Handoff to Anchor. Show pre-fix reproduction and post-fix regression for cross-Workspace authoring and carrier allocation/collision behavior. Keep existing valid package roundtrip/cold-ground behavior intact.
  - Boundary: No release/version bump, no remote push, no Docs mutation unless separately proven necessary.

## Required Context

- core-workspace
  - Material: Complete current Core Workspace containing portable authoring, creation renderer/qualification, package manufacture, carrier lineage and sibling allocation mechanics.
  - Material Reference: [Core Workspace](core::.topics/.workspaces/tiinex-core.workspace.md)
  - Purpose: Writable implementation source for this bounded shared Tooling repair.
  - Availability: available
- docs-workspace
  - Material: Complete current canonical Docs Workspace containing Root Parent recovery rules and Handoff Package carrier semantics.
  - Material Reference: [Docs Workspace](docs::.topics/.workspaces/tiinex-docs.workspace.md)
  - Purpose: Read-only canonical semantic boundary unless an actual gap is proven.
  - Availability: available
- business-workspace
  - Material: Complete current Business Workspace containing Carrier Major 002 recovery, the exact VS Code lineage audit Evidence, role authority and orchestration context.
  - Material Reference: [Business Workspace](business::.topics/.workspaces/tiinex-business.workspace.md)
  - Purpose: Controlling task/evidence/return context.
  - Availability: available

## Reference Context

- reproduced-parent-defect
  - Material: Common authoring was invoked for an `extension-vscode` Handoff with Parent reference `business::.topics/initiatives/refactor/orchestration/handoffs/002-anchor-to-kodax-vs-code-carrier-major-001-operator-trust-and-erg.trace.md` and exact Parent source bytes. The emitted artifact instead declared Trace/Origin target `../../../../business::.topics/initiatives/refactor/orchestration/handoffs/002-anchor-to-kodax-vs-code-carrier-major-001-operator-trust-and-erg.trace.md`.
  - Purpose: Exact defect shape to reproduce and prevent.
  - Availability: available
- root-recovery-rule
  - Material: Current Root semantics require every Parent to expose a truthful recovery locator; directly recoverable relative representations must be truthful; when unavailable a qualified version-stable route is required; package closure cannot make an artifact valid when its own envelope exposes no truthful recovery locator.
  - Purpose: Existing canonical boundary the repair must preserve.
  - Availability: available
- carrier-allocation-blind-spot
  - Material: Current `reserveHandoffSiblingIndex` persists reservations beside one local parent-package copy. Separate isolated runtimes holding independent copies of the same parent can therefore each reserve sibling index 1 and manufacture the same exact child Carrier Dimension with different bytes.
  - Purpose: Proven process/tooling blind spot to reproduce and harden.
  - Availability: available

## Retained Responsibilities

- major-scope-and-ingress-audit
  - Retained By: Anchor
  - Retained By Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)
  - Responsibility: Keep Carrier Major 002 bounded to proven lineage-safety defects, centrally allocate children while repair is pending, and audit returned exact Carrier Dimension plus ZIP content before merge.
  - Boundary: Turns may drift; Major scope must not silently grow.
- canonical-semantic-adjudication
  - Retained By: Axiom / canonical Docs owner when needed
  - Responsibility: Adjudicate only if implementation reveals a real semantic ambiguity rather than a mechanical bug.
  - Boundary: Loom must not mutate canonical meaning by implementation convenience.
- human-acceptance
  - Retained By: Sigma
  - Retained By Reference: [Sigma Role](business::.topics/roles/001-4-sigma-role.trace.md)
  - Responsibility: Human gates remain separate; no subjective product acceptance is transferred here.
  - Boundary: Technical Tooling qualification is not human acceptance.

## Exclusions And Dependencies

- historical-mass-rewrite
  - Kind: excluded-scope
  - Description: Existing historical artifacts containing older cross-Workspace locator forms are not to be mass-rewritten in this tranche. Stop new bad output first; later lineage hygiene/reduction is separately planned if justified.
  - Responsible Party Or Role: Anchor / future explicit lineage-hygiene Major.
- artifact-major-reinterpretation
  - Kind: excluded-scope
  - Description: Do not map Carrier Major 002 to artifact filename `002`, or infer artifact Parent from carrier progression.
  - Responsible Party Or Role: Loom / Anchor.
- release-and-remote-mutation
  - Kind: excluded-scope
  - Description: No package release, version bump, remote push, publication or deployment is authorized by this Handoff.
  - Responsible Party Or Role: later explicit owner/human gates.

## Completion Expectation

- Signal Kind: return
- Signal Meaning: Return shared Tooling source plus qualified regression Evidence showing cross-Workspace Parent authoring emits truthful addresses, malformed recovery locators fail closed despite package closure, and parallel carrier identity divergence is prevented or explicitly fail-closed by the supported manufacture contract.
- Return To: Anchor
- Return To Reference: [Anchor Role](business::.topics/roles/001-1-anchor-role.trace.md)

## Interpretation Limits

- Does Not Mean: every historical Parent edge is repaired, all carrier concurrency is globally coordinated across arbitrary offline systems, Carrier Major 002 is complete, or any release is approved.
- Must Not Be Used To Claim: package membership creates Parent authority; carrier identity may be derived from artifact filenames; same exact Carrier Dimension may legitimately contain different bytes; or Tooling may silently normalize a collision after divergent carriers exist.
- Authority Limits: bounded Core Tooling implementation and regression evidence only; canonical semantics, human acceptance and release remain separately owned.
- Transport Limits: This Handoff transfers bounded work/responsibility only through `Transfers`; Required/Reference Context does not transfer unrelated authority.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [004-1-1-anchor-full-recovery-carrier-major-002-lineage-safety-checkpoint.trace.md](004-1-1-anchor-full-recovery-carrier-major-002-lineage-safety-checkpoint.trace.md)
  - Value: TbaVmmULxEtahrd_BQuu3kvxRwmfNrOmj8Q_Q1fPbfA

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: SAE8cnCjtnT_PCobETBrOBtvCMsoGvnoH7o4C1_J6ms