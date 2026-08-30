# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-30 18:20:00
  - Trace: [Product Use Cases](001-use-cases.trace.md)
  - Origin:
    - [relative](001-use-cases.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-30 18:21:00
  - Authors: Anchor; Sigma
  - Why: Preserve a concrete problem-first scenario where Tiinex's shared human/LLM representation can be evaluated without leading with lineage or provenance terminology.
  - Summary: Product use-case hypothesis for client or organizational memory where humans and LLMs can understand what is happening, why it is happening, what still applies, and how current work connects to prior decisions and sources.
  - Status: proposed/local

---

# Client Organizational Memory

A company, consultancy, team, or other organization may need to work across several clients or internal domains whose goals, terminology, people, decisions, history, current work, and superseded context must remain distinguishable. The problem is not merely finding a document with similar words; it is helping a new human or LLM orient in the relevant organization's current structure without requiring someone to retell the whole context in every session.

## Current Read

A useful Tiinex representation could make questions such as **“Why are we building this?”** answerable through explicit current artifacts and their provenance rather than through chat memory or document similarity alone.

A human or LLM should be able to move from the current work toward the organizational reason for it, see decisions that changed direction, distinguish current from historical or superseded material, and inspect the sources that support the current read.

One illustrative lineage shape is:

`Client → Strategy → Initiative → Project → Decision → Implementation → Result`

This is an example for comprehension, not a mandatory Tiinex hierarchy. Real organizations may use different artifact types, relations, branch shapes, and scope transitions.

## Design Direction

Present the recognizable problem before introducing Tiinex mechanisms. A concise first-contact formulation to test is:

> Tiinex is a way to describe an organization so humans and AI can understand what is happening, why it is happening, and how things connect.

A practical onboarding explanation can then show the desired answer shape:

- here is the current work;
- here is the initiative or purpose it belongs to;
- here is the problem or decision that explains why it exists;
- here are changes that altered direction;
- here is what still applies versus what is historical or superseded;
- here are the sources and provenance that let the reader check the answer.

Feed, Tree, Lineage, Atlas, Tooling, and LLM ingress are possible projections or access paths over that truth. None of them is the use-case itself, and the use-case must survive a future change in presentation technology.

## Boundaries And Non-Claims

- This artifact is a product-use hypothesis and explanation target, not evidence of customer demand, willingness to pay, adoption, market size, competitive advantage, or production readiness.
- Tiinex is not claimed here to replace search, RAG, document stores, project-management systems, chat systems, or human judgment. The distinguishing hypothesis is that explicit currentness, provenance, authority boundaries, and relationship structure can improve orientation when those properties matter.
- The example does not establish a universal client ontology or require every organization to model Strategy, Initiative, Project, Decision, Implementation, and Result in that exact order.
- Human and LLM access should remain semantically comparable: a Viewer may make relationships easier for a person to see, while Tooling may expose them differently to an LLM, but neither side should gain unsupported semantic truth unavailable to the other.

## Next Artifacts

- Glimmer-role Discovery testing whether a new user can understand this use-case before learning internal Tiinex terminology.
- Later real-user observations or feedback may support, refine, split, or reject this hypothesis without rewriting the original evidence boundary.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Product Use Cases](001-use-cases.trace.md)
  - Value: CG5-37pyBAATVTWlOvAL3ua8wlYFl-JrAH3e52d0n7Y

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:GGJfS52dMUIkqlbzzVsllF-u3HP4cFf3KWJI-APtyGQ
