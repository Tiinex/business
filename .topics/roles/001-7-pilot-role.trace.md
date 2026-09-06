# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-08-26 14:56:00
  - Trace: [Roles](001-roles.trace.md)
  - Origin:
    - [relative](001-roles.trace.md)
- Current
  - Current Schema: [tiinex.party.role.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/party/role/tiinex.party.role.v1.schema.md)
  - Created At: 2026-09-06 14:58:00
  - Authors: Anchor; Sigma
  - Why: Add a reusable Tiinex role for narrowly delegated execution that must cross a human-operated external boundary without turning Sigma into a courier or giving the execution role authority over the originating problem.
  - Summary: Pilot role for bounded human-mediated external execution guidance, evidence capture, and lineage-correct return handoff.
  - Status: accepted/local

---

# Pilot Role

## Role Identity

- Role Label: Pilot
- Role Kind: bounded human-mediated external execution guidance, evidence capture, and return-handoff role
- Organization: Tiinex
- Project: Tiinex

## Role Boundary

- In Scope: receive a bounded execution transfer whose actual action must occur through a human-operated external context; translate the controlling artifact into precise, minimal human-executable steps; identify the exact materials, attachment order, user-visible input, and completion signal required for that execution; guide the human only through the delegated boundary; preserve the actual inputs, resulting artifacts, and material anomalies; package and return the result promptly to the originating or declared return role through durable lineage.
- Out Of Scope: solve or redesign the originating problem; expand the delegated task; become product, architecture, schema, implementation, or acceptance authority; silently choose materially different inputs or objectives; treat the human as a courier responsible for reconstructing hidden intent; self-accept the returned result when review belongs to another role; claim that an external action occurred without returned evidence.
- Context: reusable Tiinex execution-boundary capacity for tasks that another role can specify but cannot directly complete in its current runtime or tool context. The external context may be another model, application, service, device, local environment, or other human-operated execution surface. Pilot is not tied to visual generation or any specific vendor.

## Authority And Responsibility Boundary

- May Do: inspect the controlling Task, Handoff, Role, and supplied execution material; reduce that material to the smallest faithful human execution surface; state exactly which files or references the human should use and in what order; emit exact user-visible text or procedural steps when the task requires them; answer bounded clarification needed to complete the delegated action; record the actual material used and the actual returned result; preserve exact returned bytes when available; note deviations or failed attempts without rewriting them as success; create the required return Handoff and execution Evidence within the delegated lineage.
- Does Not Authorize: changing the originating objective; adding new product requirements; selecting a different semantic authority merely for convenience; replacing a required human judgment or recipient review; remote write, purchase, publication, deployment, legal commitment, or other consequential action unless separately authorized by the controlling artifact; accepting its own execution output as product or project completion.
- Required Instrument: Pilot work should begin from an explicit bounded Task or Handoff that identifies the intended execution boundary, required inputs, expected result, and return destination. Completion should return through a durable Handoff with enough evidence to reconstruct what the human was asked to do and what actually came back.
- Human Boundary: the human performs the external action. Pilot owns instruction fidelity, scope containment, and evidence/return continuity; the human is not required to infer missing task intent or become the durable carrier of hidden context.
- Review Boundary: Pilot may verify transport facts, file identity, obvious completion conditions, and whether the requested external action was actually attempted. Semantic, technical, product, visual, or acceptance review remains with the role or human authority designated by the controlling work.

## Execution Contract

- Prepare: identify the bounded objective, ordered materials, role of each material, exact human action, exact user-visible input when applicable, and expected return artifact or signal.
- Guide: present the next human action in a copyable, decision-minimal form and avoid unrelated explanation while execution is pending.
- Receive: capture the returned artifact, message, file, receipt, or observation exactly enough to preserve evidence; distinguish exact source bytes from previews or descriptions.
- Report: record actual inputs, deviations, output identity, failures, and unresolved questions; do not convert absence of evidence into PASS.
- Return: manufacture or author the lineage-correct return Handoff immediately when the delegated execution is complete or blocked, returning control to the declared role rather than continuing the originating work.

## Execution Input Fidelity Boundary

- Human-Visible Input: when the controlling work supplies exact user-visible text, Pilot must present that text unchanged unless the controlling artifact explicitly permits adaptation. Pilot records the actual text the human was instructed to submit.
- External Compilation Boundary: Pilot must distinguish the exact human-visible instruction from provider-, host-, tool-, or model-internal prompt compilation, hidden preprocessing, or reformulation that Pilot cannot observe or control. Exact human-visible fidelity may be claimed when evidenced; provider-internal byte-for-byte equivalence must not be claimed without direct evidence.
- Deviation Reporting: observable host/tool rewriting, attachment substitution, reordered inputs, missing bytes, or other execution-fidelity deviations are material execution evidence. Pilot reports them without deciding whether they invalidate the originating work.
- Retry Boundary: Pilot retries only when the controlling artifact authorizes retry or the return role explicitly hands back a retry. A fidelity anomaly does not silently authorize a second attempt.

## Evidence And Output Placement

- Lineage-Local Evidence: when execution outputs are materialized inside a repository for active review, transient request, input, output, receipt, and review files should share the controlling lineage stem and directory with the artifact describing that execution moment where practical. Example: '001-1-1-1-evidence.trace.md', '001-1-1-1-generated-01.png', '001-1-1-1-review-01.webp'.
- Stable Promotion: transient output placement is not stable product placement. When a returned output is accepted or otherwise gains stable domain meaning, the reviewing/owning role promotes the accepted bytes or deterministic derivative outside .topics into the domain-appropriate reference/asset location, preserving immutable linkage to the originating lineage and hashes.
- Rejected Attempts: Pilot preserves rejected or superseded attempts only as required by the controlling evidence/transport lifetime. It does not permanently populate stable asset directories with every attempt.
- Exact Bytes: when exact returned bytes are available, Pilot preserves them without decode/resave transformation before return. Derived previews, repacks, or transforms are separate artifacts with separate identities.

## Holder Relationship

- Holder State: assignable per explicit session, invocation, or Handoff; no permanent holder asserted
- Possible Holder: a person, model, runtime, or conversational agent explicitly operating in the Pilot capacity for one bounded human-mediated execution context under supplied controlling artifacts

## Interpretation Limits

- Does Not Prove: that a particular person, model, runtime, chat, or external service currently holds Pilot; that the human completed the requested action; that returned material is correct or accepted; that Pilot has authority over the external system; that a successful transport is successful product work; or that a human relay upgrades ordinary conversation into durable truth.
- Must Not Be Treated As: a general assistant role, courier role, product manager, universal external-tool operator, architecture or schema authority, final reviewer, acceptance authority, remote-write credential, permanent holder identity, model-personality prompt, delegation proof beyond the controlling artifact, or a replacement for the role that owns the originating problem.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Roles](001-roles.trace.md)
  - Value: CddsZL0M8jPTiIDkZ_arKhHjt_hibdFfGktzbz_kA6Q

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 85SDSq7fSV1rmjZ4sITCRPZdzG1XFOZIePMjLlILNbI
