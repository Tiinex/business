# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 17:49:43
  - Trace: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-sigma-real-host-machine-and-human-acceptance-gate.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-sigma-real-host-machine-and-human-acceptance-gate.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-sigma-real-host-machine-and-human-acceptance-gate.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-21 18:35:10
  - Authors: Anchor
  - Why: Preserve the failed human gate as exact durable evidence before parallel specialist recovery.
  - Summary: Real VS Code Sigma gate exposed live endpoint authority leakage, an authoring-to-Pack endpoint material mismatch, and an independent Workspace integrity/conformance Pack blocker.
  - Status: ready/local

---

## Supported Claim Or Question

- Supported Claim Or Question: What did Sigma's real VS Code operator gate prove about the current candidate, and which failures are independent enough to block product acceptance?
- Evidence Role: Anchor-observed real-host Sigma gate evidence for architecture recovery and specialist routing.
- Supported Conclusion: the current candidate is not Sigma-acceptable. The real operator path exposed at least two independent Pack blockers plus a live endpoint-discovery authority leak: test/schema material can surface as Role choices, a Role Handoff authored through the supported host flow can later fail Pack because exact Role material/reference closure is unavailable, and Workspace-only Pack remains blocked by Workspace integrity/conformance even after the Handoff attachment is removed.

## Provenance

- Known Source: silent screen recording supplied by Sigma from the real VS Code operator gate executed against the exact Anchor-to-Sigma candidate carrier.
- Preservation Basis: Anchor performed read-only review of the recording and current carried source; no candidate source, package bytes, remote repository, release or deployment was mutated while deriving this Evidence.
- Controlling Handoff: `.topics/processes/gpt/grounding/001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-sigma-real-host-machine-and-human-acceptance-gate.trace.md`.
- Observation Method: Anchor reviewed the full recording including endpoint selection, authoring, Attach/Detach, Pack progress and both final failure dialogs; no product mutation or debugging was performed during review.
- Source Corroboration: current Extension VS Code source shows normal local Workspace indexing is restricted to `<workspace-root>/.topics`, while `endpointCatalog()` also invokes shared endpoint projection against `this.extensionPath`; repository-owned Extension Host fixtures themselves contain nested `test/extension-host/fixtures/source-workspace/.topics/roles/*` Role artifacts. Host Role choices are then collapsed by label through `currentRoleChoices`, making same-label source precedence material to live presentation.
- Provenance Limits: the recording has no audio and does not itself prove the root cause of Workspace self-integrity mismatch or the exact Core/host ownership of every failing seam. Those causes remain specialist audit work.

## Evidence Material

- Material: real-host Sigma recording observations plus exact current carried Core/Extension VS Code source seams relevant to endpoint discovery, authoring and Pack failures.
- Material Kind: human operator gate observation corroborated by bounded source inspection.

### Live endpoint discovery contamination

- Sigma opened the Handoff endpoint selector during real authoring and observed Role choices sourced from the Extension VS Code acceptance fixture alongside canonical Business Roles.
- Visible fixture-derived labels included Anchor, Kodax, Loom, Pilot and Sigma from `extension-vscode:test/extension-host/fixtures/source-workspace/.topics/...`; a bounded Role/schema example also appeared as a selectable Role-like endpoint.
- Current source confirms local `indexLocalWorkspace()` itself starts at only the root `.topics`, but `endpointCatalog()` additionally calls `loadHandoffEndpointChoices(this.extensionPath)`. That second path is therefore a concrete audit seam for nested repository material entering endpoint projection.
- `currentRoleArtifacts()` groups Role artifacts by human label and chooses the latest candidate in each label group. A host-side label collapse must not silently choose a fixture/schema example over a canonical exact Role candidate.

### Authoring-to-Pack Role material contract failure

- Sigma authored a Handoff through the supported VS Code form using Role endpoints and attached it to Outgoing.
- The host displayed Core authoring-boundary text indicating fields such as `From Reference` and `To Reference` are visible to validation but not writable through Core creation in this flow.
- Pack then failed closed with `portable.handoff-material.endpoint-role.reference-missing` for the Role endpoint material closure.
- Removing the Handoff attachment removed that endpoint-role failure, proving this blocker is separable from the later Workspace-only Pack blocker.
- Canonical Handoff semantics currently define `From Reference` / `To Reference` as optional resolution aids; exact repair must therefore reconcile authoring, endpoint qualification and transport closure without silently turning optional references into new semantic requirements or allowing host inference to invent authority.

