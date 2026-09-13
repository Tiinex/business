# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-12 21:29:17
  - Trace: [012-1-anchor-full-recovery-grounding-major-001-integrated.trace.md](../../initiatives/refactor/orchestration/handoffs/012-1-anchor-full-recovery-grounding-major-001-integrated.trace.md)
  - Origin:
    - [relative](../../initiatives/refactor/orchestration/handoffs/012-1-anchor-full-recovery-grounding-major-001-integrated.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-12 22:01:03
  - Authors: Anchor
  - Why: Current recovery carries over one hundred Handoff leaves; historical terminal material is making fresh grounding more expensive and ambiguous even though the underlying lineage is largely healthy.
  - Summary: Classify and reduce historical lineage noise across the full Tiinex program while preserving current obligations and recoverability.
  - Status: ready/local

---

# Reduction Major 001 — Current Frontier And Historical Leaf Reduction

## Objective

Reduce lineage noise across the current Tiinex program without deleting history or inventing lifecycle semantics, so a fresh Anchor can recover the active program frontier cheaply and distinguish active, blocked, human-gate, completed, superseded and historical terminal material from genuinely actionable leaves.

## Current Evidence

- Cross-workspace lineage audit found 113 real Handoff leaves across the current 16-Workspace recovery, concentrated in Site (30), Business (28), Verse Playthings (24), VS Code (12), Core (8) and Docs (7).
- Leaf count is not equivalent to stale work, but this density materially increases grounding synthesis cost and ambiguity over what is current.
- Most repositories remain structurally connected to Business organization/program context, while historical terminal returns and human gates remain visible as leaves.
- Docs currently has two integrity-mismatch findings from the lineage audit; do not destructively reduce affected Docs material until semantic/integrity ownership has classified them.

## Done Criteria

- Build an exact current leaf inventory over the carried Workspaces and classify each relevant leaf using qualified evidence, not filename age or intuition.
- At minimum distinguish: active/current, waiting/blocked, human gate, completed/accepted terminal, superseded historical, fixture/test-only, genuinely orphaned/unresolved.
- Prioritize the highest-density surfaces first: Site, Business, Verse Playthings and Extension VS Code; cover the remaining Workspaces sufficiently to produce a project-wide current-frontier projection.
- Use canonical `tiinex.reduction.v1` semantics for any durable reduction event: explicit Source Context, Carry-Forward State, Loss And Uncertainty, Validation, and deterministic navigation back toward fuller source.
- Treat ordinary Reduction and destructive-lineage eligibility as separate contracts. No physical deletion/removal is allowed unless the exact candidate set separately qualifies `eligible` under the maintained destructive-lineage method and another authority surface actually authorizes mutation.
- Preserve all still-operative obligations, open Tasks, human gates, blockers, cross-repository Parents and recovery evidence needed to continue work.
- Produce a compact durable current-program carry-forward surface that future Anchors can use without scanning dozens of historical terminal leaves.
- Where classification depends on canonical semantics, integrity interpretation or Tooling capability outside Anchor authority, route a bounded finding to Axiom or Loom rather than guessing.
- Do not make a repository look cleaner merely by hiding unresolved work; unresolved remains visible.

## Scope

Cross-repository lineage/readability reduction and current-frontier projection over the exact 16 Workspaces carried by the current master Recovery. This Major may author qualified Reduction/Decision/Feedback/Handoff artifacts and may route bounded semantic/Tooling follow-ups; it does not authorize product/source-code implementation changes.

## Dependencies

- Current full Master Recovery and all 16 qualified Workspace snapshots.
- Canonical `tiinex.reduction.v1` and `tiinex-reduction-destructive-lineage-eligibility-v1` semantics from Docs.
- Qualified currentness/operative-state evidence for any material proposed as terminal/superseded.
- Exact immutable source/Parent closure for any future destructive candidate set.

## Exclusions

- No cleanup by age, filename, path depth, chat history length or visual aesthetics alone.
- No destructive apply, deletion, remote mutation, commit, push, release or publication.
- No redefinition of Task/Handoff lifecycle, Parent semantics, currentness or Reduction semantics by Anchor.
- No assumption that every Handoff leaf is stale or that every old nonterminal artifact remains active forever.

## Near-Term Gate

Return to Master Anchor with: a project-wide leaf classification, qualified Reduction artifacts for clearly terminal historical clusters where useful, explicit unresolved/blocked leaves, before/after current-frontier readability metrics, and bounded owner-routed follow-ups. Keep any destructive candidate set separate and fail closed unless every eligibility input is exact and qualified.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [012-1-anchor-full-recovery-grounding-major-001-integrated.trace.md](../../initiatives/refactor/orchestration/handoffs/012-1-anchor-full-recovery-grounding-major-001-integrated.trace.md)
  - Value: IrRUMV4k_5NXbs0E08i1yTExruoTVZzYJdx1KFdHYEk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: --QLlB6rz_n_5AhdaG17iLwXBEE09ZzbcJfSyEM1v-E