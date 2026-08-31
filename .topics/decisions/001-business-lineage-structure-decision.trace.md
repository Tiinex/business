# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.party.organization.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/party/organization/tiinex.party.organization.v1.schema.md)
  - Created At: 2026-08-26 14:55:00
  - Trace: [001-tiinex.trace.md](../001-tiinex.trace.md)
  - Origin:
    - [relative](../001-tiinex.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 15:04:00
  - Authors: Anchor
  - Summary: Business lineage structure
  - Status: accepted/local
  - Why: Preserve the current authoring convention that keeps organizational lineage readable and dimension-consistent across Tiinex Business.
- Repairs
  - Local dimension and recovery boundary clarification
    - Target: filename dimension scope and cross-repository Parent recovery
    - Note: Filename dimensions are local navigation projections and do not import an upstream repository's dimension path. Cross-source Parent continuity remains semantic and exact recovery follows truthful local or version-stable external routes without requiring duplicate Parent material.
    - Reason: First real cross-repository specialist lineages exposed that globalized filename dimensions and mandatory vendored relative recovery made local trees look truncated and coupled unrelated source layouts.
  - Major stability and leaf-projection clarification
    - Target: local filename dimension progression and current semantic leaves
    - Note: Serial work turns extend the existing local dimension path; Handoff/research/return boundaries do not allocate majors. New majors require explicit recoverable stability/re-anchor rationale, while real parallel branches may remain separately visible.
    - Reason: A cleanup pass incorrectly used majors as turn counters, producing many apparent discovery leaves even though declared Parent formed one serial lineage.

---

# Business Lineage Structure

## Decision

- State: accepted
- Subject: organizational lineage and filename discipline in tiinex/business
- Decision: `.topics/001-tiinex.trace.md` is the Tiinex organization root. Filename dimensions are local human navigation coordinates inside the directory/source surface where artifacts are authored; they project work shape but never replace declared `Parent` authority. A local semantic branch normally begins at major `001`. While work remains on the same local progression, direct descendants extend that local path one segment per Parent edge (`001` -> `001-1` -> `001-1-1`, ...). A role/session boundary, Handoff, research/discovery turn, implementation-evidence turn, or return Handoff does not by itself justify a new major. A new local major requires an explicit stability or re-anchor reason that a later reader can recover: for example an accepted/landed checkpoint before a materially new track, a deliberately established parallel stable branch, or practical path compression after a stable point when continued suffix growth has become unwieldy. If no such reason exists, authoring continues the existing dimension path. Starting a new local major does not reset semantic lineage: `Parent` may still point to the prior stable artifact or to an artifact in another source. Repository/source boundaries therefore preserve semantic Parent continuity but do not import the upstream repository's filename dimension coordinates. Collection directories such as `decisions/` do not add invented semantic dimension levels merely because they store artifacts. Schemas and explicitly non-organizational artifacts may retain their own authority roots.

## Basis

- A human contributor should be able to open current work locally and follow Parent upward when more context is needed.
- Path conventions alone are not enough to establish semantic ancestry.
- A local dimension-path filename lets a human infer nearby progression and stable checkpoints before opening an artifact, while `Parent` remains the exact cross-source semantic authority.
- Git history preserves superseded current states, so current artifacts may be corrected without fabricating historical Parent facts.

## Consequences

- Roles, Initiatives, Financing, Funds, and other real subject branches use explicit local anchors. Descendants on one active branch normally extend the current local dimension path one segment per Parent edge. A major must not be used as a turn counter. Multiple genuinely parallel current branches may be represented separately when the divergence is real and explicit, but serial Handoff/research/return steps remain one lineage until an explicit stable re-anchor is declared.
- Tiinex is the Organization root; concrete Projects, Roles, funds, and work packages use their appropriate schemas.
- Business remains a manager-readable organizational surface; detailed implementation Tasks live in their natural repository while retaining truthful upward organizational context.
- Specialist Discoveries, implementation Tasks, verification evidence, and role development lineages normally live in the repository whose domain they inspect or change. Business retains the organizational why, priority, acceptance boundary, and concise cross-repository disposition rather than mirroring technical detail.
- Handoff/package carrier lineage is coordination and consumer-facing progress/recovery projection, not permanent work ancestry. When no prior carrier major is known, a new exported carrier may begin at `001`; Tooling does not need global carrier history merely to allocate that convenience root. Continuation suffixes may expose turns/retries/divergence, while a new carrier major marks an explicit stable transport checkpoint. Carrier dimensions never replace artifact Parent lineage or need to mirror source-artifact filename dimensions. Transport-only artifacts should remain package-local unless their coordination meaning itself warrants durable source provenance.
- Cross-repository specialist work retains its real organizational `Parent` when that ancestry is known; repository boundaries must not silently restart semantic lineage. Filename dimensions remain local to the child repository/directory and do not copy the external Parent's local coordinate path. Recovery follows the Parent representation that is truthfully available: directly materialized same-source Parents use `relative`; an external or otherwise non-local Parent uses a qualified version-stable recovery locator such as a commit-pinned `browse + git` representation when available. A child repository must not vendor duplicate Parent bytes solely to manufacture relative locality. Viewer/Tooling should recover the external Parent as a distinct source boundary so the source change appears as a scope transition. If exact Parent identity or a truthful recovery route is genuinely unavailable, fail closed rather than fabricating an edge.
- New collection folders are not semantic parents by default, and no semantic branch should be created only as empty taxonomy.
- Current HEAD is a curated current-truth surface, not a status archive. Leaf-first discovery makes filename projection operationally visible: every semantic leaf that remains should represent a current frontier or an intentionally active parallel branch. Serial completed Handoff/research/return steps should normally remain ancestors in their real lineage rather than being projected as artificial sibling/major leaves. Git preserves superseded history.
- `business-development/` is the Business repository active workbench. While a Role is actively changing Business, that Role has at most one active development lineage there; deeper descendants may continue the same work, but parallel sibling lineages must not become a substitute for prioritization. Completed workbench lineage leaves current HEAD after its outcome is landed and local role-level checks are complete, with Git retaining history.
- Presence or absence of an active development leaf is a current-work signal, not a universal completion/acceptance rule. A bounded Follow may use that signal in context, but acceptance remains owned by the relevant Epic/gate and its tests.
- The same active-workbench behavior is intended for other Tiinex repositories. The exact folder name is not yet locked cross-repository: current portable Tooling still treats `.topics/development` as specially quarantined legacy material during broad reads, so that path must be reconciled before it is adopted as the normal current-work surface elsewhere.
- Process metrics such as acceptance/rework loops should later be derived from real provenance/history when the Process model is designed; no KPI/status schema is introduced here merely because the history could support one.

## Review Conditions

- Review if Tiinex gains an explicit branch-anchor schema or another declared authority that supersedes this local anchor convention.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-tiinex.trace.md](../001-tiinex.trace.md)
  - Value: p4YGHsMqWThhcRwqAOWh1RznaqBKd_pndsSvDXyZycQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: B3OuFOgxMy_nnM5ts47ZFvrEKLLITc6g1QxsFjc5Lnc
