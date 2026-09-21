# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-21 13:52:52
  - Trace: [001-1-4-1-3-1-anchor-to-axiom-independent-semantic-boundary-audit.trace.md](001-1-4-1-3-1-anchor-to-axiom-independent-semantic-boundary-audit.trace.md)
  - Origin:
    - [relative](001-1-4-1-3-1-anchor-to-axiom-independent-semantic-boundary-audit.trace.md)
- Current
  - Current Schema: tiinex.decision.v1
  - Created At: 2026-09-21 14:09:11
  - Authors: Axiom
  - Why: The architecture-recovery Handoff requires a durable Axiom semantic disposition before Core or VS Code implementation resumes.
  - Summary: Classify canonical Handoff endpoint/reference/material semantics, reject authority leakage from carriage and internal bindings, and bound Core/VS Code implementation after reconciliation.
  - Status: ready/local

---

# Axiom Semantic Boundary Disposition — Handoff Endpoints, References, And Carried Material

## Decision

- State: accepted
- Subject: canonical Handoff endpoint, reference, material-resolution, and recipient-carriage boundaries for the architecture-recovery audit
- Decision: within the transferred Axiom semantic-audit scope, preserve the current canonical Handoff requirement for explicit readable `From`, `From Kind`, `To`, and `To Kind`; treat endpoint, capacity, material, return, and result References as durable resolution aids rather than substitutes for readable declarations or independent authority; keep resolver/package binding and exact carried-byte provenance mechanically separate from semantic identity and applicability; and reject any implementation that derives endpoint identity, transfer truth, participant authority, required-context meaning, or semantic applicability from package placement, cache presence, internal binding keys, host state, or byte availability.

## Source-Proven Canonical Semantics

- The current `tiinex.handoff.v1` contract defines a Handoff as one explicit bounded transfer from one declared `From` endpoint to one declared intended `To` endpoint.
- `Purpose`, `From`, `From Kind`, `To`, and `To Kind` are required Handoff-party fields. `From Kind` and `To Kind` are closed to `party`, `role`, or `unknown`; an unresolved classification is therefore represented explicitly as `unknown`, not by omitting the field.
- `From` and `To` remain required readable endpoint declarations even when no durable Party or Role artifact exists. Precise human-readable descriptors are sufficient for readability; a durable endpoint Reference is optional.
- `From Reference` and `To Reference` are optional resolution aids. They must not override contradictory readable endpoint identity.
- Capacity is separate from endpoint identity. When the endpoint is a Role, duplicative Capacity fields are absent; when a Party endpoint acts in a distinct bounded Role/capacity, the Party identity and capacity remain separate declarations.
- An unresolved optional endpoint or capacity Reference remains unresolved. Tooling must not guess from path, filename, `Authors`, repository actor, transport recipient, application session, Role-holder heuristics, workspace membership, or package adjacency.
- A readable Capacity that materially contradicts a resolved Capacity Reference creates ambiguity; neither silently overrides the other.
- Required Context and Reference Context declare material meaning independently from package membership. Their declaration names are readability handles, not material identity.
- Required-context `Availability` explicitly preserves `available`, `unavailable`, `unresolved`, or `unknown`. Missing or unresolved required material must not be silently replaced by repository-global search, package guessing, filename guessing, or fabricated source.
- `Material Reference`, `Retained By Reference`, `Return To Reference`, endpoint References, and capacity References are resolution aids with field-specific semantics. Their presence does not create transferred responsibility, holder assignment, acceptance, delegation authority, or proof of review.
- A Handoff is not a package manifest, resolver, transport receipt, workflow engine, or protocol state machine. Packaging and transport may carry a Handoff representation but do not define transfer semantics.
- Package/workspace/message inclusion, cache presence, exact byte availability, directory location, and transport delivery do not create transfer truth, recipient identity, context classification, authority, acceptance, completion, or successful material resolution.
- Required context may be referenced rather than physically packaged when its Reference remains usable.
- The current Core Workspace boundary confirms that package implementation belongs to Core while canonical schema authority remains in Docs; current Core behavior is therefore implementation evidence only and cannot create or revise Handoff semantics.

## Disposition Of Recovered End-Of-Session Ideas

### Already Authoritative

- Separate readable endpoint identity from optional durable Party/Role References.
- Preserve unresolved optional References instead of guessing replacements.
- Preserve contradiction/ambiguity when readable capacity and resolved capacity material disagree; do not silently pick one.
- Separate required context, reference-only context, transferred work/responsibility, and retained responsibility.
- Separate material availability from responsibility transfer.
- Separate semantic Handoff truth from packaging, transport, resolver state, cache layout, and carried-byte presence.
- Allow required material to be referenced instead of physically carried when the durable Reference remains usable.
- Keep Docs as semantic owner and Core/host layers as implementation consumers.

### Requires New Semantic Or Mechanical Disposition Before Adoption

