# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-29 16:07:00
  - Trace: [Processes](001-processes.trace.md)
  - Origin:
    - [relative](001-processes.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-06 15:35:00
  - Authors: Anchor; Sigma
  - Why: Make bounded work that must cross a human-operated external execution boundary reproducible without turning the human into hidden context carriage or the execution role into owner of the originating problem.
  - Summary: Generic Pilot-mediated external execution process, evidence contract, output-lineage placement, return boundary, and stable-output promotion rule.
  - Status: accepted/local

---

# Human-Mediated External Execution Process

## Applicability

Use this process when a Tiinex role can specify a bounded action but the actual action must occur in an external model, application, service, device, local environment, or other context that is operated by a human rather than directly available to the originating role. Pilot is the reusable execution-boundary role; the origin/review role retains the originating problem and acceptance authority unless explicitly transferred.

## Bounded Execution Request Contract

The controlling Task or Handoff should identify, as applicable:

- origin lineage and declared return role;
- bounded objective and explicit non-objectives;
- ordered execution materials and the authority/function of each material;
- exact human-visible input or procedural steps, plus whether adaptation is allowed;
- expected result artifact, receipt, observation, or completion signal;
- evidence requirements, byte-preservation requirement, retry policy, and blocked-return behavior;
- responsibilities retained by the originating/review role and by the human executor.

The human should not have to reconstruct missing intent from chat history. If the request cannot make the human action decision-minimal without guessing materially, Pilot returns blocked rather than inventing scope.

## Execution Turn

1. **Prepare** — Pilot grounds from the controlling lineage, verifies ordered materials where identity checks are available, and projects the smallest faithful human execution surface.
2. **Guide** — Pilot tells the human exactly what to use, in what order, and what to submit/do. While execution is pending, unrelated analysis and redesign are out of scope.
3. **Receive** — Pilot captures what actually came back. Exact bytes are preserved when exposed; previews/descriptions are explicitly distinguished from exact source.
4. **Report** — Pilot records actual human-visible input, attachment/material identities, result identity, failures, deviations, preservation limits, and unresolved provider/host behavior.
5. **Return** — Pilot immediately authors or manufactures the lineage-correct Evidence and return Handoff when the bounded execution succeeds or becomes blocked. It does not continue the originating work.

## Fidelity Boundary

Exact human-visible execution input and provider-internal execution are different evidence layers. Pilot may prove which text/material it presented to the human and which bytes came back. It must not claim unseen provider-side prompt compilation, hidden preprocessing, or byte-for-byte prompt forwarding. Observable rewriting or substitution is recorded as an anomaly for the return role; it is not silently normalized into PASS.

## Evidence And File-Lineage Contract

- Active execution artifacts belong to the execution/evidence lifetime, not automatically to stable product/reference storage.
- When materialized in repository source, transient files should share the directory and lineage stem of the artifact describing the moment. A lineage such as '001-1-1-1-evidence.trace.md' may carry '001-1-1-1-generated-01.png', '001-1-1-1-execution-request.md', and '001-1-1-1-review-01.webp'. File extensions remain native; a binary output is not disguised as a Trace artifact.
- Exact source bytes and deterministic derivatives are separate identities. Hash both when material.
- Rejected/transient attempts may remain package/workspace evidence while the lineage is active, but they are not promoted into stable domain asset directories merely because they were generated.
- After explicit review/acceptance or another stable-domain disposition, the owning role promotes the selected source or deterministic derivative outside .topics into the natural domain location. The stable asset preserves the originating lineage stem where practical and the durable Evidence records the stable path plus immutable hash.
- Reduction is allowed only after the relevant work is durably landed and recovery/audit paths are preserved. Reduction summarizes superseded attempts rather than treating every generated byte as permanent current source.

## Review And Acceptance Boundary

Pilot verifies execution/transport facts, not originating semantic success. Technical, visual, product, schema, implementation, or human acceptance remains with the role/human named by the controlling work. A successful external action is not automatically successful product work.

## Reproducibility Minimum

A replayable bounded execution should be reconstructible from durable material without hidden chat context: controlling lineage, ordered material identities, exact human-visible instruction, expected return, actual returned identity, anomalies, and return Handoff. Tool-assisted domains may additionally carry deterministic postprocess/review manifests.

## Interpretation Limits

- Does Not Mean: every external action requires Pilot; Pilot becomes a universal remote operator; human execution grants remote-system authority; or exact user-visible text proves provider-internal prompt equivalence.
- Must Not Be Used To Claim: acceptance merely because execution returned, permission to retain every transient output forever, or authority to place unstable generated attempts in stable asset directories.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Processes](001-processes.trace.md)
  - Value: -dIbKFmhRYlDVjL-4TkCoeb6KCK-5wH6l4U8zsPgj8s

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: GeoEGgWDREbAm7xuoPXC6OCqTRhYEJ4mc0veH32X0ho
