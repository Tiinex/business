# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-21 13:51:37
  - Trace: [001-1-4-1-3-architecture-recovery-audit-before-further-host-mutation.trace.md](001-1-4-1-3-architecture-recovery-audit-before-further-host-mutation.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-architecture-recovery-audit-before-further-host-mutation.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-21 14:30:20
  - Authors: Anchor
  - Why: Independent audits converged on distinct semantic, Core, and host defects and now require one durable Anchor disposition before implementation resumes.
  - Summary: Reconcile Axiom, Loom, and Kodax audits into one Core-first implementation and acceptance sequence.
  - Status: ready/local

---

## Decision

- State: accepted
- Subject: architecture-recovery reconciliation after independent Axiom, Loom, and Kodax audits
- Decision: preserve the current canonical Handoff endpoint/reference semantics, authorize only the source-proven Core and VS Code corrections that follow from the independent returns, and sequence implementation Core-first so shared participant/material/packing authority is mechanically sound before host thinning and real Extension Host acceptance resume.

## Reconciled Findings

### Canonical Handoff semantics remain unchanged

- Current `tiinex.handoff.v1` continues to require readable `From`, `From Kind`, `To`, and `To Kind` declarations. Uncertainty uses explicit `Kind: unknown`; endpoint omission is not adopted in this tranche.
- Endpoint, capacity, material, return, and result References remain field-specific resolution aids. They do not replace readable declarations, holder/participant authority, transfer truth, or acceptance.
- Durable semantic References and internal workspace/path/material bindings remain separate fact classes. Internal bindings may resolve exact bytes/provenance but must not be serialized or interpreted as semantic identity by convenience.
- Resolver outcomes such as resolved, unresolved, ambiguous, or contradictory may be exposed as derived mechanical state, but this tranche does not add them as canonical Handoff fields.
- Transparent recipient carriage is compatible with current semantics only as transport/resolver evidence. Carriage, cache presence, package placement, or exact bytes do not create Required Context classification, participation, applicability, transfer, or authority.

### Core participant-authority qualification defect is accepted as real

- Loom reproduced that the current participant-manufacturing source boundary can derive semantic participant authority from a Task whose lexical participant declaration survives while the Task's c14n-v2 self-integrity no longer qualifies.
- Core must require the exact current-work Task schema and self-integrity to qualify before Task participant declarations may become semantic participant requirements.
- A stale, tampered, schema-mismatched, or otherwise unqualified Task must produce no semantic participant requirement and must fail visible with a dedicated blocking finding.
- Existing manual participant input, cache inventory, Role carriage, endpoint labels, and host state remain non-authoritative for semantic participation.

### Core failure timing must move earlier

- Current manufacture performs expensive bootstrap/archive/package construction before all selected-Handoff/current-work/material blockers are known.
- Blocking semantic/material preflight must be hoisted before bootstrap archive construction and recipient package assembly where the same facts are already available.
- This is a mechanical fail-fast correction only; it must not broaden semantic authority or change the meaning of package success.

### Opaque detached cache is inspectability debt, not semantic authority

- Existing numbered `.bin` cache entries are not themselves a semantic-authority violation because the owning External Payload/cache descriptors already carry non-authoritative transport scope and provenance.
- They are nevertheless a recipient inspectability debt and conflict with the desired human-legible Tiinex transport surface.
- Loom may refactor detached textual material carriage to deterministic, safe, source-shaped or otherwise directly inspectable entry identities/media extensions, plus exact digest/provenance metadata, provided exact bytes, bounded scope, deduplication, authority boundaries, and recipient qualification remain unchanged.
- The refactor must not silently promote detached cache material into a bounded Workspace Representation or new semantic artifact. Any such semantic reclassification requires a separate Axiom/Docs disposition.
- `carried-material` may be used as a human transport/presentation concept only if its implementation remains package/resolver evidence rather than Handoff semantics.

### Party Capacity Reference closure is not widened in this tranche

- A Party endpoint's optional Capacity/Capacity Reference remains an optional resolution aid under current canonical semantics.
- Core must not make Party Capacity material automatically mandatory for package closure merely because the optional Capacity Reference exists.
- If independent current-work, participant, holder, or operation requirements require exact Role/capacity material, that exact requirement may drive closure. Otherwise unresolved optional capacity resolution remains explicitly unresolved rather than guessed or globally searched.
- No Docs schema change is authorized here.

### VS Code confirmed participant-owner violation must be removed

- Kodax established that Attach stores Core's exact qualified participant set, but the live host exposes a later action that can splice one participant locally and forward the weakened subset to Pack.
- Between Attach and Pack, a Core-qualified exact participant projection is immutable host state unless the host explicitly re-runs Core projection and the resulting exact qualified set authorizes the replacement.
- The host must not maintain a partial locally-edited semantic participant set.
- This is a VS Code host correction; it does not require new participant semantics.

### VS Code remains a host, not a second Core

- Filesystem/Git execution, VS Code commands, TreeView/dialog/progress/error presentation, destination-local publication, workspace selection, and host-session choices remain legitimate host responsibilities.
- Shared route qualification, participant authority, carrier allocation, manufacture, material closure, and exact transport text remain Core-owned truth consumed by the host.
- `operatorTrees.ts` is an accepted architecture hotspot because it concentrates otherwise separable host controllers; the correction is to split host responsibilities without moving all host behavior into Core.
- Extension-local `src/core/*` helpers are review surfaces, not automatically semantic defects. They must remain receipt/view-model adapters and must not accumulate new semantic rules.
- `landing.ts` is treated as legacy/suspect rather than active receive evidence; deletion requires compatibility/test reconciliation first.

### Restart/session state must not serialize semantic authority

- The host currently persists Transport presentation state but not general Incoming/Outgoing composition, creating a real lifecycle seam.
- The accepted target is: persist only host identifiers/choices needed for resumability, then re-open and requalify package/Handoff/participant/Core state after restart. Serialized semantic receipts must not become authority merely because they survived workspace state.
- If a particular operation intentionally remains ephemeral, the UI and acceptance tests must make that boundary explicit rather than implying recovery.

## Implementation Sequence

1. Loom/Core implementation tranche first:
   - qualify Task schema/self-integrity before participant derivation;
   - hoist blocking semantic/material preflight before bootstrap/archive/package assembly;
   - improve detached textual material inspectability without changing semantic scope or authority;
   - add focused adversarial and seam-level tests.
2. Anchor consumes and reconciles the Loom return before host implementation continues.
3. Kodax/VS Code implementation tranche against the reconciled Core frontier:
   - remove or Core-requalify participant weakening after Attach;
   - split the operator controller by host responsibility while preserving Core ownership;
   - reconcile legacy receive code deliberately;
   - implement the explicit restart/requalification contract;
   - add actual VS Code Extension Host acceptance for Incoming/Replace/Outgoing/Attach/Pack/Transport under both Local and Published Core bindings.
4. Machine-level cross-layer acceptance must pass before a new Sigma live replay is manufactured.
5. Sigma remains the final human operator/UX gate and is not used as implementation debugger.

## Acceptance Boundary

### Core acceptance

- stale-self-integrity Task with otherwise valid participant prose produces no semantic participant requirement and a blocking finding;
- end-to-end manufacture with that stale current-work Task blocks before package assembly;
- existing manual participant/cache-authority negative tests remain green;
- seam-level evidence proves blocking preflight prevents bootstrap/archive builder entry;
- detached textual carried material is inspectable with deterministic entry identity while digest, exact bytes, bounded scope, provenance, and semantic non-authority remain intact;
- no automatic Party Capacity closure widening is introduced.

### VS Code acceptance

- a real Extension Host flow exercises Incoming, Merge/Replace, Outgoing, Attach, participant presentation, Pack, Transport, restart/reload, and error/progress surfaces;
- host UI cannot retain or Pack a partial participant subset where Core projected an exact set;
- restart restores only host choices/identifiers and requalifies semantic state before action;
- one controller-level flow runs against exact Local Core source and one against the lock-qualified Published Core binding;
- package outputs re-qualify through Core and exact Core-projected transport text is presented without host reconstruction.

## Deferred / Rejected Changes

- No optional `From`/`To` or omitted `Kind` schema change in this tranche.
- No canonical Handoff resolver-state fields in this tranche.
- No conversion of internal `workspaceId::path`-style bindings into durable semantic References.
- No global repository search fallback for unresolved material or identity.
- No automatic cache-to-Workspace-Representation semantic reclassification.
- No broad VS Code rewrite, release, publication, deployment, or remote mutation as part of this reconciliation.

## Reconciliation Evidence

- Axiom + Loom non-overlap reconciliation proof fingerprint: `5ac19c8a3984d740fc2a0509ec663fd4c23c2c2d51c809254163d9f6f80121ca`.
- Axiom + Loom + Kodax non-overlap reconciliation proof fingerprint: `3fefffbb0ad6d9e217dc916e430ecd93bacc2a5ff9efeb811a8ed453c3c5b6e5`.
- Reconciled Business snapshot fingerprint before this Decision: `4f987a7ecf01f559f4bceb17ded218f87311f45c89ec067e759425f364c669df`.
- Mechanical reconciliation reported zero conflicting overlaps, zero deletion candidates, zero unexpected reconciled paths, and complete preservation of all specialist-only artifacts.

## Authority Limits

- This Decision reconciles the bounded architecture-recovery audit only.
- It authorizes the implementation sequence above only through subsequent qualified specialist Tasks/Handoffs; it is not itself source mutation authority for Core or Extension VS Code.
- Axiom retains canonical semantic ownership; Loom retains shared Core implementation responsibility when explicitly delegated; Kodax retains VS Code host implementation responsibility when explicitly delegated; Anchor retains cross-return reconciliation and sequencing; Sigma retains the later human gate.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-architecture-recovery-audit-before-further-host-mutation.trace.md](001-1-4-1-3-architecture-recovery-audit-before-further-host-mutation.trace.md)
  - Value: CwSMZE4hholnEXmxpP2EKrCNx1hOKzVThX58NGr7Glk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: qdY3x0VPVib9xg1MWR3j9eT7W9XgsotrWjeuqkGeZcw