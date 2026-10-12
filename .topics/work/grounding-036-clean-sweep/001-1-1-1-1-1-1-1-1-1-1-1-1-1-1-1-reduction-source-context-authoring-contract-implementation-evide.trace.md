# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-10-12 10:22:54
  - Trace: [001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-sigma-to-anchor.trace.md](001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-sigma-to-anchor.trace.md)
  - Origin:
    - [relative](001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-sigma-to-anchor.trace.md)
- Current
  - Current Schema: [tiinex.evidence.v1](https://github.com/Tiinex/docs/blob/9ef3c2caed38152b1948c93cb45c985786660d91/.topics/.schemas/core/evidence/tiinex.evidence.v1.schema.md)
  - Created At: 2026-10-12 10:57:37
  - Authors: ChatGPT (grounding collaboration; holder unverified)
  - Why: Respond to Sigma Reduction consistency feedback with actual Tooling mechanics and tests
  - Summary: Implemented reduction source authoring enforcement, contract sync and historical migration limits
  - Status: draft/local

---

# Reduction Source Context — Authoring Contract Implementation Evidence

## Supported Claim Or Question

- Supported Claim Or Question: Does the proposed compact Reduction Source Context convention now guide creation and fail closed under the actual Tiinex authoring and draft-validation pathways, without silently invalidating historical Reductions?
- Evidence Role: Source-bound code/schema/scaffold change and executable preflight evidence for bounded Sigma review; not a published Tooling release, human acceptance, or destructive Reduction eligibility proof.

## Provenance

- Known Source: incoming qualified `tiinex-036-1-1-1-1-1-1-1-sigma-to-anchor.handoff-package.zip`, SHA-256 `c73a14f29bc1fdbf56f7c11079d928e0c186765dbfa9e8fb700b77e56fb51b12`, 17 Workspace members; its current Business Task and Sigma feedback remain unchanged. Compare only the new candidate Workspace sources under the same frozen carrier; no remote source mutation.
- Preservation Basis: initial source archive is retained unchanged. Code/schema/scaffold sources were edited in a disposable Workspace copy, and the schema's c14n-v2 self-integrity resealed after its change. The Native schema pack was regenerated with canonical `schemas-sync`, not manually patched.
- Provenance Limits: tool results establish local source-level behavior, not remote publication, recipient readiness of an as-yet-unmanufactured carrier, or a global schema migration authorization.

## Evidence Material

- maintained-schema-and-scaffold
  - Material: Docs `tiinex.reduction.v1.schema.md` keeps exactly the four existing Reduction body headings. Its Minimal Example uses Sigmas `001-clean-up` style: Workspace-grouped commit-pinned clickable source links with per-file c14n-v2 or raw SHA-256 where appropriate. Historical recovery and source-type exceptions remain truthful; verbose raw ledgers are not the primary Source Context. Native workspace-reduction scaffold now prefers a flat `.topics/reductions/` and the exact maintained compact source shape.
  - Material Kind: exact local Docs and Native file revision, c14n-v2 self-integrity and `schemas-sync`/`schemas-check` receipts.
  - Description: Regeneration updated five Native schema-pack outputs (including inherited redaction runtime and catalog). `schemas-check` returned ready, zero errors and zero warnings.
  - Material Limits: Schema note alone is not machine enforcement and does not assign publication authority.
- real-creation-enforcement
  - Material: Core adds `src/tooling/portable/reduction/reduction.sourceContext.js` and uses it in `cli.common-author.js` **before writing**, and `draft.operations.js` to catch other local prospective stage-draft sources. The accepted new-authoring grammar handles published commit-pinned `.trace.md` and `.schema.md` sources with c14n-v2, binary Git assets and exact carrier/runtime sources with raw SHA-256, and maps `extension-vscode` Git repository to `vscode` Workspace.
  - Material Kind: source implementation, actual Tiinex `author --preflight` and targeted node:test.
  - Description: A Sigmas-format published-source Reduction returned `qualified-preflight`, zero errors and warnings. The old `- Source: old stuff` prose returned a fail-closed `portable.cli.author.reduction-source-context.invalid` without creating an artifact. Fourteen isolated parser/stage tests passed; this new rule applies on creation and draft validation, not retroactive canonical audit of previous exact schema revisions.
  - Material Limits: This is structural validation. It does not fetch actual source bytes, qualify Source meaning, guarantee external URL immutability beyond pinned Git locator syntax, or authorize deletion. An external carrier label requires independent exact bytes/digest checking.
- existing-history-migration-limit
  - Material: Current 17-Workspace candidate contains 21 existing `.topics/reductions/**/*.trace.md`; a strict check against the NEW authoring grammar marked 2 fully conforming, 19 legacy/nonconforming. Examples: Business `002-directory-local-namespace-and-flat-reduction-convergence.trace.md`, Interop OpenAI `001-1-chatgpt-web-operator-annotation-lineage-consolidation.trace.md`, and the historical standalone/consolidated Reduction roots.
  - Material Kind: read-only format inventory of unchanged carried current artefacts.
  - Description: These 19 remain valid historical source as qualified by the carried original Schema; blindly changing them would reseal parents used by still-current Role/Handoff/Reduction chains. Their future reauthoring is a separately qualified lineage/recovery action, not silently implied by schema evolution.
  - Material Limits: Format-audit classification is not a semantic validity verdict or authorization to rewrite old history. Full legacy migration was intentionally not represented as complete by this implementation.
- broader-test-limit
  - Material: Four previously existing raw Core tests related to generic creation and root/Redaction authoring were run without the packaged canonical Test runner; 8 of 22 subtests failed due missing contract/runtime initialization. New source-context tests passed. These failures are documented rather than relabeled regression PASS; the packaging path and recipient runtime still require separate source-based qualification.
  - Material Kind: actual Node test receipts and source-runtime Tooling checks.
  - Description: Native, Docs and Business individual Workspace qualifiers returned `ready` and no findings after new schema sync and code changes.
  - Material Limits: No complete, independent Core CI or VS Code Windows suite PASS established by this test selection.

## Preservation And Fidelity

- Preservation State: Changed sources in Core, Docs and Native are carried as complete Workspace candidates; original qualified carrier is the source/recovery boundary. Previous historical Reduction bytes remain unchanged.
- Fidelity Notes: One new Reduction format is enforced only for prospective creation. No synthetic Git URLs are produced for unpublised carrier/runtime snapshots and the Tooling validator does not pretend to compare remote bytes.
- Known Losses: Historical Reduction prose/manifest complexity is not rewritten in this bounded source-convention implementation. A full lifecycle-safe source migration and separately qualified publish/build remain unresolved.

## Interpretation Limits

- Not Yet Used As: Sigma final clean-sweep PASS, remote release acceptance, destructive lineage eligibility, Role holder authority, or complete CI result.
- Does Not Prove: all old Reductions were migrated, that every `Source Context` claimed public URL is byte-verified, or that the old bundled runtime has already been replaced on remote installed hosts.
- Must Not Be Treated As: approval to mass-rewrite already-signed historical Reductions or substitute a new Release for current signed carrier source.
- Must Not Be Used To Claim: everything in Tiinex has one historical Reduction presentation style today or that no further validation is needed.
- Need For Review: source code, schema and native pack adoption; executable author/preflight and draft tests; later source-recovery-safe legacy normalization and human acceptance.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-sigma-to-anchor.trace.md](001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-sigma-to-anchor.trace.md)
  - Value: ZWitrgmDQQT-A5zW-WFsJJZ65RaPdWZO-Y2qDWkKZ8Q

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: Al_QmGOp5b6zgeO3THzDUUVKxjL2X8vCBIjz6VuLo8E