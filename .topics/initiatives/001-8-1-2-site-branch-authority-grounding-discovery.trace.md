# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/4cb7046454f1cf75333097fc1a3d4562838afc26/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/4cb7046454f1cf75333097fc1a3d4562838afc26/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-29 10:09:00
  - Trace: [Repository LLM Cold-Start And Bootstrap Surface](001-8-1-repository-llm-cold-start-and-bootstrap-surface-task.trace.md)
  - Origin:
    - [relative](001-8-1-repository-llm-cold-start-and-bootstrap-surface-task.trace.md)
- Current
  - Current Schema: [tiinex.discovery.v1](https://github.com/Tiinex/docs/blob/4cb7046454f1cf75333097fc1a3d4562838afc26/.topics/.schemas/discovery/tiinex.discovery.v1.schema.md)
  - Created At: 2026-09-02 02:48:00
  - Authors: Anchor; Sigma
  - Why: A real cold recipient treated the conventional `master` name as stronger current authority than the repository actually assigns it, exposing a first-contact grounding gap before Viewer parity work.
  - Summary: Site Branch Authority Grounding Discovery
  - Status: accepted/local

---

# Site Branch Authority Grounding Discovery

## Discovery Intent

- Intent: establish the smallest explicit repository-facing authority boundary needed so a cold human or LLM does not have to infer current-versus-PoC meaning from Git branch naming conventions.
- Starting Question: which current `Tiinex/site` branches are implementation authority versus historical PoC evidence, and where must that distinction be projected for cold readers?

## Discovery Field

- Field: current public `Tiinex/site` branch heads, current `refactor` README/`llms.txt`, the Viewer parity evidence, and the observed grounding failure during Foundation work.
- In Scope: branch role, current-versus-historical implementation authority, PoC evidence role, first-contact projection, and downstream parity interpretation.
- Out Of Scope: changing canonical schema semantics, renaming branches, changing Git default-branch configuration, claiming a public release, implementing Viewer parity, or optimizing the CLI itself.
- Freshness Boundary: branch observations verified 2026-09-02 before this Discovery was authored.

## Discovery Method

- Method: inspect the actual public branch heads and compare `master` with `poc-monolith`; inspect current `refactor` first-contact text; reconcile those facts with the human-supplied repository history and the parity task boundary.
- Evidence Approach: branch names are locators only. Current implementation authority must come from explicit maintained project guidance and accepted operating context, not from a convention such as assuming `master` means current.

## Discovery Outcome

- Outcome: bounded first-contact grounding defect confirmed; no new semantic schema is required.
- `master`: PoC evidence at observed head `6691491f0450f115ecf806342afec86b3c6a4df4`.
- `poc-monolith`: PoC evidence at observed head `b10abe25e2da65e4f91e1bae68a4da41ea10fa3f`; it is one commit ahead of the observed `master` head and that comparison changes only `.gitignore` by adding `.old` handling.
- `refactor`: current active implementation at observed head `5d472b1b1f3a926db1b4034b01961be10d7af1e6`.
- Current Site README and `llms.txt` correctly describe the repository as the current Viewer/reference/shared Tooling source when read on `refactor`, but they do not explicitly tell a cold reader that `master` and `poc-monolith` are PoC evidence while `refactor` is the active implementation.
- The practical failure mode was reproduced socially: a grounded recipient began treating `master` as the likely current product baseline until Sigma supplied the missing branch meaning.
- Required projection repair: `refactor` first-contact surfaces should state the three branch roles compactly and warn readers not to infer implementation authority from the default/conventional branch name.
- Viewer parity repair: parity discovery must explicitly compare PoC evidence (`master` + `poc-monolith`) to the active `refactor` target rather than allowing the refactor ledger to define its own baseline.
- Tooling implication: normal Tooling/source inspection should expose requested/configured ref and current/historical purpose when that purpose is explicitly declared; this Discovery does not authorize Tooling to guess branch purpose from branch names.
- Axiom disposition: no schema-semantic reconciliation is currently demonstrated. The defect is repository grounding/projection plus later Tooling ergonomics, so Axiom remains unopened.

## Next Artifact

- One bounded Site-local grounding Task should update the current first-contact branch-role projection and preserve an evidence-honest current/PоC boundary before the common CLI ergonomics tranche begins.

## Interpretation Limits

- This Discovery does not make branch names universal Tiinex semantics, prove that `refactor` should remain current forever, make `master` disposable, or claim `poc-monolith` differs from `master` only in all historical senses beyond the exact observed comparison. A later explicit repository decision may change branch roles; first-contact projections must then change with it.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/4cb7046454f1cf75333097fc1a3d4562838afc26/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Repository LLM Cold-Start And Bootstrap Surface](001-8-1-repository-llm-cold-start-and-bootstrap-surface-task.trace.md)
  - Value: W9ilLnXyCbsYd4_wCczszY87LLtPjEgULC5tmjA_Ikk

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/4cb7046454f1cf75333097fc1a3d4562838afc26/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:VSW11faSGHjpEXIRP0F2HpyZgq5DDuym44aUIxXFRpc