### Independent Workspace-only Pack blocker

- After Sigma detached the authored Handoff and retried Pack, Pack still failed.
- The remaining failure reported `workspace-target-self-integrity-mismatch` and `workspace-target-artifact-conformance-unqualified` for the explicit Workspace target.
- Because this persisted with no attached Handoff, it is independent from endpoint Role closure.
- Root cause is unresolved: specialist audit must compare exact Workspace artifact bytes/integrity across source, Incoming/Replace landing, Local-mode transition and Pack preflight before assigning ownership.

### Secondary host-state signals

- During Topic authoring the UI reported `Attach to Outgoing — create an Outgoing context first` despite an Outgoing context having already been created; later Handoff authoring recognized Outgoing. This is evidence of a possible host/session hydration gap, not yet a proven semantic defect.
- Participant behavior improved relative to the previous gate: the host explicitly reported no additional Core-qualified participants for the tested Handoff rather than silently omitting participant handling. The recording did not exercise a positive multi-participant selection, so positive participant acceptance remains unproven.

## Required Recovery Properties

- Live endpoint discovery must project only qualified endpoint candidates from explicit qualified Workspace/material authority; nested test fixtures, schema examples, repository proximity and label recency must not become production endpoint authority.
- Human labels may aid presentation but must not collapse multiple exact endpoint candidates into one authoritative choice without qualified selection authority. Ambiguity must remain visible/fail closed.
- Supported authoring and Pack must share one coherent Core contract. A Handoff produced by supported authoring must not become un-packable merely because an optional reference was not writable, unless the authoring step itself could already establish the exact contradiction/blocker and stop earlier.
- Role-/identity-unresolved Handoffs must remain representable at the exact strength canonical Docs allow; explicit exact references, when present, must be honored and contradictions fail closed.
- Workspace integrity/conformance must be proven stable through Incoming/Replace/Local/restart/Pack; the owning layer must be identified by exact byte/integrity comparison rather than assumption.
- The next machine acceptance must reproduce the real Sigma path and additionally assert that repository test fixtures/schema examples never appear as live endpoint choices in a normal production Workspace context.


## Preservation And Fidelity

- Preservation State: the failed Sigma candidate and supplied recording remain unchanged; this Evidence records observations and source-corroborated seams only.
- Fidelity Notes: error codes, visible endpoint-source labels and operator ordering are preserved at the strength observed in the recording; inferred root causes are explicitly separated from observed failures.
- Known Losses: no audio transcript and no direct machine log/receipt from the user's VS Code process were supplied with the recording. Root cause of Workspace self-integrity mismatch remains unresolved.

## Interpretation Limits

- Not Yet Used As: implementation acceptance, Sigma acceptance, release approval, remote mutation authority, or proof of the unresolved root causes.
- Does Not Prove: that Core alone caused endpoint contamination, that VS Code alone mutated Workspace bytes, that optional endpoint References must be removed, or that every participant path is broken.
- Must Not Be Treated As: a substitute for Loom/Core or Kodax/VS Code reproduction, a semantic schema amendment, or authority to patch around the failures in the host.
- Must Not Be Used To Claim: the candidate is release-ready, Sigma-accepted, or that prior synthetic/fixture host gates remain sufficient.
- Disposition: real-host Sigma gate BLOCKED; route exact root-cause work to Loom/Core and Kodax/VS Code in parallel before another Sigma attempt.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-sigma-real-host-machine-and-human-acceptance-gate.trace.md](001-1-4-1-3-5-1-2-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-sigma-real-host-machine-and-human-acceptance-gate.trace.md)
  - Value: 8fJfdgCx3ZtsNj3wtIf9a28cvyHQ_AFMW0gmnEYVstQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: L57FenwU_is-dnIjwvJKgUQhZqm7m-Xz_P7Lb0Wqemo