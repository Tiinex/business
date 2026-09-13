# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-13 16:11:46
  - Trace: [001-1-anchor-to-loom-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md](001-1-anchor-to-loom-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md)
  - Origin:
    - [relative](001-1-anchor-to-loom-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-13 16:35:10
  - Authors: Loom
  - Why: The delegation requires fail-closed active-WIP protection plus exact evidence suitable for Anchor disposition.
  - Summary: Qualify exact target-byte landing preflight, coarse Recovery acceptance audit, and broad Core validation.
  - Status: ready/local

---

# Recovery Major 001 — Loom Recovery Integrity Implementation Evidence

## Supported Claim Or Question

- Supported Claim Or Question: whether Recovery landing now fails closed before destructive mutation when a live target contains current-only or byte-divergent durable source, while exact-safe targets remain green, without promoting unaccepted target WIP into accepted Recovery
- Evidence Role: bounded Loom implementation and validation evidence for Recovery Major 001

## Provenance

- Known Source: qualified Anchor → Loom Recovery Major 001 delegation, exact package-carried Core Workspace basis, and the package-carried portable Tooling bootstrap used to materialize and validate the candidate
- Preservation Basis: Core candidate was materialized from the qualified package provider after Tooling takeover; edits are confined to host-neutral portable landing/audit mechanics, CLI integration, package export, and focused tests
- Provenance Limits: no canonical schema semantics, artifact history, extension-vscode feature source, or accepted Recovery state were rewritten; target WIP is detected but never auto-promoted

## Evidence Material

- Material: `project-workspace-landing` no longer treats a repository-level `clean` boolean as replacement authority. The CLI captures an exact target durable-source snapshot using the same local enumeration/source-eligibility contract as Handoff manufacture. The landing plan builds an incoming frontier from the qualified package provider and reconciles it against the exact current target with accepted Recovery serving as base+incoming. Exact bytes return `exact-safe` / `land`; any target addition, deletion, or byte change returns `reconciliation-required` / `stop` with deterministic path-level current-change evidence before mutation. A clean-but-divergent target therefore blocks, while an exact target remains green even if the coarse Git cleanliness flag is false. The new `audit-recovery-acceptance` independently qualifies accepted-basis and candidate carriers, re-materializes selected Workspace bytes through the package provider, requires complete candidate coverage, compares exact source frontiers, and blocks unexplained removals while explicitly leaving Git committability and semantic acceptance unproven. An exact Core package round-trip reports complete coverage, zero changes/removals, and `restart-source-ready`. Broad Core validation passed on the exact candidate bytes: `npm run validate` completed 106/106 Node tests, portable smoke, and embedded bootstrap verification. Exact basis→candidate source comparison reports one added file, eight byte-changed files, zero removed files, and no comparison findings. Focused landing regression proves an exact target is green; a clean target with no exact snapshot fails closed; and a target with `.topics/handoffs/return.trace.md` byte divergence plus `src/current-only-wip.txt` addition blocks as `reconciliation-required` with both exact paths identified before mutation.
- Material Kind: exact host-neutral Core Tooling candidate bytes, focused regression assertions, broad validation, source-frontier comparison, and package-carrier audit evidence

## Preservation And Fidelity

- Preservation State: accepted Recovery remains the comparison basis and candidate package source; current target WIP is classified as target-side divergence and is neither copied into Recovery nor silently removed
- Fidelity Notes: the implementation reuses existing source-frontier and three-way reconciliation semantics instead of introducing a parallel merge policy; Git cleanliness remains informational rather than authoritative for destructive replacement
- Known Losses: the coarse acceptance audit intentionally does not prove repository commit state or semantic acceptance; Anchor retains those dispositions

## Interpretation Limits

- Does Not Prove: any current-only target byte is accepted work, that Git cleanliness alone is sufficient for landing, or that the Recovery acceptance audit grants Master Recovery acceptance
- Not Yet Used As: Anchor integration acceptance, final Master Recovery disposition, or Sigma-facing committability guarantee
- Must Not Be Treated As: permission to merge, delete, revert, or promote active target WIP automatically

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-anchor-to-loom-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md](001-1-anchor-to-loom-recovery-major-001-committable-full-recovery-and-active-wip-protection.trace.md)
  - Value: xzbFm8w-iXRSE6KHEof2uyCeGRN0Dwn7FUqT7ofahWo

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: jZuerCXV5ne6S5HpPpaVOA074T0oZ58Nv4rZZG8COF4