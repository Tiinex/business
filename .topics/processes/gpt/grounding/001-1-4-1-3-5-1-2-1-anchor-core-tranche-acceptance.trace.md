# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 15:10:29
  - Trace: [001-1-4-1-3-5-1-2-loom-to-anchor-core-participant-preflight-and-carriage-inspectab.trace.md](001-1-4-1-3-5-1-2-loom-to-anchor-core-participant-preflight-and-carriage-inspectab.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-5-1-2-loom-to-anchor-core-participant-preflight-and-carriage-inspectab.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-21 15:27:28
  - Authors: Anchor
  - Why: Independent Anchor source and test acceptance confirms the bounded Core repair while preserving explicit suite and cross-layer limits.
  - Summary: Accept the bounded Loom Core participant/preflight/inspectability repair and reopen the reconciled VS Code host lane without promoting partial suite evidence into full acceptance.
  - Status: ready/local

---

## Decision

- State: accepted
- Subject: Anchor acceptance of Loom Core participant, preflight, and detached-text inspectability tranche
- Decision: accept the bounded Loom Core implementation as satisfying the delegated Core tranche sufficiently to resume the separately reconciled VS Code host correction lane, while preserving the explicit limitation that no clean full wildcard-suite process exit was observed and no cross-layer or Sigma acceptance is implied.

## Acceptance Basis

- Exact Tiinex source-frontier comparison between the Anchor-to-Loom carrier and Loom return reports Core with zero added files, zero removed files, and exactly ten byte-changed files; Docs is byte-exact; Business adds only the Loom Evidence and Loom-to-Anchor return Handoff for this tranche.
- Independent comparison against current `Tiinex/core@master` confirms all 816 Core files outside the declared ten-file tranche are byte-identical to the remote tracked baseline.
- Anchor reran the focused compatibility surface on the exact returned Core bytes: 37/37 tests passed with clean process exit across bounded carrier, endpoint Role route binding, participant projection, manufacture hygiene, minimal carrier/material transport projection, and source-frontier comparison coverage.
- Anchor reran the four new adversarial seams from the large blank-workspace regression file individually: tampered current-work Task blocks participant authority, self-verified non-canonical current-work Task blocks participant authority, participant preflight blocks before tooling bootstrap construction, and unresolved required material blocks before recipient package assembly; 4/4 passed with clean exit.
- Anchor reran the detached-text inspectability/roundtrip specimen individually; it passed with clean exit and verified exact textual bytes, media type, source-shaped archive identity, digest preservation, cold orientation, and grounding boundaries.
- `npm run test:portable` exited clean with `portable node surface imports`; `npm run test:bootstrap` exited clean with `embedded-qualified`, 516 runtime files, manifest SHA-256 `5f9f3f881be8f9703eb0a647b25f1f1fccce3a3b1a1561223518f2edc13e9705`, and representation SHA-256 `84f34d18020ed0f02cbccc1ee1f13ff8fa48325a086f43bdf43cf2c9fada3da5`.
- The earlier apparent source-hygiene concern from literal NUL separators in `recipientV2.topology.materials.js` is not a Loom-introduced delta: the exact pre-Loom/GitHub baseline already contains the same three NUL separators. It is not promoted into a blocker or silently attributed to this tranche.

## Accepted Technical Disposition

- Semantic participant manufacturing now requires an exact current-work Task whose schema is canonical `tiinex.task.v1`, whose primary c14n-v2 self-digest verifies, and whose canonical Task validator has no error findings before participant declarations may create transport requirements.
- A present but stale, tampered, schema-mismatched, or otherwise unqualified current-work Task yields zero semantic participant requirements and an explicit blocking finding; manual participant input, cache/Role inventory, Handoff endpoints, filenames, package proximity, and host/session state remain non-authoritative.
- Blocking selected-Handoff/current-work/material preflight now occurs before tooling-bootstrap construction and before recipient package assembly when the blocking facts are already available. The qualified baseline still computes its own closure plan, so fail-fast timing does not become an alternate semantic path.
- Detached textual carried material remains External Payload/cache transport evidence. It gains deterministic safe source-shaped archive identity plus visible media type while exact bytes, SHA-256, provenance, bounded scope, deduplication, and semantic non-authority remain preserved.
- No Handoff endpoint/kind schema change, resolver-state field, Party Capacity closure widening, cache-to-Workspace-Representation reclassification, or internal-binding-to-durable-Reference promotion is accepted.

## Retained Limitations

- The full wildcard Core suite and the full large blank-workspace test process did not provide a clean complete process exit in Loom's environment; completed PASS assertions are evidence, not a substituted full-suite PASS.
- This Decision does not establish Extension VS Code correctness, real Extension Host lifecycle acceptance, Published/Local parity, Sigma acceptance, release readiness, or remote mutation authority.
- Pre-existing source-format debt outside the ten-file Loom delta is not silently folded into this acceptance.

## Next Sequence

- Resume the separately reconciled Kodax/Extension VS Code lane against these exact accepted Core bytes.
- Kodax must remove host-local weakening of exact Core participant projections, keep shared route/packing/material/transport truth Core-owned, split the operator hotspot only along legitimate host-controller boundaries, and requalify semantic state after restart rather than serializing semantic authority.
- The Kodax return must include machine-level coverage of the real host/controller path and a true Extension Host acceptance attempt across Incoming/Replace/Outgoing/Attach/participant presentation/Pack/Transport and Local/Published bindings. Any environment blocker must remain explicit rather than becoming a synthetic PASS.
- Anchor will reconcile the Kodax return against this accepted Core frontier and the prior independent host audit before manufacturing any Sigma gate.

## Authority Limits

- This Decision accepts only the bounded Core tranche returned by Loom.
- It authorizes progression to the already-reconciled VS Code implementation lane through a new qualified Kodax Task/Handoff; it is not itself Extension VS Code mutation authority.
- Loom qualification remains technical evidence, Anchor owns this tranche acceptance, Kodax owns only subsequently delegated host implementation, Axiom/Docs retain canonical semantics, and Sigma retains the final human operator gate.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-5-1-2-loom-to-anchor-core-participant-preflight-and-carriage-inspectab.trace.md](001-1-4-1-3-5-1-2-loom-to-anchor-core-participant-preflight-and-carriage-inspectab.trace.md)
  - Value: oyB4i60oRg5H8fXyxch4elRh1qvDCJGtjJP20KL6BKg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: zTXZ92BWFrRrCNXQPEQCnkFEQsXbnGqljHWQb4HW7Nk