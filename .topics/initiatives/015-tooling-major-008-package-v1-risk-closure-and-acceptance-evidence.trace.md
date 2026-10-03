# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-24 02:38:00
  - Trace: [043-anchor-to-anchor-direct-package-v1-machine-qualified-commit-gate.trace.md](handoffs/043-anchor-to-anchor-direct-package-v1-machine-qualified-commit-gate.trace.md)
  - Origin:
    - [relative](handoffs/043-anchor-to-anchor-direct-package-v1-machine-qualified-commit-gate.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-24 13:20:00
  - Authors: Anchor
  - Why: Sigma review exposed ambiguity around participant pointers, public Workspace-qualified pseudo-references, pointer overprojection and cache version identity; those risks were isolated, corrected and replayed before commit/push.
  - Summary: Package V1 risk-discovery is closed for the pre-commit Core candidate: participant combinations, adapter-owned versioned cache, public Reference separation, bounded root-pointer selection, exact recovery and physical/hermetic A/B packages are machine-qualified; immutable Docs commit binding, independent fresh-LLM acceptance and Sigma final acceptance remain open.
  - Status: ready/local

---

# Tooling Major 008 — Package V1 Risk Closure And Acceptance Evidence

## Supported Claim Or Question

- Supported Claim Or Question: does the current pre-commit Core candidate implement the agreed direct Package V1 shape without the identified participant/cache/reference/pointer technical-debt risks, and can representative physical ZIPs be consumed from their own embedded Tooling?
- Evidence Role: machine and architecture-risk qualification for the Task 013 pre-commit frontier.
- Supported Conclusion: yes for the current machine frontier. Final immutable canonical Docs binding, independent fresh-LLM behavioral acceptance, Sigma acceptance and Core freeze are intentionally not claimed.

## Provenance

- Controlling Task: [Task 013](013-tooling-major-008-handoff-package-v2-purge-and-native-v1-rebuild.trace.md).
- Prior Checkpoint: [Handoff 043](handoffs/043-anchor-to-anchor-direct-package-v1-machine-qualified-commit-gate.trace.md).
- Evidence Boundary: exact local Core, Docs and Business Workspace bytes used for this recovery checkpoint; no remote mutation and no VS Code implementation.

## Risk Discovery And Closure

- Multi-Participant Identity: participant requirement identifiers are stable by semantic identity rather than array order; three participant Roles no longer cross-bind after sorting.
- Carried-First Resolution: exact carried participant/context material resolves before cache and is not duplicated into cache; zero, three-carried, three-cache-only, mixed carried/cache and endpoint/participant overlap cases are green.
- Public Reference Boundary: Package V1 Pointer Reference preserves a true adapter-native reference when available and does not expose an internal Workspace coordinate such as `business::path` as if it were a source permalink. Workspace Id/path remain separate package-local resolution identity.
- Root Pointer Boundary: root route closure is limited to pre-Handoff Process/Policy pointers, explicit participant Role pointers, From/To Role pointers and the final authoritative Handoff pointer. Ordinary Task/Evidence/Workspace Required Context is resolved after Handoff selection rather than projected as redundant root pointers.
- Adapter-Owned Cache Identity: GitHub cache entries are `github/<owner>/<repo>/<exact-commit>/<repo-relative-path>`; the same repository path at two exact commits coexists without collision. No `blob/`, generic `material/`, hidden mapping JSON or `.bin` indirection is used.
- Adapter Fail-Closed Boundary: unpinned GitHub cache identity and unsupported external adapters fail closed; they do not silently fall back to native cache semantics.
- Automatic Carried GitHub Binding: absent an explicit qualified material binding, automatic permalink-to-carried-Workspace binding requires the Workspace source entrypoint to declare the same exact commit.
- Recovery: missing ordinary Required Context receives exact read-only host recovery when available and exact manual-input recovery otherwise; returned bytes must re-enter Tooling verification before authority is restored.

## Machine Evidence

- Full Core Validation: `npm run validate` passes 236/236 Node tests, portable smoke and embedded bootstrap qualification after the final risk fixes.
- Focused Package/Endpoint/Recovery Matrix: the final focused run passes 37/37 tests across direct Package V1, participant combinations, endpoint authoring separation and recovery.
- Retired V2 Sweep: active Core `src/` and `tools/` contain zero retired Handoff Package V2 support hits for the guarded recipient/archive/bin/hidden-carrier tokens. Historical trace provenance and the c14n-v2 integrity method are not treated as Handoff Package V2 support.
- Acceptance A: one physical Core-produced ZIP has one route, zero extra participant pointers, no cache, carried Anchor Role, separate From/To pointers and final Handoff pointer; physical roundtrip, orientation and grounded-to-act pass.
- Acceptance B: one physical Core-produced ZIP has Process + Policy + Sigma + Loom + Axiom participant pointers + From/To + Handoff; its bounded cache contains only versioned `github/Tiinex/business/<exact-commit>/...` entries; physical roundtrip, orientation and grounded-to-act pass.
- Hermetic Acceptance B: from an empty host directory containing only the untouched B ZIP, the declared embedded bootstrap was extracted and its own `tiinex-portable.mjs` returned `orient: ready` and `ground: grounded-to-act` without npm install, internet or a Core checkout.

## Remaining Gates

- Sigma commits/pushes exact Core, Docs and Business Workspace bytes.
- Anchor resolves the new Docs commit read-only and binds Package V1 schema references to that immutable commit, then reruns validation and A/B/hermetic replay.
- A genuinely fresh no-precontext LLM receives only the final package/Start instruction and must independently orient/ground/reconstruct the bounded continuation without producer-chat help.
- Sigma reviews the final representative ZIP shape/usability.
- Only after Sigma acceptance is Core frozen and VS Code thawed for thin-consumer work.

## Interpretation Limits

- This Evidence does not claim that package-carried Role pointers create semantic participant authority; they ground exact Role material only.
- This Evidence does not claim the current local Docs schema has an immutable GitHub commit yet.
- This Evidence does not claim fresh-LLM or Sigma acceptance.
- This Evidence does not authorize remote write, commit, push, release or VS Code implementation.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [043-anchor-to-anchor-direct-package-v1-machine-qualified-commit-gate.trace.md](handoffs/043-anchor-to-anchor-direct-package-v1-machine-qualified-commit-gate.trace.md)
  - Value: faNuWREIHK-8su5QCmgU2lQuyVPuDJJhYJzBuUrtDws

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:IPvXRElFqJ603cJG0G8OgaR_pEBAQk1SYVDsoejX7HQ
