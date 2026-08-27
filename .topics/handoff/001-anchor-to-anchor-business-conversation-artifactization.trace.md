# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Current
  - Current Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-08-26 16:30:00
  - Authors: Anchor
  - Why: Transfer an existing Tiinex/business conversation to another Anchor for durable artifactization without prescribing its conclusions or artifact shape.
  - Summary: Anchor-to-Anchor conversation artifactization in tiinex/business, with Sigma as an interaction participant and a Tooling-manufactured return Handoff package expected.
  - Status: active/local

---

# tiinex/business — Anchor Conversation Artifactization

## Handoff Parties

- Purpose: Artifactize the current conversation into the tiinex/business Workspace and return the resulting durable state through Tiinex Tooling.
- From: Anchor
- From Kind: role
- To: Anchor
- To Kind: role

## Transfers

- conversation-artifactization
  - Transfer Kind: work
  - Description: Use the conversation already present in this chat as the source material. Materialize the durable Tiinex artifacts warranted by that conversation into the carried tiinex/business Workspace, then create a return Handoff and manufacture a Handoff package for Anchor.
  - Boundary: Do not invent business facts or conclusions not supported by the conversation. Do not let this Handoff prescribe artifact count or artifact types; use Tiinex Tooling and the conversation itself to determine what warrants durable materialization.

## Required Context

- none

## Reference Context

- none

## Retained Responsibilities

- tooling-contract
  - Retained By: Anchor
  - Responsibility: retain responsibility for Tiinex Tooling and carrier-format evolution
  - Boundary: the receiving Anchor owns only the transferred conversation-artifactization work

## Exclusions And Dependencies

- no-seeded-business-outcome
  - Kind: excluded-scope
  - Description: the package intentionally carries no pre-authored business conclusions, artifact plan, expected artifact count, or expected artifact schema selection

- no-invented-role
  - Kind: excluded-scope
  - Description: the package identifies the recipient as Anchor and carries Sigma participation, but does not invent any additional Role or role-holder identity

- no-manual-carrier-construction
  - Kind: excluded-scope
  - Description: the return Handoff package must be manufactured by Tiinex Tooling rather than assembled manually

## Completion Expectation

- Signal Kind: return
- Signal Meaning: return the Tooling-manufactured Handoff package representing the artifactized tiinex/business Workspace
- Return To: Anchor

## Interpretation Limits

- Does Not Mean: the incoming Handoff determines the conversation's business conclusions or durable artifact taxonomy.
- Must Not Be Used To Claim: facts, decisions, commitments, new Roles, role-holder identity, or authority not supported by the existing conversation or qualified Tiinex material.
- Authority Limits: this Handoff transfers the artifactization task and completion route only.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:aj0P9_1olrr4pgPNmCzELGCZH9Mx5jtyHbxUBn0P7Lo
