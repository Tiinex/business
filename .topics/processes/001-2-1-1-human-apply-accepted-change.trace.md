# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.transition.definition.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/transition/definition/tiinex.transition.definition.v1.schema.md)
  - Created At: 2026-08-29 19:51:00
  - Trace: [Prepare Accepted Candidate](001-2-1-prepare-accepted-candidate.trace.md)
  - Origin:
    - [relative](001-2-1-prepare-accepted-candidate.trace.md)
- Current
  - Current Schema: [tiinex.transition.definition.v1](https://github.com/Tiinex/docs/blob/911d4cf990e35ce25a56e8f376d296e327c48260/.topics/.schemas/transition/definition/tiinex.transition.definition.v1.schema.md)
  - Created At: 2026-08-29 19:51:00
  - Authors: Anchor; Sigma
  - Why: Make today's human transfer responsibility visible without confusing today's copy/paste or Git mechanics with the durable higher-level process.
  - Summary: Apply the prepared accepted candidate to the intended target current state through the trustworthy mechanism currently available to the responsible human.
  - Status: proposed/local

---

# Human Apply Accepted Change

## Transition Identity

- Name: Human Apply Accepted Change
- Version: 1
- Canonical Identifier: tiinex.process.accepted-change-landing.human-apply-accepted-change.v1
- Transition Family: accepted-change-landing-process
- Human Label: Human Apply Accepted Change

## Purpose And Scope

- Purpose: Let the responsible human carry the prepared accepted candidate into the intended target current state using the currently available trustworthy mechanism.
- Semantic Boundary: The durable meaning is human-controlled application of an already accepted candidate. The current mechanism may include ChatGPT-produced source or a source package, copy/paste or equivalent manual file application, and Git commit/push when the target workflow requires them; those mechanics are replaceable.
- Intended Domains: current Tiinex work where direct artifact-aware landing Tooling is not yet sufficient for the responsible human to apply the accepted candidate without a manual bridge.
- Not Intended For: silently changing the accepted scope, skipping target verification, treating Git transport as acceptance, or making the human a permanent implementation middleware requirement.

## Input Roles

- prepared landing candidate
  - Meaning: the bounded accepted candidate prepared for the current landing mechanism
  - Minimum Count: 1
  - Maximum Count: 1
  - Acquisition Policy: invocation-provided
  - Target Kind: non-artifact

## Output Roles

- applied target state candidate
  - Meaning: the target state after the human has attempted to apply the prepared candidate, before landed-state verification
  - Minimum Count: 1
  - Maximum Count: 1
  - Target Kind: non-artifact

## Lifecycle And Continuity Effects

### Lifecycle Effects

- produce applied target state candidate
  - Target Binding: applied target state candidate
  - Effect: create-new
  - Logical Continuity: no-subject-effect

### Parent Effects

- none

## Relation Effects

- none

## Applicability And Conditions

- Applicability Meaning: applicable while the accepted change requires a human-controlled transfer/application bridge because the available Tooling does not yet own the full trustworthy landing action.
- Unknown Meaning: if target, candidate, authority, or safe application mechanism is unclear, the step remains unresolved rather than guessed or auto-applied.

## Authoring Bindings

- none

## Placement Intent

### Destination Bindings

- none

### Output Placements

- applied target state candidate
  - Output Binding: applied target state candidate
  - Placement Intent: no-materialization

## Interpretation Limits

- Does Not Prove: that the landed target matches the accepted candidate, that a commit/push occurred, that remote state is current, or that the higher-level outcome is complete.
- Must Not Be Inferred: that copy/paste, ChatGPT, a ZIP package, an IDE, or a particular Git UI is required by the durable process.
- Execution Boundary: the actual target repository/artifacts and their verification remain the authority after the human application attempt.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Prepare Accepted Candidate](001-2-1-prepare-accepted-candidate.trace.md)
  - Value: fHPOn_mdMFWkru0cb6xxm1GS5983uhxS_Ok4V8F087Y

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: X5KR12tB-DoCpAWcruafw2ZBXaxx-s1Ft7L3v_4doR8
