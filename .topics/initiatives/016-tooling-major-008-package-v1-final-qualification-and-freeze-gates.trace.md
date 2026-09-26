# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-24 13:21:00
  - Trace: [044-anchor-to-anchor-package-v1-risk-closed-recovery-frontier.trace.md](handoffs/044-anchor-to-anchor-package-v1-risk-closed-recovery-frontier.trace.md)
  - Origin:
    - [relative](handoffs/044-anchor-to-anchor-package-v1-risk-closed-recovery-frontier.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-24 13:35:00
  - Authors: Anchor
  - Why: Task 013 is already integrity-pinned by downstream Handoffs and must remain byte-stable; the risk-closed Package V1 implementation therefore needs a successor Task for the remaining immutable-source, fresh-LLM, Sigma and freeze gates.
  - Summary: Preserve the accepted direct Package V1 architecture and complete only the post-risk-closure gates: immutable Docs commit binding, full replay, independent fresh-LLM package-only acceptance, Sigma review and Core freeze before VS Code resumes.
  - Status: ready/local

---

# Tooling Major 008 — Package V1 Final Qualification And Freeze Gates

## Objective

Complete Tooling Major 008 from the risk-closed direct Package V1 frontier without changing the now-locked receiver architecture or mutating historical Task 013 continuity.

The current pre-commit implementation is already machine-qualified for direct V1 manufacture/orient/ground, participant combinations, adapter-owned versioned cache, public Reference separation, root-pointer selection, read-only/manual recovery and hermetic embedded-Tooling execution. This successor Task exists because Task 013 already has integrity-pinned descendants and must not be edited in place merely to record new progress.

## Locked Package V1 Boundaries

- One direct manufacture path: qualified Core plan -> Package V1 allocation/materialization -> direct V1 verification -> physical ZIP.
- No recipient-v2/Handoff-Package-V2 builder, converter, verifier, writer or fallback.
- `sha256-base64url-c14n-v2` remains the trace integrity method and is unrelated to the retired package representation.
- Workspace ZIPs are repo-root byte trees with no organization/repository or commit wrapper directory.
- Cache is bounded to exact required material absent from carried Workspaces and never duplicates carried bytes.
- Each adapter owns its deterministic collision-safe cache identity beneath its namespace.
- GitHub cache layout is exactly `github/<owner>/<repo>/<exact-commit>/<repo-relative-path>`; no `blob/`, generic `material/`, opaque `.bin`, central hash lookup or hidden JSON mapping truth.
- Public Package V1 `Reference` preserves a qualified adapter-native reference when available. Internal Workspace coordinates such as `business::path` may remain internal resolution identity but must not masquerade as provider/source references.
- Root route pointers are limited to pre-Handoff Process/Policy grounding, explicit 0..N participant Roles, From Role, To Role and the final authoritative Handoff. Ordinary Task/Evidence/Workspace Required Context resolves after Handoff selection.
- Participant Role pointers are separate from From/To endpoint pointers; endpoint/participant overlap may share exact material but not semantic pointer role.
- Adapter-native resolution order remains carried Workspace -> bounded cache -> read-only provider/host -> exact manual input -> verify/fail closed.
- Unsupported external adapters and unpinned GitHub cache identities fail closed rather than falling back to generic/native caching.

## Qualified Pre-Commit Evidence

Evidence 015 records the current machine state:

- full Core validation: 236/236 tests plus portable smoke and embedded bootstrap qualification;
- zero active retired Handoff Package V2 support hits in Core `src/` + `tools/` for the guarded implementation tokens;
- participant matrix: zero, three cache-only, three carried, mixed carried/cache and endpoint/participant overlap all green;
- physical Acceptance A: single route, zero extra participants, cache-free, From/To/Handoff only;
- physical Acceptance B: Process + Policy + Sigma + Loom + Axiom participant Role pointers + From/To + Handoff with versioned GitHub bounded cache;
- Acceptance B hermetic replay: empty host + untouched ZIP + declared embedded bootstrap -> orient ready -> ground grounded-to-act without npm, internet or Core checkout;
- recovery architecture: complete Business + Core + Docs Workspace carriage with only semantically required root pointers and no cache when all required bytes are carried.

## Remaining Gates

### Gate A — Immutable Canonical Docs Binding

After Sigma commits/pushes the exact carried Core, Docs and Business bytes:

- resolve the new Docs commit read-only;
- verify that the committed Package V1 schema bytes exactly match the locally qualified schema bytes;
- bind Core's canonical Package V1 schema target/bootstrap representation to that immutable Docs commit;
- do not use GitHub mutation from Anchor.

### Gate B — Final Machine Replay

After immutable binding:

- rerun full Core validation and retired-V2 anti-drift sweep;
- rebuild Acceptance A and B using the final bound Core;
- verify physical ZIP roundtrip, root pointer selection, public Reference boundary, versioned adapter cache paths and no carried-byte cache duplication;
- rerun the empty-host embedded-bootstrap orient/ground/continue challenge.

### Gate C — Independent Fresh LLM Acceptance

A genuinely fresh no-precontext LLM receives only the final Handoff Package and the explicit Start/routing instruction. It must independently use packaged Tooling to orient, ground exact Workspaces/cache/Roles/Process/Policy, identify unresolved recovery needs without substitution, reconstruct the bounded current Task/Handoff authority and continue without producer-chat memory.

Machine-hermetic execution is necessary but does not substitute for this behavioral gate.

### Gate D — Sigma Review And Core Freeze

Present at least the simple and multi-participant/cache representative ZIPs to Sigma. If Sigma rejects structure/usability, return only to Core/Docs as needed while VS Code remains frozen.

After Sigma accepts the machine behavior and human package shape, record the Package V1 Core freeze. Only then may the separate VS Code thin-consumer task begin.

## Scope

- Final Core + Docs + Business continuity needed to complete Package V1 acceptance and freeze.
- Read-only source qualification after Sigma commit/push.
- Final A/B/hermetic/fresh-LLM/Sigma gates.
- VS Code implementation is excluded until explicit Core freeze.

## Dependencies

- [Original Task 013](013-tooling-major-008-handoff-package-v2-purge-and-native-v1-rebuild.trace.md) remains historical controlling authority for the purge/direct-V1 recovery and is byte-stable.
- [Evidence 015](015-tooling-major-008-package-v1-risk-closure-and-acceptance-evidence.trace.md) records the risk-closed pre-commit machine frontier.
- Sigma supplies commit/push transport and final human acceptance.

## Done Criteria

- new immutable Docs commit exactly matches the qualified canonical Package V1 schema bytes;
- final Core schema target/bootstrap binds to that commit and all Core machine/anti-drift tests pass;
- final A/B physical packages and empty-host embedded-bootstrap replay pass;
- independent fresh-LLM package-only acceptance passes;
- Sigma accepts representative Package V1 shape/usability;
- Core Package V1 freeze is recorded before VS Code implementation resumes.

## Interpretation Limits

- This Task does not reopen the retired V2 architecture or authorize compatibility fallback.
- This Task does not authorize changing historical Task 013 merely to update status.
- Participant Role carriage does not itself create semantic participant authority.
- Package/cache/reference location does not replace semantic artifact authority.
- Anchor has no remote GitHub write, commit, push, release or publication authority.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [044-anchor-to-anchor-package-v1-risk-closed-recovery-frontier.trace.md](handoffs/044-anchor-to-anchor-package-v1-risk-closed-recovery-frontier.trace.md)
  - Value: mgMS4VhnpIrJVuAdk-QkecmYvlxPreqloKdpFcjPSUg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:5JtuWr2GjE1KvS2X_j74ZSWulNQRF9AANy9FbMI5Fm4
