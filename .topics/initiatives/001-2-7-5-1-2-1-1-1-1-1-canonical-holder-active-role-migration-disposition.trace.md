# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-15 21:59:25
  - Trace: [001-2-7-5-1-2-1-1-1-1-identifier-only-historical-role-parent-authoring-correction.trace.md](001-2-7-5-1-2-1-1-1-1-identifier-only-historical-role-parent-authoring-correction.trace.md)
  - Origin:
    - [relative](001-2-7-5-1-2-1-1-1-1-identifier-only-historical-role-parent-authoring-correction.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-15 22:41:47
  - Authors: Anchor
  - Summary: Accept the complete eight-Role canonical holder migration and authorize final removal of legacy-positive holder authorization after Core verification.
  - Status: ready/local

---

# Canonical Holder Active Role Migration Disposition

## Decision

- State: accepted
- Subject: active Tiinex Role holder-assignment cutover
- Decision: the explicitly scoped active Role set for this cutover is now represented by one canonical `tiinex.party.role.v1` continuation per Role with direct canonical `Assignment Modes`. The active set is Anchor, Axiom, Loom, Sigma, Glimmer, Kodax, Pilot and Prism. Legacy prose-derived holder authorization remains temporary migration machinery only and is no longer required by any of these active Role continuations.

## Basis

- Axiom established `Assignment Modes` as the single machine-readable holder-assignment authority while keeping human-readable Holder State descriptive.
- Loom corrected ordinary Role authoring so immutable historical Parents that predate `Assignment Modes`, including Parents carrying identifier-only historical schema authority, can be continued truthfully without rewriting history or inferring a historical schema revision.
- The exact canonical active Role artifacts are:
  - Anchor: `.topics/roles/001-1-1-1-1-1-anchor-canonical-holder-cutover-role.trace.md`; SHA-256 `8302ced51dca642e4f2cc38e76344e0bc5583b988d17d472176d812813f917f3`.
  - Axiom: `.topics/roles/001-2-1-axiom-canonical-holder-cutover-role.trace.md`; SHA-256 `97d00ef1b7263f47703ae2875aba4f58c2f236b32b3fc508d2f4528eefbb0d01`.
  - Loom: `.topics/roles/001-3-1-loom-canonical-holder-cutover-role.trace.md`; SHA-256 `b6206c9d450c13f2eac24895567255f0afadbd9dc71685b29c668201c78c88ad`.
  - Sigma: `.topics/roles/001-4-1-sigma-canonical-holder-cutover-role.trace.md`; SHA-256 `0f5944dc3f0c4c21ea6f29318da92171dad5343b45b18a7a6b5dac59f386cebf`.
  - Glimmer: `.topics/roles/001-5-1-glimmer-canonical-holder-cutover-role.trace.md`; SHA-256 `f08a155596381ba8a8d4b7f3dda84a67f53f82c7b777ce8a0dd1312fd8035724`.
  - Kodax: `.topics/roles/001-6-1-kodax-canonical-holder-cutover-role.trace.md`; SHA-256 `1983edfcc64f136eee8ed3f40fac163b5fb4ecb57edba5068883f77f10db268e`.
  - Pilot: `.topics/roles/001-7-1-pilot-canonical-holder-cutover-role.trace.md`; SHA-256 `b6ff95c6edc9669ea8c41170a14847b9733bd83c1008d72a23484a2b8a89dd8f`.
  - Prism: `.topics/roles/001-8-1-1-prism-canonical-holder-cutover-role.trace.md`; SHA-256 `590880b05ee3915e8499ed0fbd7e7b7aaf3ab658c14ca98abfac73bf060767ae`.
- Anchor and Prism were re-authored from their exact active immutable historical Parents using the accepted identifier-only historical Parent rule; ordinary Tooling qualified both continuations without history rewrite or revision inference.
- Existing canonical continuations for Axiom, Loom, Sigma, Glimmer, Kodax and Pilot were already qualified under the same current Role contract.

## Consequences

- Current holder authorization must derive from direct canonical `Assignment Modes` on the active Role artifact.
- `Holder State` prose remains human-readable description and must not be parsed or matched to create authority.
- Exact legacy Role mappings may now be removed from active Core runtime behavior after Core verifies the complete canonical set and preserves historical artifacts as audit evidence only.
- Removal must also remove legacy-positive regression expectations; obsolete historical artifacts remain immutable evidence but are not accepted as current operational holder authority.
- No Role-name, repository-path, model-provider, chat-session or executor-specific compatibility branch may replace the legacy mapping.
- Historical carriers remain historical evidence. Reusing one as current work requires explicit migration/requalification rather than permanent runtime backward compatibility.

## Review Conditions

- Review only if a future holder-assignment mechanism cannot be represented generically by the canonical Role contract, or if a new active Role requires a genuinely new semantic assignment mode rather than a Tooling-specific exception.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-7-5-1-2-1-1-1-1-identifier-only-historical-role-parent-authoring-correction.trace.md](001-2-7-5-1-2-1-1-1-1-identifier-only-historical-role-parent-authoring-correction.trace.md)
  - Value: J6vISAbZ5HdMLrD25emWRHWNGgl6hlL9iZJV_IGMufg

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: dHaWh3GK2mRQvU1_9pweXc9uyGuRpyLtuF2Wfz604QU