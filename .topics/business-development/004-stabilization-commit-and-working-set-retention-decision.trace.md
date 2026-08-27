# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.discovery.research.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/discovery/research/tiinex.discovery.research.v1.schema.md)
  - Created At: 2026-08-26 22:36:00
  - Trace: [Current Repository Frontier And Portfolio Synthesis](003-current-repository-frontier-and-portfolio-synthesis-research.trace.md)
  - Origin:
    - [relative](003-current-repository-frontier-and-portfolio-synthesis-research.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 23:10:00
  - Authors: Anchor; Sigma
  - Why: Define the durability and review point for the current Business Development repair tranche before Sigma commits or publishes repository state, and separate semantic stabilization from later working-set reduction.
  - Summary: Tiinex Business should pass semantic repair, Tooling qualification, Anchor graph review, and repository audit before the first stabilization commit; cleanup of recoverable historical/materialized working-set artifacts follows in a separate post-commit round.
  - Status: accepted/local

---

# Stabilization Commit And Working-Set Retention Decision

## Decision

- State: accepted
- Subject: quality gate for the current Tiinex Business Development tranche, repository durability, and later working-set reduction
- Decision: do not treat the current local Business portfolio as ready for the first stabilization commit/merge until the Axiom semantic repair round has dispositioned local Parent/Origin truth, Project/Task association, Practitioner specialization, role versioning, Handoff closure hygiene, and related schema gaps; any required Loom Tooling changes have been implemented and qualified; and Anchor has repaired the Business artifact graph and completed a final Discovery/audit review. Once that coherent state exists, Sigma may create the real Git durability checkpoint. Perform working-set reduction only after that checkpoint proves the relevant predecessor material is recoverable through immutable adapter-backed provenance and historical references remain resolvable.

## Basis

- Current Business artifacts are local/carried and must not be assumed to exist in Git history before a real commit or published adapter state exists.
- The current epic Tasks expose a real lineage gap: truthful Project ancestry is blocked by Root Parent-Origin rules for unpublished local artifacts, and visually or structurally tidy ancestry must not be fabricated.
- The current `.topics/.cache` material is predecessor-Handoff closure residue rather than intended Business domain structure, but deleting it before historical references are recoverable would trade clutter for broken provenance.
- Role evolution is intended to preserve immutable/recoverable predecessor versions while allowing the active workspace to retain primarily current leaves after durable source recovery is established.
- Separating stabilization from cleanup gives one reviewable semantic checkpoint before reducing the working set and makes rollback/recovery straightforward.

## Consequences

- Axiom receives the semantic-gap tranche first and returns a bounded disposition to Anchor.
- Loom receives implementation work only where Axiom or direct Tooling evidence demonstrates an implementation gap, and must qualify the changed behavior through Tiinex Tooling rather than hidden native-only assumptions.
- Anchor performs the consolidation pass after semantic/tooling returns: repair truthful Parent lineages, role-version/specialization representation, Business Development continuity, and Handoff routing; then run Discovery, validation, package/context audit, and regression checks.
- Sigma is the human decision point for the actual Git commit/push/merge. This Decision does not claim that any repository mutation has occurred.
- After the stabilization commit, a separate cleanup tranche may remove superseded current-workspace copies, legacy closure material such as `.topics/.cache`, or predecessor Role material only when commit-pinned or equivalent adapter-backed recovery remains demonstrably available and no historical reference is silently broken.
- Roadmap authoring remains after the epic/lineage repair view is coherent; reusable Process semantics remain last and should be abstracted from real repeated work.

## Review Conditions

Reopen this decision if the selected adapter cannot provide immutable predecessor recovery, if the semantic repair shows that cleanup must precede a safe commit, if Git is no longer the current durability adapter, or if Sigma deliberately chooses a smaller explicit checkpoint with preserved recovery guarantees.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Current Repository Frontier And Portfolio Synthesis](003-current-repository-frontier-and-portfolio-synthesis-research.trace.md)
  - Value: g43lAHYeTSRqKNRLYPqroqojvU3x7bYYzWT8eUVbjKw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:Y5O2Atvv_EmxJr6l-rPfDRqyBGQFMkOeQlasXtHzE4M
