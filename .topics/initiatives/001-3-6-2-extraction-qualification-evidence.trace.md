# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-08 17:38:00
  - Trace: [Extract Core and App; unblock the Playthings consumer](001-3-6-core-app-site-extraction-task.trace.md)
  - Origin:
    - [relative](001-3-6-core-app-site-extraction-task.trace.md)
- Current
  - Current Schema: [tiinex.evidence.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/evidence/tiinex.evidence.v1.schema.md)
  - Created At: 2026-09-08 17:54:00
  - Authors: Anchor
  - Why: Preserve the user-requested source extraction and its actual qualification boundary.
  - Summary: Preserve exact source and distinguish passing local checks from unrun browser qualification.
  - Status: active/local

---

# Core/App/Site installed-package qualification and source-preservation evidence

## Supported Claim Or Question

- Supported Claim Or Question: The six-workspace extraction is preserved as a recoverable checkpoint, with passing local checks and unqualified browser gates distinguished.
- Evidence Role: Supports source preservation and bounded progress, not Turn-1 completion.

## Provenance

- Known Source: Sigma-provided Business, Docs, Site and Playthings ZIPs plus verified Core/App recovery checkpoint.
- Preservation Basis: Complete source Workspaces and embedded delivery reports.
- Provenance Limits: No current Git commit is invented for local uncommitted changes; archive digests identify the supplied inputs.

## Evidence Material

- Material: [Qualification report](../../delivery/STATUS.md); [source inventory](../../delivery/source-inventory.json).
- Material Kind: full-source snapshot and executable-check receipts

## Preservation And Fidelity

- Preservation State: Files preserved in the six carried full Workspaces.
- Fidelity Notes: Source bytes and per-file hashes are recorded; runtime dependencies and Git internals are excluded by the transport policy.
- Known Losses: No new source loss is claimed. A dependency-equipped React/Vite build could not be run in this environment.

## Interpretation Limits

- Does Not Prove: Rendered Playthings behavior, full post-extraction browser qualification, publication, human acceptance or closure.
- Must Not Be Treated As: Canonical meaning, technical approval from Sigma, or evidence that a baseline pass proves the new package composition.

## Review Notes

# Turn 1 — full-source progress checkpoint

Status: **FULL-SOURCE PROGRESS CHECKPOINT; IMPLEMENTATION NOT RELEASE-QUALIFIED.**
This pass preserves six complete source Workspaces. Turn 1 remains open.

## Implemented in this pass

Core owns the extracted portable implementation and public declared-data projections, schema ancestry and companion resource resolution. App owns the extracted Viewer source, a persistent application data store, external Verse registry/React host and bounded companion byte readers. Site now contains one src/main.jsx deployment entrypoint and explicit configuration; reusable runtime source lives in Core/App and is consumed through npm package exports, not copied into Site.

The Viewer remains mounted but hidden during an external Verse. This preserves its intake controller while App exposes the latest snapshot. It is an intentional intermediate state-ownership boundary, not a claim that every old Viewer state machine has been redesigned.

Business carries one forward Viewer-initiative task plus Core/App/Site work links and explicit evidence/Handoff continuity. Historical Site artifacts are retained; qualified historical reduction is Round 2. Docs and Playthings supplied source are unchanged. No GitHub mutation, npm publish, Chrome/CLI/Interop/VS Code work or additional role delegation was performed.

## Executed checks

- Current Core focused regressions: 18/18 passed; portable Node import passed; real embedded bootstrap generation passed (482 runtime files).
- Current App headless/resource/lifecycle tests: 5/5 passed.
- Current Site structural deployment test: 1/1 passed.
- Supplied unchanged Playthings headless suite: 87/87 passed.
- Original unchanged Site baseline regressions: 70/70 passed. This is BASELINE evidence, not post-extraction qualification.
- Static browser source graph: 631 files, syntax/import checks passed; no Node builtins in the browser graph. This is not a Vite bundle or browser test.
- Installed Core/App npm tarballs: isolated npm installation and lock-based npm ci passed with cached exact package bytes; no source symlinks.
- Installed App/Core -> actual supplied Playthings story API: passed with two synthetic records, explicit Parent link and artifact-local companion byte access. The three test bytes are not a rendered PNG or a playable Verse.

## Release blockers / not proved

App and Site npm run validate both stop at the real Vite build with exit 127: vite is not installed. The required external packages cannot be fetched because this runtime receives npm registry DNS EAI_AGAIN. No React/Vite/browser build is claimed. The original full regression suite must still be qualified against the post-extraction composition; the baseline pass does not substitute for it.

The supplied Playthings repository has a headless story/world foundation, not a renderable React Verse entrypoint. App exposes the consumer boundary but Site does not register an invented or fake playable Verse. Runtime snapshots expose declared data; they do not certify schema conformance, participants, identity authority or integrity merely by projection. Generic package companion-manifest generation and every schema-specific participant projection remain to be completed/qualified.

App/Site active lockfiles preserve the external dependency records supplied by Sigma and add exact local Tiinex tarball SRI values. Full registry-based npm ci remains unqualified. Core/App are unpublished local candidates; changed bytes under these candidate versions must not be published until final qualification and version disposition.

CI and OIDC publication workflows are authored, not run in GitHub. Automatic npm publication is disabled by .github/release-policy.json and additionally requires an explicit repository variable. See NPM-SETUP.md. A user commit/push of this checkpoint must not be mistaken for release qualification.

## Next bounded pass

Start with this full-source carrier, preserve all six Workspaces, and use the reports and public App consumer contract. Install the exact external dependencies in a functioning npm-connected environment; run full App/Site builds, post-extraction regression reconciliation and browser mount/Verse-switch tests. Integrate a real Playthings React Verse only when that entrypoint exists. Do not widen scope to VS Code before closing this boundary.

## Preservation

source-inventory.json records checkpoint source hashes before the final Evidence/Handoff additions; exclusions are explicit to avoid a self-hash cycle. Those final artifacts are separately sealed by Tiinex manufacture. Final transport must verify all carried Workspace archive entries against the final working source. The qualified carrier is the recovery input, not installed node_modules or an unreferenced scratch directory.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Extract Core and App; unblock the Playthings consumer](001-3-6-core-app-site-extraction-task.trace.md)
  - Value: SOxxB77pxLrbHBJ3AodTGDgynI770PNNulV-Ov0MPqQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:tF0w9s-oTafXBWQ2MNWQ1AZcrkpajPyv06qmcaU-vSU