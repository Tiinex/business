# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [001-2-tooling-project.trace.md](001-2-tooling-project.trace.md)
  - Origin:
    - [relative](001-2-tooling-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-22 14:57:34
  - Authors: Anchor
  - Why: The normal VS Code workflow can Attach and Transport, but Handoff authoring and pointer materialization are still not durable or identity-complete: endpoint selection can degrade to free text, Role References are not reliably persisted, participant selection needs Core-backed multi-Workspace Attach UX, and qualified Role/material pointers must resolve through carried Workspaces or bounded cache on the restored single Package V1 model.
  - Summary: Close the remaining VS Code/Core Handoff authoring, participant selection, durable Role reference, cache-material, and Package V1 pointer-lineage gaps without reintroducing a second semantic or recipient package layer.
  - Status: ready/local

---

# Tooling Major 008 — Native Handoff Authoring And Durable Pointer Closure

## Objective

Complete the ordinary Tiinex Handoff workflow so VS Code is a thin, trustworthy host over shared Core semantics rather than a second Handoff implementation.

A human must be able to create and maintain a Handoff in VS Code by selecting qualified Roles/Identities from the currently open qualified Workspaces, optionally add one or more participant Roles during Attach, save durable canonical references in the Handoff, Attach the Handoff later or after restart, and Pack single- or multi-Handoff Package V1 carriers whose cache/material and pointer lineage is complete, numerically correct, adapter-resolvable, and free of parallel recipient/meta truth.

This Major exists because the remaining product gap is no longer basic Transport or Package-V1 emission. The unresolved chain is:

`open Workspace Role discovery -> authoring selection -> durable Handoff Reference -> Attach participant selection -> Core material closure -> numeric pointer lineage -> Package V1`.

Every acceptance criterion below is required. Passing internal tests while the normal VS Code operator flow remains weaker does not complete the Major.

## Current Human Observation

- VS Code can currently author a Handoff with free-text `From`, `To`, `From Kind`, and `To Kind`, but the previously useful qualified Role/Identity selectors are not available when Core discovery yields no endpoint catalog for the authoring context.
- The authored Handoff can therefore contain labels/kinds without durable `From Reference` / `To Reference`.
- Attach and Outgoing can succeed, and Transport is no longer the primary blocker.
- A Package can then legitimately omit endpoint Role pointers because no exact Role binding survived into the Handoff artifact.
- Outgoing may still visually imply a future Role pointer from endpoint labels even when Core cannot materialize that pointer.
- Existing host-side transient endpoint/participant state must not be the correctness boundary for a durable Tiinex Handoff.
- The Package V1 representation, numeric lineage, JSON-free normal path, and shared-Core direction restored immediately before this Major are non-regression invariants, not redesign scope.


## Scope

- Shared Core Handoff authoring and endpoint/participant qualification needed to persist exact canonical References.
- Core-backed multi-Workspace endpoint and participant discovery for VS Code.
- VS Code authoring UX for qualified endpoint selection and Attach-time multi-select participant Roles.
- Durable edit/reload/Attach behavior for authored Handoffs.
- Shared Core material closure from carried Workspaces or bounded cache/material ZIP.
- Package V1 numeric pointer lineage and truthful prospective Outgoing projection.
- Single- and multi-Handoff parity through the same Package V1 path.
- Deterministic machine regression coverage and final real-host Sigma acceptance.

The scope is deliberately end-to-end for the ordinary Handoff operator journey, but it is not authority to redesign Handoff semantics, introduce a new package representation, or duplicate shared Core behavior inside VS Code.

## Dependencies

- The accepted Tiinex Tooling Project as organizational parent and scope owner.
- The currently restored Package V1 normal path and its numeric Workspace/cache/Role/Handoff lineage mechanics.
- Existing canonical optional Handoff endpoint Reference semantics (`From Reference` / `To Reference`) and Role/Identity artifacts.
- Shared Core operator-context, Handoff endpoint, participant, material-closure, adapter, Package V1, and transport projections.
- Explicit operator-open Workspace roots supplied by the host; repository-recursive discovery is not a dependency.
- Business/Core/VS Code exact current source frontiers for implementation fan-out and later Anchor reconciliation.
- Sigma's real VS Code environment for final human acceptance only after deterministic machine qualification.
- Axiom/semantic-owner review only if implementation exposes an actual canonical contradiction; this is not a default dependency.

## Done Criteria

### 1. Qualified Role/Identity discovery during Handoff authoring

- Handoff authoring in VS Code offers qualified `From` and `To` Role/Identity selections discovered by Core from the explicit set of currently open qualified Workspace roots.
- Authoring discovery MUST NOT require an Outgoing context to exist first.
- VS Code supplies explicit open roots/context to Core and presents Core-qualified candidates; it does not recursively scan repositories or invent Role authority.
- Nested test, fixture, schema-example, or otherwise non-operator Workspace material MUST NOT appear as ordinary endpoint candidates unless that Workspace is itself explicitly opened/authorized as an operator root.
- Candidate presentation is human-readable and disambiguates same-label artifacts with kind and Workspace/provenance.
- The normal operator interaction is a selector/dropdown, not manual schema-field entry.
- A deliberate manual/unbound endpoint option remains available for identity-less Handoffs.

### 2. Manual / identity-less Handoffs remain first-class

- Qualified Role/Identity selection is optional.
- A human may deliberately author label/kind endpoints without a Reference.
- Core continues to accept and Pack such Handoffs without fabricating Role pointers and without reintroducing the historical optional-Reference Pack blocker.
- The UI distinguishes a deliberate unbound/manual endpoint from a failed qualified Role lookup.

### 3. Qualified endpoint selection becomes durable canonical Handoff state

When a human selects a qualified Role/Identity, Core authoring writes the exact canonical Reference into the Handoff artifact itself.

Example property:

```text
From: Sigma
From Kind: role
From Reference: [Sigma Role](business::.topics/roles/...)

To: Anchor
To Kind: role
To Reference: [Anchor Role](business::.topics/roles/...)
```

Acceptance:

- Core, not VS Code string manipulation, creates/validates the canonical Reference.
- The Reference survives save, VS Code reload/restart, new Outgoing creation, later Attach, and later Pack.
- Re-opening the Handoff lets VS Code reconstruct the selected endpoint from the durable artifact.
- Display labels are never sufficient authority for a qualified pointer.

### 4. No transient endpoint side-channel is required for correctness

- Existing or replacement host state such as `endpointSelections`, `OutgoingDraft.endpointRoles`, UI cache, or equivalent may improve UX but MUST NOT be required for semantic correctness.
- An existing Handoff containing exact endpoint References is sufficient by itself for Core to rediscover endpoint requirements and materialize the same endpoint pointers after restart.
- Attach of an existing Handoff does not require the human to select the same endpoint Roles again.
- Removing transient VS Code state must not weaken the Package result.

### 5. Attach provides explicit multi-select participant Role discovery

At Attach time, VS Code provides a multi-select control for **zero, one, or multiple additional participant Roles**.

Acceptance:

- Participant candidates are projected by Core from the same explicit multi-Workspace operator context: all currently open qualified Workspaces, not merely the Handoff's own Workspace and not a repository-recursive host scan.
- The operator may select multiple participant Roles in one Attach interaction.
- Each selected participant has exact qualified Workspace/artifact identity; labels alone are not authority.
- Participant selection is passed into the shared Core Handoff/Attach/material-closure path. VS Code does not implement participant semantics or pointer construction itself.
- Repeated selection of the same qualified participant is deduplicated deterministically.
- No participant is inferred merely because its Role artifact is carried or visible.

### 6. Participant material comes from carried Workspaces or cache according to actual Outgoing membership

For every participant selected during Attach:

- If that participant Role's authoritative Workspace is already included in the Outgoing package set, Core resolves the Role directly from that carried Workspace.
- If that participant Role's authoritative Workspace is **not** included in Outgoing, Core carries only the required bounded Role/material closure in the cache/material ZIP.
- The host MUST NOT silently add the participant's entire Workspace to Outgoing merely to make Role resolution convenient.
- Cache carriage preserves the Role's qualified source identity/provenance and provides normal adapter-resolvable access to its exact material.
- The same rule applies generically to endpoint Role material and other required external material.

### 7. Participant authority is durable enough for later Pack

- The effective participant selection attached to the Handoff/Outgoing must survive the ordinary lifecycle required by the product: tree refresh, Pack, and any supported restart/requalification boundary.
- Correctness MUST NOT depend on an unqualified in-memory label list.
- Core owns the qualified participant projection used by Pack.
- A later Pack must materialize the same selected participant Role pointers or explicitly report why a previously selected qualified participant can no longer be resolved.

### 8. Attach derives endpoint requirements from the Handoff artifact

- For Handoffs with `From Reference` / `To Reference`, Attach derives endpoint Role requirements from those References.
- Attach does not ask the user to reselect durable endpoint Roles.
- Attach does not require a VS Code-private endpoint binding payload to make Pack work.
- A stale or unresolved Reference produces explicit unresolved state before Pack rather than optimistic pointer presentation.
- Optional References remain optional.

### 9. Role pointers are materially complete at Pack

For every qualified Role that requires package-local resolution, Pack emits the necessary pointer on the Handoff route's actual ancestor chain.

Expected shape when participant and cache are both present:

```text
Workspace
└─ Cache/material
   └─ Participant Role pointer
      └─ From Role pointer
         └─ To Role pointer
            └─ Handoff pointer
```

Acceptance:

- Participant pointers precede endpoint pointers.
- Endpoint pointers reflect exact qualified Handoff References, never display labels alone.
- A qualified Role pointer visible as prospective output before Pack is actually present after Pack.
- Identity-less endpoints do not receive fabricated Role pointers.
- Multiple participants extend the real numeric Parent chain; they do not create a separate participant namespace.

### 10. Required Context / Process / generic external material resolves through the shared adapter model

This Major must not create type-specific VS Code logic for Process artifacts.

For any Required Context or other required material:

- If the exact target is already available in a carried Workspace, Core resolves it through the Workspace representation/adapters without package-local duplication.
- If required material is not in a carried Workspace, Core carries the required bounded material in cache/material ZIP.
- Qualified reference identity and provenance are preserved.
- Normal adapter/workspace-qualified/permalink resolution can resolve the material from the cache.
- The behavior is generic across Role, Process, and other allowed material types.

### 11. Cache/material ZIP is a real numeric Parent in Package V1 lineage

When cache is required, the canonical package-local lineage is:

```text
001-5-1
Workspace trace
Workspace ZIP

001-5-1-1
Cache/material trace
Cache/material ZIP

001-5-1-1-1
Participant pointer

001-5-1-1-1-1
From pointer

001-5-1-1-1-1-1
To pointer

001-5-1-1-1-1-1-1
Handoff pointer
```

Acceptance:

- Workspace trace and Workspace ZIP share the Workspace filename dimension.
- Cache trace and cache ZIP share the cache filename dimension.
- Cache artifact declares the Workspace artifact as Parent.
- The first route pointer declares cache as Parent when cache exists; otherwise it descends directly from Workspace.
- Every following pointer declares the immediately preceding pointer as Parent and its numeric filename dimension mirrors that continuity.
- Multiple participants continue the same numeric chain.
- If cache is unnecessary, no empty/artificial cache node is emitted.
- Cache contents are adapter-resolvable; no extra cache-index JSON is required.

### 12. Outgoing preview reflects Core-qualified prospective Package truth

- Outgoing does not invent pending Role pointers from `From`/`To` labels.
- If Outgoing presents `Role pointer - pending Pack`, Core already has exact qualified binding/material projection sufficient to materialize it.
- If a Role binding is unresolved, Outgoing says so explicitly and does not promise a pointer.
- Prospective pointer/material presentation comes from shared Core projection used by Pack, not duplicated VS Code filename/lineage logic.

### 13. Single- and multi-Handoff use exactly the same Core Package V1 pipeline

- One Handoff and multiple Handoffs use the same recipient-facing Package V1 representation and the same material/pointer logic.
- Route cardinality MUST NOT select another package representation.
- Each Handoff receives a correct numeric route branch/chain below the appropriate Workspace/cache ancestor.
- Shared Workspace/cache material may be reused only where Core proves that reuse is qualified.
- Material and Role authority from one route MUST NOT leak into another route.
- Adding a second Handoff MUST NOT rewrite semantic source prefixes, introduce hash/source-path filenames, or change the package contract.

### 14. VS Code remains a thin Core consumer

VS Code MAY:

- supply explicit open Workspace roots/operator context;
- present Core-qualified endpoint and participant candidates;
- collect operator selections;
- render Core-qualified prospective state;
- invoke shared Core authoring, Attach, Pack, and Transport operations.

VS Code MUST NOT independently:

- decide Role/Identity authority;
- construct qualified artifact references;
- derive material closure;
- construct participant/endpoint pointer semantics;
- allocate pointer lineage or filenames;
- implement cache closure;
- infer repository-local material because of path proximity;
- maintain a second semantic model required for correctness.

Any rule needed by CLI/Tooling and VS Code belongs in shared Core.

### 15. Authoring/edit/restart lifecycle is proven

A real acceptance scenario must pass:

```text
1. Open VS Code with multiple qualified Workspaces, including Business and another working Workspace.
2. Create a Handoff in the intended authoring Workspace.
3. Select qualified From Role/Identity from the Core-projected dropdown.
4. Select qualified To Role/Identity from the Core-projected dropdown.
5. Save the Handoff.
6. Reload/restart VS Code.
7. Re-open the Handoff; the qualified endpoint selections are reconstructed from durable References.
8. Create a new Outgoing.
9. Attach that existing Handoff.
10. Use Attach multi-select to choose zero, one, or multiple extra participant Roles from the open multi-Workspace context.
11. Pack.
12. Inspect the Package V1 carrier and verify the complete numeric cache/participant/from/to/Handoff lineage actually materialized.
13. Transport the package.
```

No semantic selection made before step 6 may need hidden host state after step 6.

### 16. Positive external-cache participant scenario is mandatory

At least one deterministic machine test and one real-host Sigma scenario must select a participant Role whose authoritative Workspace is open for discovery but intentionally **not included in the Outgoing Workspace package set**.

Expected result:

- participant is discoverable/selectable in Attach multi-select;
- participant's entire Workspace is not silently added;
- exact bounded participant Role/material closure is emitted into cache/material ZIP;
- participant pointer resolves to that cached material using normal adapters;
- cache remains Parent of the participant/from/to/Handoff pointer chain;
- recipient cold orientation/grounding qualifies the resulting material without a recipient/meta sidecar.

This scenario is mandatory because it proves the cache design rather than only testing absence/error paths.

### 17. Positive carried-Workspace participant scenario is mandatory

A complementary scenario must select a participant Role whose authoritative Workspace **is already included in Outgoing**.

Expected result:

- Role material resolves directly from the carried Workspace;
- no duplicate copy of that Role is added to cache merely because it is a participant;
- participant pointer remains in the correct numeric Handoff route lineage;
- cold recipient resolution reaches the exact carried Role material.

### 18. Real-host VS Code acceptance remains the final gate

Machine tests are necessary but not sufficient.

Sigma acceptance must exercise at minimum:

- endpoint dropdown discovery from open multi-Workspace context;
- author and save a Handoff with durable `From Reference` / `To Reference`;
- reload/re-open and verify selections persist;
- Attach existing Handoff;
- Attach participant multi-select with multiple Roles where available;
- one participant resolved from an already-carried Workspace;
- one participant/external Role resolved through cache when its Workspace is not included in Outgoing;
- single-Handoff Pack;
- multi-Handoff Pack;
- visual Package V1 inspection;
- Transport;
- no blocker hidden behind optimistic Outgoing preview.

Major completion requires the human-visible operator workflow, not only source/unit/package assertions.

## Non-Regression Invariants — MUST NOT

### One recipient-facing Handoff Package representation

- Package V1 is the normal recipient-facing representation for pointerless, single-Handoff, and multi-Handoff carriage.
- Route count must never activate a second recipient-facing package standard.
- Experimental/specimen artifact-first representations must not silently re-enter the normal path.

### No recipient/meta sidecar truth

Do not introduce or reintroduce:

- `tiinex-recipient-v2.transport.json`;
- an equivalent recipient manifest/index under another filename;
- cache index JSON duplicating artifact authority;
- another parallel byte-map/semantic truth required for recipient understanding.

Exact payload bytes, qualified artifact envelopes, Parent continuity, Workspace/cache bindings, and adapters are the verification/resolution surface.

### Numeric artifact lineage only

- Filename dimensions mirror actual Parent lineage.
- No alphabetic semantic dimensions such as `e` or `p`.
- No source-path slug/hash dimension used as a substitute for lineage.
- Classification such as participant/from/to belongs in artifact content/role, not in invented filename dimensions.

### Cache is transported material, not semantic authority

- Handoff and repository artifacts own meaning.
- Cache only makes exact required external material available.
- Cache presence MUST NOT create Role participation, endpoint identity, Required Context meaning, or authority that the Handoff/artifacts do not already declare.

### Optional References remain optional

- Identity-less endpoints remain valid.
- Strong qualified References produce stronger exact materialization.
- Missing optional Reference does not by itself block a valid Handoff package.

### Open Workspace discovery only

- Endpoint/participant discovery begins from explicit operator-open qualified Workspace roots.
- Do not restore recursive repository scanning or nested test-fixture discovery as normal host behavior.

### No host-specific reimplementation of shared semantics

- Kodax/VS Code consumes Core projections and operations.
- Loom/Core owns reusable authoring, qualification, material closure, lineage, Package V1, and adapter behavior.
- Do not fix Core deficiencies by adding a permanent VS Code-private semantic layer.

### No canonical Docs/schema change without an actual semantic contradiction

- The expected References, Handoff semantics, Workspace/cache lineage model, and adapters are treated as existing semantics.
- If implementation exposes a genuine contradiction, fail visible and escalate to the semantic owner rather than inventing a workaround.
- This Major does not authorize broad schema redesign merely to make current implementation easier.

## Required Machine Acceptance

Before returning to Sigma, the integrated Core + VS Code candidate must include deterministic regressions for:

- endpoint discovery across multiple explicit open Workspace roots;
- exclusion of nested/non-open fixture Workspaces;
- manual identity-less authoring;
- qualified endpoint selection writing durable canonical References;
- reload/reparse preserving those References;
- Attach of an existing Handoff without endpoint side-channel state;
- Attach multi-select of multiple qualified participant Roles;
- participant direct resolution when its Workspace is in Outgoing;
- participant cache resolution when its Workspace is open for discovery but excluded from Outgoing;
- generic external Required Context cache resolution;
- numeric cache -> participant(s) -> From -> To -> Handoff Parent lineage;
- Outgoing preview matching actual Pack;
- single-Handoff Package V1;
- multi-Handoff Package V1 through the same normal builder;
- no `e`/`p` pseudo-dimensions;
- no source-path/hash filename leakage;
- no recipient/meta JSON sidecar;
- cold orientation/grounding through the produced carrier;
- bridge/package regressions against the exact integrated Core bytes, not a stale or separately patched Core.

## Ownership And Work Split

- **Loom / Core:** shared endpoint/identity authoring capability, canonical durable References, endpoint/participant/material qualification, cache closure, adapter resolution, prospective Package projection, pointer lineage, and Package V1 mechanics.
- **Kodax / VS Code:** thin operator UX over Core — open-root context, endpoint selectors, Attach participant multi-select, durable edit/reload presentation, truthful Outgoing rendering, and invoking the shared Core path.
- **Anchor:** architecture/invariant protection, parallel fan-out, exact source reconciliation, integrated acceptance, and Sigma gate preparation.
- **Sigma:** real VS Code operator acceptance and human usability judgment.
- **Axiom / semantic authority:** only if a genuine canonical semantic contradiction is found; not a default dependency.

Loom and Kodax must not repair each other's owned layer by duplicating logic. Parallel work is expected where source ownership is disjoint.

## Explicit Out Of Scope

- New recipient package standards.
- Broad Handoff schema redesign without semantic contradiction.
- New metadata databases/manifests for byte verification.
- Recursive repository role discovery.
- Release, publication, deployment, commit, push, or other remote mutation unless separately authorized.
- Viewer-specific presentation work unrelated to the VS Code Handoff operator flow.
- Using Sigma as the routine machine test runner for behavior deterministic tests can prove first.

## Definition Of Done

This Major is complete only when:

> A user can create a Tiinex Handoff in VS Code by selecting qualified endpoint Roles/Identities from the currently open Workspaces; Core writes those choices durably as canonical Handoff References; after restart the same Handoff can be attached without hidden endpoint state; Attach offers a Core-backed multi-select for zero or more extra participant Roles across the open multi-Workspace context; participant/endpoint/external material resolves directly from included Outgoing Workspaces or, when the authoritative Workspace is not included, through bounded cache/material ZIP; Pack materializes the required participant/From/To/Handoff pointers on one real numeric Parent lineage; single and multi-Handoff use the same Package V1 representation; and the resulting carrier contains no parallel recipient/meta truth.

And additionally:

> Deliberately identity-less Handoffs remain valid and packable without fabricated Role pointers, while Outgoing always tells the truth about what Core can actually materialize.

Machine qualification and real-host Sigma acceptance are both required before closure.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-tooling-project.trace.md](001-2-tooling-project.trace.md)
  - Value: id2V3L4aVv616_NbFUngZrbSnZ9T_HN5G-x8Z1003W4

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: pGG1b6GOIfihv1TvR8xXuymohSGoimS0jzPdVMD1-dI