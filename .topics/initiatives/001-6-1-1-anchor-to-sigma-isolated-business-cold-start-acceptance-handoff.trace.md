# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-29 10:32:00
  - Trace: [Business Repository-Only Cold-Start Acceptance](001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
  - Origin:
    - [relative](001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-02 00:05:00
  - Authors: Anchor
  - Why: Give Sigma one precise operator handoff for the genuinely isolated Business repository-only cold-start acceptance without leaking Handoff, Tooling, Docs, Site, or prior Tiinex context into the model being tested.
  - Summary: Anchor To Sigma — Isolated Business Repository-Only Cold-Start Acceptance
  - Status: ready/local

---

# Isolated Business Repository-Only Cold-Start Acceptance — Anchor To Sigma

## Handoff Parties

- Purpose: run the final human-controlled isolated cold-start test for Business semantic self-sufficiency while preserving the test boundary that the model under test receives only the Business repository and no Tiinex continuation machinery
- From: Anchor
- From Kind: role
- From Reference: [Anchor Role](../roles/001-1-anchor-role.trace.md)
- To: Sigma
- To Kind: role
- To Reference: [Sigma Role](../roles/001-4-sigma-role.trace.md)

## Transfers

- prepare-isolated-test-project
  - Transfer Kind: work-and-responsibility
  - Description: create a completely fresh isolated project or chat with no Tiinex instructions, no prior Tiinex conversation, no Anchor/Glimmer role prompt, no uploaded Docs or Site material, and no Tooling bootstrap; the Handoff Package carrying this instruction is for Sigma as test operator and MUST NOT be supplied to the model under test
  - Controlling Artifact: [Business Repository-Only Cold-Start Acceptance](001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
  - Boundary: the tested model receives only a materialized copy of the carried current Business Workspace source; giving it this Handoff Package, its Start/Continue route, Docs, Site, or role pre-context invalidates the test

- run-natural-first-contact
  - Transfer Kind: work-and-responsibility
  - Description: give the isolated model the Business repository only and ask one ordinary open first-contact question requesting its own explanation of what the project is, what problem it addresses, what is currently true, what remains uncertain, and what appears to be the current priority; do not tell it the expected answers or that it is being evaluated until after the test
  - Controlling Artifact: [Business Repository-Only Cold-Start Acceptance](001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
  - Boundary: wording parity with Anchor is not required; the important test is truthful recovery of Business authority, boundaries, current-versus-unknown distinctions, and priorities without invented certainty

- probe-novel-organizational-questions
  - Transfer Kind: work-and-responsibility
  - Description: after the first answer, ask two or three natural follow-up questions that were not pre-scripted into the repository, including at least one question where the truthful answer may be unknown or bounded; do not correct the model between questions
  - Controlling Artifact: [Business Repository-Only Cold-Start Acceptance](001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
  - Boundary: this is a semantic cold-start test, not Tooling execution, repository mutation, implementation debugging, or a test of whether the model can resume this Anchor session

- return-sigma-observation
  - Transfer Kind: responsibility
  - Description: return the isolated model's first answer, the follow-up questions and answers, and Sigma's compact human observation of what was clear, confusing, or wrong so Anchor can dispose the Business cold-start gate without reconstructing the test from memory
  - Controlling Artifact: [Business Repository-Only Cold-Start Acceptance](001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
  - Boundary: Sigma observation is human acceptance evidence; the isolated model's confidence or fluency is not itself proof of correctness

## Required Context

- business-cold-start-task
  - Material: Business Repository-Only Cold-Start Acceptance
  - Material Reference: [Business Repository-Only Cold-Start Acceptance](001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
  - Purpose: controlling Done criteria and the explicit separation between repository-only semantic cold start, operational bootstrap, and Handoff continuation
  - Availability: available

- foundation-readiness
  - Material: Foundation Readiness And Operating Reconciliation
  - Material Reference: [Foundation Readiness And Operating Reconciliation](001-6-foundation-readiness-operating-reconciliation-task.trace.md)
  - Purpose: organizational Foundation boundary and the reason this isolated human test gates broader expansion
  - Availability: available

- sigma-role
  - Material: current Sigma Role
  - Material Reference: [Sigma Role](../roles/001-4-sigma-role.trace.md)
  - Purpose: human observation and acceptance boundary for the isolated quality test
  - Availability: available

## Reference Context

- current-business-workspace
  - Material: complete current Business Workspace carried in this Handoff Package
  - Purpose: source bytes Sigma must materialize and provide alone to the isolated model; the model under test must not receive the rest of this package
  - Availability: available

## Retained Responsibilities

- acceptance-disposition
  - Retained By: Anchor
  - Responsibility: compare Sigma's returned observations against the controlling Business Done criteria, decide whether the repository-only cold-start gate passes or needs a Business authority/projection repair, and preserve the result durably

- test-environment-control
  - Retained By: Sigma
  - Responsibility: keep the tested project genuinely isolated, withhold this Handoff Package and all non-Business Tiinex context from the tested model, and report any accidental contamination rather than treating the run as valid

## Exclusions And Dependencies

- handoff-to-tested-model
  - Kind: excluded-scope
  - Description: do not upload or expose this Handoff Package, its bootstrap, Start/Continue route, Role pointers, Docs Workspace, or Site Workspace to the isolated model being evaluated

- coaching-the-answer
  - Kind: excluded-scope
  - Description: do not supply expected Tiinex definitions, Foundation status, role meanings, financing facts, or a grading rubric to the isolated model before it answers

- tooling-execution
  - Kind: excluded-scope
  - Description: Tooling bootstrap, package qualification, repository mutation, Site runtime, implementation work, and specific prior-session continuation are not part of this Business semantic cold-start acceptance

- hidden-certainty
  - Kind: excluded-scope
  - Description: do not accept invented legal-company status, employees/headcount, budget/runway, production readiness, commercial positioning, roadmap, or schema/runtime completeness when the Business repository does not establish them

## Completion Expectation

- Signal Kind: result
- Signal Meaning: Sigma returns one compact isolated-test observation containing the model's first-contact explanation, two or three natural follow-up exchanges, and Sigma's clear/confusing/wrong assessment; the run is explicitly marked invalid if the tested model received anything beyond the current Business repository and ordinary user questions
- Return To: Anchor
- Return To Reference: [Anchor Role](../roles/001-1-anchor-role.trace.md)

## Interpretation Limits

- Does Not Mean: receiving this Handoff Package makes the Business repository-only test pass, the tested model may use Handoff or Tooling, fluency proves semantic correctness, one scripted answer proves novel-question robustness, or Sigma must inspect implementation details
- Must Not Be Used To Claim: Business semantic self-sufficiency if the tested model received this carrier or other Tiinex context; Tooling readiness; Site runtime readiness; production readiness; final Foundation acceptance; or authority to commit/push any resulting local test material
- Authority Limits: this Handoff controls Sigma's test-operation boundary only; the Business repository remains the sole semantic input to the isolated model under test, Sigma owns human observation, and Anchor owns the later Foundation disposition

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Business Repository-Only Cold-Start Acceptance](001-6-1-business-repository-only-cold-start-acceptance-task.trace.md)
  - Value: jMnkDwuaxJa8HCxHGFjWlyBw-LqBTSuzSDHOqTEZdXw

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:lOWMbMGY0IemT2t_kSG0MD3_6reM4LYlnWKQ7au4ff8
