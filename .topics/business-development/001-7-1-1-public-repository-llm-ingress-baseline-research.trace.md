# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-29 10:09:00
  - Trace: [Repository LLM Cold-Start And Bootstrap Surface](001-7-1-repository-llm-cold-start-and-bootstrap-surface-task.trace.md)
  - Origin:
    - [relative](001-7-1-repository-llm-cold-start-and-bootstrap-surface-task.trace.md)
- Current
  - Current Schema: [tiinex.discovery.research.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/discovery/research/tiinex.discovery.research.v1.schema.md)
  - Created At: 2026-08-29 10:09:00
  - Authors: Anchor; Sigma
  - Summary: Public Repository LLM Ingress Baseline
  - Status: draft/local

---

# Public Repository LLM Ingress Baseline

## Research Question

Can a blank LLM given any current public Tiinex repository discover a bounded and truthful path from first contact to Tiinex identity, repository role/status, canonical orientation, and the portable Tooling bootstrap without guessing hidden context or executing discovered code?

## Source Field

- In Scope: the seven current public Tiinex repositories (`.github`, `docs`, `site`, `ai-provenance`, `ai`, `ai-vscode-tools`, `business`); their root README/LLM/orientation/context surfaces; the current `site` refactor bootstrap Markdown/pointer; and the supplied current Business/Docs/Site snapshots.
- Out Of Scope: private repositories or accounts; proving behavior of every model provider; performing repository writes; judging product feature quality unrelated to ingress; executing code discovered in repository material.
- Freshness Boundary: observations are a 2026-08-29 baseline and must be re-resolved before being treated as later current state.

## Method

Perform a cold-reader simulation from each repository root. Prefer the ordinary first-contact surface a human or LLM is likely to see, then test whether it can reach stable Tiinex identity, repo-local context/status, current-vs-historical boundaries, and a portable bootstrap locator. Verify referenced files against the current public repository or supplied current snapshot. Treat `site/refactor` separately from the default `site/master` branch because current implementation and public/default branch authority are presently split. Do not infer missing files or execute repository code.

## Findings

- `Tiinex/.github` has strong `README.md`, `tiinex.orientation.v1.md`, `tiinex.context.v1.md`, and `tiinex.orientation.manifest.v1.json` identity surfaces, but no root `llms.txt` and no first-contact bootstrap locator.
- `Tiinex/docs` has a concise `llms.txt` router that points to README, orientation, context, schema orientation, and lineage policy. It does not currently route onward to the portable Tooling bootstrap.
- `Tiinex/site` default `master` has an LLM router with good identity/runtime cautions, but it does not expose the portable bootstrap as the first operational continuation.
- Current `Tiinex/site` `refactor` contains the actual portable bootstrap Markdown, pointer, CLI, and verifier, but its root `llms.txt` still points to pre-cleanup architecture/handover documents that are absent from the current refactor snapshot. The useful bootstrap exists but the current LLM front door does not lead to it.
- `Tiinex/ai-provenance` has a good bounded `llms.txt` status router and explicitly prevents stale runtime claims from becoming current, but it does not expose a bootstrap route.
- `Tiinex/ai`, `Tiinex/ai-vscode-tools`, and `Tiinex/business` have no root `llms.txt` baseline. `business` also lacks an ordinary root README/orientation surface, so a blank reader lands directly on `.topics` structure without project-level cold-start guidance.
- The current public bootstrap pointer already encodes strong safety semantics: `semanticAuthority: false`, host-mediated remote fetch only, no remote write, no source mutation, and no received-code execution. It names `discover-tooling`, `describe-checkpoint-gate`, `plan-host-action`, and `prepare-task` as first operations.
- The bootstrap pointer names repository and paths and tells readers to prefer an explicit commit/release, but the pointer itself does not pin a publication ref. A public first-contact router therefore still needs a qualified stable locator or release/checksum boundary rather than simply saying `use refactor`.
- No single current public convention makes all repositories converge on the same cold-start path. The components largely exist; discoverability and publication qualification are the main missing composition.

## Synthesis

The gap is primarily an ingress/projection gap, not a new Tiinex semantic-model gap. Tiinex already has stable organization identity, repo-specific LLM routers on several surfaces, and a safety-bounded portable bootstrap. The smallest coherent model is: every public repo exposes a very short machine/human route; that route delegates stable project identity to `Tiinex/.github`, declares only repo-local status/boundaries, and then points to one qualified portable-bootstrap locator. Business should own the acceptance requirement, while Tooling owns the bootstrap mechanics. A repository should be considered LLM-ambassador-ready only when a blank reader can explain Tiinex accurately and continue safely without hidden pre-prompt context. The model should be tested as a cold-start behavior before adding provider-specific files such as `AGENTS.md`, `CLAUDE.md`, or Copilot instructions; those are adapters only if evidence shows they materially improve discovery.

## Interpretation Limits

- This baseline does not prove how every LLM host chooses files automatically; `llms.txt` is useful but cannot be assumed universal.
- It does not qualify the current Site release or make `refactor` a stable public branch merely because the bootstrap source is present there.
- It does not prove the bootstrap package is publication-ready as a standalone downloadable release; only the current readable source/pointer and previously qualified handoff bootstrap behavior were inspected.
- Missing routers are discoverability findings, not evidence that a model could never infer Tiinex from other files.
- No public repository changes are authorized by this research artifact alone; the parent task and later Sigma acceptance own that work boundary.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Repository LLM Cold-Start And Bootstrap Surface](001-7-1-repository-llm-cold-start-and-bootstrap-surface-task.trace.md)
  - Value: MX41lwq2K34KbmJ6VhNhMd5h3qgm02oLfSR4XPaGy8w

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: z1Z2pZztsBcIQUT0QWPthuX9EmbnYOt-BtJ4cSUh--c
