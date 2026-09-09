# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-09 15:45:03
  - Trace: [001-turn-2-repository-decomposition-frontier.trace.md](../001-turn-2-repository-decomposition-frontier.trace.md)
  - Origin:
    - [relative](../001-turn-2-repository-decomposition-frontier.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-09 16:59:49
  - Authors: Anchor
  - Summary: Turn 2 renamed repository and runtime bootstrap readiness evidence
  - Status: ready/local

---

# Turn 2 renamed repository and runtime bootstrap readiness evidence

## Supported Claim Or Question

- Supported Claim Or Question: what exact current Refactor source set is ready for Sigma to land after the repository renames and runtime/Chrome frontiers, and which npm repositories have the local source/workflow prerequisites for `publish:bootstrap`
- Evidence Role: supports source identity, repository-lineage, local qualification and operator-bootstrap readiness claims for this progression

## Provenance

- Known Source: the Refactor Anchor current integration tree under `/mnt/data/anchor-turn2/integration`, descended from the previously surfaced 13-Workspace Handoff and reconciled with Sigma-reported repository renames/creation
- Remote Metadata Cross-check: read-only GitHub repository metadata confirmed `Tiinex/runtime-native`, `Tiinex/extension-chrome`, `Tiinex/interop-native`, `Tiinex/extension-vscode`, and `Tiinex/verse-playthings` exist. GitHub visibility is not used as current-source authority and no repository source was reconstructed from the connector.
- Preservation Basis: the forthcoming Handoff carries full source for every Workspace it claims. The previous surfaced Handoff remains recovery provenance for predecessor repository/Workspace identities.
- Provenance Limits: newly created/renamed repository commits and npm registry publication do not yet exist for this local source progression; remote metadata does not prove that Sigma's local worktrees equal these carried bytes

## Evidence Material

- Material Kind: bounded source, package-readiness and test receipt
- Material: current carried repositories are `business`, `docs`, `core`, `app`, `site`, `extension-vscode`, `extension-chrome`, `verse-playthings`, `provider-native`, `provider-github`, `verse-native`, `verse-atlas`, `interop-native`, `interop-openai`, and `runtime-native`; `cli` remains not source-established and is not fabricated. Repository-local Tasks/Subtasks for the new Runtime and Chrome frontiers point back to controlling Business topics, and current rename Tasks exist for Extension VS Code and Interop Native. `provider-native`, `provider-github`, `verse-native`, `verse-atlas`, `interop-native`, `interop-openai`, and `runtime-native` each passed 1/1 package-boundary identity test plus `npm pack --dry-run`. A machine receipt at `receipts/npm-bootstrap-readiness-2026-09-09.json` confirms package identity, repository URL, public publish config, `publish:bootstrap`, master release-policy, OIDC `publish.yml`, npm environment and publish gate are present for those packages and for `verse-playthings`. Current Core passed 40/40 tests; App passed 8/8 headless tests; Site passed 2/2 deployment/package-boundary tests. Extension VS Code passed 37/37 bridge core cases when the exact current Core package source was temporarily materialized at its expected installed-package location; the temporary `node_modules` material is not carried. Verse Playthings passed 219/219 runtime tests, installed-package test, release-policy test and 22/22 App/Core adapter tests.

## Preservation And Fidelity

- Preservation State: runtime-only `.tiinex` state, temporary dependency material and `node_modules` are excluded from canonical source. Historical artifacts that truthfully name predecessor repositories/packages are not mass-rewritten.
- Fidelity Notes: active package/release surfaces use `@tiinex/verse-playthings`, `@tiinex/interop-native`, and `@tiinex/runtime-native`; Extension VS Code repository identity is `Tiinex/extension-vscode` while VSIX/product identity remains independent. Predecessor Workspace artifacts may remain as explicit recovery/history context where carried lineage still references them.
- Known Losses: no final browser E2E, final Viewer/Verse extraction, provider extraction, Site historical Reduction, VS Code 0.1.8 release qualification, Chrome implementation qualification, Runtime implementation qualification or npm publication is claimed

## Interpretation Limits

- Does Not Prove: final Turn-2 stability, npm Trusted Publisher configuration, successful `publish:bootstrap`, successful Git landing, Marketplace/Chrome Store readiness, or human product acceptance
- Not Yet Used As: final Turn-2 acceptance or authority to publish packages automatically
- Must Not Be Treated As: evidence that GitHub latest is current source, evidence that repository creation equals implementation completion, or evidence that passing package scaffolds freeze future public contracts

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-turn-2-repository-decomposition-frontier.trace.md](../001-turn-2-repository-decomposition-frontier.trace.md)
  - Value: FSTPBfQmP7ZXOwuLt5OxiGGRIC7uF4WtwqPKJO54Dzw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: QXe-WZQr9kO8ohBZy3PJWTE4YoFT7Mvfhxk8MZmzdz8