# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-26 21:31:11
  - Trace: [009-anchor-to-sigma-vs-code-shared-core-human-parity-merge-candidate.trace.md](../../../handoffs/009-anchor-to-sigma-vs-code-shared-core-human-parity-merge-candidate.trace.md)
  - Origin:
    - [relative](../../../handoffs/009-anchor-to-sigma-vs-code-shared-core-human-parity-merge-candidate.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-26 22:36:06
  - Authors: Anchor
  - Why: Preserve the exact host build diagnosis, bounded correction, qualification, and next real-host gate before another Sigma run.
  - Summary: VS Code-only TypeScript route-projection typing fix after Sigma real-host build blocker; Core remains frozen.
  - Status: ready/local

---

# VS Code Re-entry — Real-Host Build Blocker Closure Evidence

## Supported Claim Or Question

- Supported Claim Or Question: what did Sigma's first real VS Code build reveal, what exact correction was made, and does that correction preserve the frozen Core/shared-tooling boundary?
- Evidence Role: post-Sigma real-host blocker closure and full-recovery checkpoint before the next real Extension Host run.
- Supported Conclusion: Sigma's real Windows `npm run dev:build` reached TypeScript compilation and stopped on exactly five `TS2339` diagnostics in `src/packageBuilder.ts`, all caused by one host-side inference gap in the map joining Core-projected route metadata back to selected UI routes. The correction is a TypeScript-only structural type on that projection map; it adds no runtime branch, fallback, lineage rule, package rule, grounding rule, or Core compensation. Core remains frozen and unchanged. The bridge/runtime regression suite and package-integration suite remain green against the frozen Core implementation.

## Provenance

- Known Source: exact preceding five-Workspace VS Code merge/test candidate; Sigma's uploaded real-host build video showing the five TypeScript diagnostics; the carried VS Code source; frozen Core; and local disposable bridge/package qualification after the bounded type correction.
- Preservation Basis: preserve all five Workspaces and the full shared-Core bridge state. Add only the bounded VS Code type correction and this Business checkpoint; do not reopen Core or revive legacy/V2 behavior.
- Provenance Limits: this Evidence does not claim a second successful real Extension Host launch after the correction. Sigma's rerun remains the human/product gate.

## Evidence Material

- Material: exact current VS Code source, frozen Core source, Sigma's real-host build observation, disposable regression harness output, and package-integration output.
- Material Kind: VS Code-only implementation correction and qualification evidence.
- Real-host blocker: `npm run dev:build` on Sigma's Windows checkout reported five errors in `src/packageBuilder.ts` beginning at the route transport projection join. The diagnostics were `TS2339` for `workspaceId`, `workspaceRelativeHandoffPath`, `workspaceRelativePath`, `to`, and `parties` on an inferred `{}` value.
- Root cause: `new Map(...)` received an `any`-derived tuple sequence, so TypeScript did not retain the structural shape of Core's route projection value even though runtime behavior and tests already used that shape correctly.
- Correction: `projectionById` now has one explicit host-side value type containing only the Core projection fields the bridge reads: `workspaceId`, `workspaceRelativeHandoffPath`, `workspaceRelativePath`, `to`, and `parties.to`. The emitted JavaScript behavior is unchanged.
- No semantic duplication: VS Code still obtains route identity, workspace/path, recipient presentation and transport text from Core projection/manufacture output. The correction does not calculate or infer any Tiinex semantics.
- Core freeze: no Core file was changed. The exact Core implementation carried by the preceding recovery remains the semantic/tooling owner.
- Isolated type proof: the exact corrected `routeRoutingTexts` projection compiles under strict TypeScript with no diagnostics; this specifically closes the five reported property-access errors.
- Bridge regression: 117/117 VS Code bridge runtime cases pass in a disposable installed-binding harness using the frozen Core implementation. Harness-only package-version metadata is aligned to the extension lock expectation so the installed-binding contract tests can execute; Core implementation source is not modified.
- Package integration: 5/5 package integration scenarios pass, including pointerless Pack, exact Workspace reorientation without invented Handoff authority, multi-route Core-qualified routing, idempotent/non-overwriting publication, and extracted VSIX use of the bundled public Core entrypoint.
- App discovery boundary: the App deletions visible in Sigma's SCM view predate this VS Code turn. The App Workspace carried at the beginning and the current carried App Workspace are byte-identical; the removed portable Tooling tests/files match the prior App-to-Core extraction boundary. This Evidence does not claim those App changes as VS Code work.

## Preservation And Fidelity

- Preservation State: Business, Core, VS Code, App, and Docs must all remain in the successor recovery. VS Code carries the type-fixed bridge candidate; Core remains frozen; App/Docs remain exact carried context; Business adds only this checkpoint and successor Handoff.
- Fidelity Notes: no V2 compatibility, host-private route parser, host-private package/grounding semantics, fallback route calculation, manual package resealing, or Core workaround was introduced.
- Known Losses: the corrected source has not yet been rerun by Sigma in the real Windows Extension Host after this exact fix; that is the next acceptance action.

## Interpretation Limits

- Does Not Prove: final Sigma UI acceptance, merge/push, published Core release alignment, or that no later real-host issue can exist.
- Not Yet Used As: remote mutation authority or permission to modify frozen Core.
- Must Not Be Treated As: evidence that the earlier failed Windows build was a semantic Core failure. It was a VS Code TypeScript host-boundary typing defect.
- Disposition: return the corrected full five-Workspace candidate to Sigma for immediate real VS Code `dev:build`/Extension Host rerun. If another concrete blocker appears, resume from this recovery; discuss any genuine Core blocker with Sigma before reopening Core.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [009-anchor-to-sigma-vs-code-shared-core-human-parity-merge-candidate.trace.md](../../../handoffs/009-anchor-to-sigma-vs-code-shared-core-human-parity-merge-candidate.trace.md)
  - Value: cxzRUHCZJ5NIgZdc8I4AjczqGe2soOzxIyXVW_vQkSk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: OU2U7hcl_KJBE-GJtXAi4oIF8659xGo_7VjM_IJmtzQ