- A transparent carried-material/provenance manifest is compatible with current Handoff semantics and is preferable to opaque cache-only recipient behavior for inspectability, but it is not currently a Handoff semantic requirement. If durable package selection, closure, provenance, or resolver state has independent semantic value, it belongs in the package/planner/payload/evidence authority that owns that truth rather than being inferred from Handoff context or package placement.
- A canonical endpoint-level resolver state field such as `resolved`, `unresolved`, `ambiguous`, or `contradictory` is not part of the current Handoff contract. Core may compute such states mechanically from exact declarations and resolution evidence, but persisting them as new Handoff semantics requires a Docs-owned schema disposition.
- A durable semantic Reference and an internal workspace/path/material binding are different classes of fact. Core may maintain an internal binding from a semantic Reference to exact carried bytes and provenance, but that binding remains resolver/transport evidence unless a separately owned schema explicitly makes it semantic.
- Exact-carried-byte provenance may strengthen reproducibility and mechanical qualification, but it does not by itself establish semantic identity, applicability, authority, participant status, transfer, or acceptance.

### Rejected For Handoff Semantics

- Making readable `From` or `To` endpoint identity optional. Without a declared origin and intended recipient, the artifact no longer satisfies the current Handoff meaning.
- Making `From Kind` or `To Kind` absent as a way to express uncertainty. The maintained contract already provides explicit `Kind: unknown`; omission would collapse “unknown” into “not declared” and weaken machine-readable intent.
- Treating an internal binding key, archive entry, cache object, workspace path, package slot, transport destination, host session, current holder, or available byte blob as a durable semantic Reference by convenience.
- Treating successful resolution of an optional Reference as permission to rewrite or override contradictory readable endpoint declarations.
- Treating unresolved, ambiguous, or contradictory resolution evidence as permission to search globally and select a plausible substitute.
- Treating transparent carriage as proof that carried material is Required Context, applicable to the current work, authoritative, reviewed, accepted, or transferred.
- Expanding `tiinex.handoff.v1` into a generic package manifest, dependency resolver, or lifecycle state machine.

## Implementation Boundary For Loom / Core After Anchor Reconciliation

- Core may own mechanical Reference resolution, exact-byte closure, carriage manifests, provenance receipts, and internal bindings, provided those mechanics preserve rather than rewrite the semantic Handoff declarations.
- Core may expose resolver outcomes such as resolved, unresolved, ambiguous, or contradictory as derived mechanical/validation state. Those outcomes must retain the exact source facts and must not masquerade as new Handoff fields or semantic authority.
- Where an operation requires exact identity or exact material and resolution is unresolved, ambiguous, or contradictory, Core should fail visible/closed rather than infer from repository-global search, filenames, paths, package adjacency, host/session state, or cached Roles.
- A transparent carriage manifest may enumerate exact carried materials, workspace identity, internal binding, digest/provenance, and resolution outcome for recipient inspection. Its fields must be documented as carriage/resolver evidence and must not implicitly classify context, participants, transfer, authority, or applicability.
- Durable References should remain stable artifact-level references independent of package layout. Internal package/cache bindings should be replaceable without changing the semantic Handoff bytes.
- Core must not require physical packaging of every Required Context item when the Handoff truthfully declares an available usable Reference instead.

## Implementation Boundary For Kodax / VS Code After Anchor Reconciliation

- VS Code may render readable endpoint identity/capacity and separate Reference-resolution diagnostics, but it must not hide or replace the readable declarations because a Reference resolves.
- VS Code may surface unresolved/ambiguous/contradictory diagnostics and transparent carried-material/provenance views, but it must not infer endpoint identity, holder/participant authority, context applicability, or transfer truth from UI session state, open workspace state, package contents, cache entries, or transport recipient.
- Shared Reference resolution, closure, packing, provenance, and binding logic belongs in Core. The host should consume qualified Core results instead of duplicating resolver or package semantics in controller/UI edge cases.
- Host behavior must preserve explicit unknown/unresolved facts and fail visibly when an action requires authority or identity that the semantic artifacts do not establish.

## Schema-Change Boundary

- This disposition does not mutate `tiinex.handoff.v1` and does not authorize Core or VS Code to add or remove Handoff fields.
- Any future change that makes endpoint identity or kind optional, introduces canonical endpoint-resolution state fields, or elevates carriage/binding data into semantic authority requires a new Docs-owned semantic decision and schema qualification.
- If future requirements need a pre-Handoff object with no explicit intended recipient, use or define the artifact type that owns invitation/planning/unresolved-routing semantics rather than weakening Handoff’s explicit transfer meaning.

## Reconciliation Boundary

- Anchor retains responsibility to reconcile this Axiom disposition with the independent Loom and Kodax returns before implementation is authorized.
- This disposition is authoritative only for the bounded semantic audit transferred to Axiom. It is not program acceptance, implementation approval, schema migration completion, or proof that current Core/VS Code behavior conforms.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-4-1-3-1-anchor-to-axiom-independent-semantic-boundary-audit.trace.md](001-1-4-1-3-1-anchor-to-axiom-independent-semantic-boundary-audit.trace.md)
  - Value: cAdJLXSyWI9qEnNYk05DNfEHeNopZrx9o9zXIJ25ygs

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: ZGkh5bDKrRJQNN7P1JK8h85S8BCMBbPmElMJbpIK8EE