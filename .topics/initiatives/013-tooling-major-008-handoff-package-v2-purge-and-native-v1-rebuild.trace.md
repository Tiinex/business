# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-23 14:01:25
  - Trace: [040-anchor-to-kodax-tooling-major-008-capable-exact-lockfile-build-g.trace.md](handoffs/040-anchor-to-kodax-tooling-major-008-capable-exact-lockfile-build-g.trace.md)
  - Origin:
    - [relative](handoffs/040-anchor-to-kodax-tooling-major-008-capable-exact-lockfile-build-g.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-24 00:20:00
  - Authors: Anchor
  - Why: Six days of Package V1 improvement work accumulated recipient-v2/Handoff-Package-V2 machinery, alternate manufacture/verification paths, binary/cache indirection and host-facing drift. The retired machinery must be removed before rebuilding one direct readable Package V1 path.
  - Summary: Purge Handoff Package V2 as executable architecture, then rebuild native Package V1 in Core + LLM Tooling from the agreed human-readable oracle; prove physical ZIP, cold LLM grounding and anti-drift acceptance before Sigma freezes Core and any VS Code work resumes.
  - Status: ready/local

---

# Tooling Major 008 — Handoff Package V2 Purge And Native Package V1 Rebuild

## Objective

Restore one understandable Handoff Package architecture by removing the abandoned recipient-v2/Handoff-Package-V2 implementation before further Package V1 development, then complete the prior Core-first recovery plan against one direct Package V1 manufacture/orient/ground path.

This Task recovers and extends the earlier successor Task 015 acceptance plan from the qualified Anchor carrier onto the latest Business baseline. The key sequencing change is explicit: **V2 purge is Gate 0 and precedes Uppdrag 1 implementation.**

The work remains Anchor-driven without specialist implementation loops. Sigma retains final human acceptance. VS Code remains a thin downstream consumer and does not regain implementation scope until Core/LLM Package V1 is accepted and frozen.

## Gate 0 — Remove Handoff Package V2 Machinery Before Rebuild

### Purge Boundary

Remove executable Handoff Package V2 / recipient-v2 architecture from every active repository surface where it exists:

- source modules, builders, inspectors, writers, conversion/upgrader paths and compatibility switches;
- public package exports that expose recipient-v2/Handoff-v2 implementation;
- CLI, Node, LLM or package operations that can choose or fall back to the retired representation;
- active tests, fixtures and validation baselines whose purpose is to execute or preserve the retired representation as current behavior.

Do **not** remove `sha256-base64url-c14n-v2`. That is the current trace self-integrity method and is unrelated to Handoff Package V2.

Historical `.topics/*.trace.md` provenance may continue to describe recipient-v2/Handoff-v2 because historical artifacts must remain honest about prior architecture. Historical mention is not executable support.

### Gate 0 Current Candidate State

The current local purge candidate establishes:

- Core: recipientV2 and archiveV2 implementation files removed; recipient-v2 exports/writer/inspector paths removed; new Handoff Package manufacture/orient/materialization paths fail closed at an explicit `portable.handoff-package-v1.rebuild-required` boundary instead of falling back to V2.
- Core: anti-regression coverage scans active Package tooling for retired V2 names, hidden JSON carrier/closure/companion truth, `handoff.material/` and `material.bin`; trace c14n-v2 integrity remains independently verified.
- Core: normal Core qualification outside the intentionally removed Handoff-package path remains green (`npm test`, portable smoke and embedded bootstrap qualification).
- App: stale cross-package recipient-v2 cases and recipientV2 static-validation debt entries removed so App no longer teaches or exercises the retired representation.
- VS Code: whole source/test/tools/scripts/docs/dist scan found no explicit recipient-v2/Handoff-v2 machinery; therefore no purge mutation is justified there.
- Final whole-org active-support sweep across all 16 supplied repositories found zero retired V2 support references outside the intentional Core anti-regression test patterns; historical `.topics` provenance remains excluded from purge by design.

Gate 0 is complete only when a final whole-org active-code scan remains clean and the changed repositories pass the qualification available from the carried Workspace bytes.

## Package V1 Product Intent

A Handoff Package is one portable receiver-facing ZIP that lets a human or fresh LLM:

```text
receive one ZIP
  -> read Start
  -> qualify embedded Tooling bootstrap
  -> orient the package
  -> select/confirm the intended Handoff route
  -> ground exact Workspaces + required context + Roles
  -> reconstruct current work and applicable process/policy context
  -> continue without producer-chat memory
```

The implementation should be boring and singular:

```text
ONE PACKAGE GRAMMAR
ONE SOURCE OF TRUTH
ONE NEW-OUTPUT PATH
```

Readable Markdown artifacts, exact Workspace ZIPs, bounded cache ZIPs, adapter-native references, trace integrity and explicit pointer lineage are preferred over opaque recipient databases, detached byte maps or hidden compatibility manifests.

## Canonical Package V1 Recipient Shape

The package root is flat. A maximal representative carrier may contain:

```text
001-tiinex-handoff-package.trace.md
001-1-READ-BEFORE-PROCEEDING.trace.md
001-2-bootstrap.trace.md
001-2-bootstrap.zip
001-3-<workspace-a>.workspace.md
001-3-<workspace-a>.workspace.zip
001-3-1-<workspace-b>.workspace.md
001-3-1-<workspace-b>.workspace.zip
001-3-1-1-cache.trace.md
001-3-1-1-cache.zip
001-3-1-1-1-<process>-pointer.trace.md
001-3-1-1-1-1-<policy>-pointer.trace.md
001-3-1-1-1-1-1-<participant>-role-pointer.trace.md
001-3-1-1-1-1-1-1-<from>-from-role-pointer.trace.md
001-3-1-1-1-1-1-1-1-<to>-to-role-pointer.trace.md
001-3-1-1-1-1-1-1-1-1-handoff-pointer.trace.md
```

Exact ordinal allocation may vary with carried Workspaces/routes and optional dependencies. The invariant is one numeric Parent chain/branch grammar with no alternate recipient representation.

### Workspace ZIP Rule

Each `.workspace.zip` is the exact Workspace/repository byte tree from its repo root. It does not introduce an extra organization/repository wrapper inside the Workspace ZIP.

Example:

```text
<workspace>.workspace.zip
├── README.md
├── package.json
├── src/
├── test/
└── .topics/
```

### Cache ZIP Rule

Cache is only for required exact material not already available through carried Workspace bytes. Cache does not pretend to be a Workspace and must not duplicate material that is already carried.

Cache path identity follows the owning adapter's natural identity convention instead of a generic `material/` namespace or a hash-to-file lookup table.

For GitHub the intended readable shape is:

```text
<cache>.zip
└── github/
    └── Tiinex/
        └── business/
            └── <original repo-relative path>
```

General rule:

```text
<adapter namespace>/<adapter-native source identity>/<original source-relative path>
```

The cache descriptor binds exact source identity/commit and integrity, but the cached path must be deterministically derivable rather than maintained through a parallel JSON mapping database.

Do not place commit/hash tokens into every directory path merely to create uniqueness. Exact version binding belongs in qualified source/cache metadata and byte verification while the path remains human navigable.

## General Grounding Pointer Model

Process, Policy, endpoint Roles, participant Roles and the selected Handoff must not become five unrelated resolver systems.

Use one generic grounding dependency/resolution mechanism, with human-readable pointer names where useful.

Semantic authority stays with the referenced artifacts and Handoff declarations. In particular:

- Process/Policy material required for correct execution is carried through ordinary Handoff `Required Context` / explicit qualified relation authority.
- Do not create a privileged Policy semantic channel merely because the package projects a file named `*-policy-pointer.trace.md`.
- Role pointers are grounding aids and do not create holder identity, participation, consent or authority.
- The authoritative Handoff remains inside its carried Workspace; the root pointer identifies/resolves exact authoritative bytes rather than duplicating Handoff truth.

A pointer should preserve the adapter-native qualified reference. Tooling resolution should behave conceptually as:

```text
exact reference
  -> already available from a carried qualified Workspace? use it
  -> otherwise exact matching bounded cache material? use it
  -> otherwise host/provider can perform read-only resolution? request it
  -> otherwise emit explicit manual-input request
  -> ingest returned bytes
  -> verify exact reference/integrity
  -> continue or fail closed
```

Do not rewrite GitHub permalinks into Package-private pseudo-identities merely to resolve local bytes.

## LLM / Host Recovery Boundary

LLM sandboxes may be unable to resolve GitHub permalinks or network URLs directly. This is an expected host-capability boundary, not a reason to invent a second cache model.

When exact required material is absent from carried Workspace/cache bytes:

- Tooling should describe the exact read-only material request to the LLM/host.
- An LLM may use an available repository/web connector to **fetch/read only**.
- GitHub connector mutation is forbidden for this recovery path.
- If the LLM cannot fetch, Tooling should provide a manual input path so a human can return the requested exact content/bytes.
- Returned content must be rebound and verified by Tooling before it gains material authority.
- No hidden session memory or unverified pasted content becomes equivalent to the declared source.

## Uppdrag 1 — Core + LLM Tooling Only

After Gate 0, rebuild the missing path directly in Core/portable Tooling. VS Code implementation remains frozen.

### Gate 1 — Freeze The V1 Oracle

Before implementing, encode the agreed Package V1 structure and forbidden architecture as executable acceptance. Do not weaken the oracle to fit existing code.

Hard forbidden new-output behavior includes:

- recipient-v2/Handoff-v2 manufacture, verifier or conversion dependency;
- route-count-dependent representation switching;
- hidden recipient/meta/route/workspace JSON as parallel truth;
- `material.bin` or hash-indexed cache representation replacing readable adapter-native paths;
- detached authoritative Handoff copies;
- host-owned package lineage/cache/Role/participant semantics;
- output-shape-only acceptance while execution still uses an alternate internal carrier.

### Gate 2 — Native Direct Package V1 Manufacture

The only accepted new-output shape is:

```text
qualified normalized Core plan
  -> Package V1 allocation
  -> Package V1 materialization
  -> Package V1 verification
  -> physical ZIP
```

The normalized Core plan must be sufficient for:

- carried Workspace bindings and exact payload provenance;
- single or multiple exact Handoff routes;
- endpoint Role references/material;
- explicit participant Roles 0..N;
- ordinary Required Context dependencies including selected process/policy material;
- carried-vs-cache resolution;
- deterministic cache adapter path projection;
- numeric package Parent lineage;
- Start/bootstrap contract;
- direct V1 read/orient/ground qualification.

### Gate 3 — Physical ZIP Black-Box Matrix

At minimum prove real serialized archives for:

1. single route, zero additional participants;
2. participant/endpoint Roles already present in carried Workspace(s), no redundant cache;
3. external endpoint/participant Role material through bounded cache;
4. Required Context process/policy material through carried Workspace and through cache;
5. multi-Workspace carrier with one authoritative Handoff in one Workspace;
6. multi-route package using the same grammar;
7. multi-route/shared external material without whole-repository cache expansion.

For each archive prove manufacture -> physical ZIP inspection -> orient -> selected route ground -> bootstrap cold consumption.

### Gate 4 — Anti-Drift / Mutation Proof

Tests must fail if any future change reintroduces or depends on:

- retired recipient-v2/Handoff-v2 builders/verifiers/writers;
- hidden JSON parallel recipient truth;
- `.bin` cache indirection;
- wrong Parent/pointer lineage;
- stale pointer target bytes/hash;
- carried material duplicated into cache;
- unbounded cache expansion;
- sibling-route material borrowing;
- host-specific semantic reconstruction.

Source grep may be one guard, but acceptance must also prove the executed new-output path.

### Gate 5 — Fresh LLM Usability

A fresh LLM receives only the Handoff Package and the explicit Start/routing instruction. It must use the packaged Tooling rather than producer-chat knowledge to:

- qualify Start/bootstrap;
- orient route(s);
- resolve carried Workspace and cache material;
- identify required Role/process/policy grounding context;
- reconstruct current Task/Handoff authority;
- explain unresolved host fetch/manual-input needs precisely;
- reach the correct bounded continuation without improvising missing authority.

A required final variant starts from an empty multi-workspace environment in which only one local Workspace exists with the Task/Handoff and at least two required Role/context artifacts are absent locally and available only through bounded cache. No internet, npm install, prior Core checkout or producer conversation may be required for the package-contained path.

## Sigma Gate And Core Freeze

After Anchor machine/LLM acceptance, Sigma reviews representative real Core-produced Package V1 ZIPs from the human perspective, including at least:

- one simple/single route package;
- one multi-Workspace or multi-route package with bounded external cache and several pointer kinds.

If Sigma rejects structure/usability, return to Core while VS Code remains untouched.

If Sigma accepts both machine behavior and package shape, record a Core Package V1 freeze. Only then may VS Code implementation resume as Uppdrag 2.

## Uppdrag 2 — VS Code Thin Consumer (Later Only)

VS Code may call Core APIs, present Core-qualified candidates/results and supply explicit host capabilities. It may not recreate package semantics.

If the host needs information Core does not expose, stop and improve Core deliberately rather than adding a VS Code-private workaround.

## Scope

- Gate 0 purge continuity plus Uppdrag 1 direct Core + LLM Package V1 manufacture, orient, ground, cache/pointer resolution, physical ZIP, anti-drift, fresh-LLM and Sigma acceptance preparation.
- VS Code implementation remains out of scope until Core is accepted and frozen.

## Dependencies

- Exact carried Core, Business and Docs authority used by this Task.
- Existing Handoff Required Context / Relation authority unless a demonstrated package-only cache contract gap requires the bounded Docs change recorded by this Task.
- Sigma remains the final human Package V1 acceptance gate.

## Scope And Authority

- Anchor drives Gate 0 and Uppdrag 1 directly; no specialist implementation loop unless Sigma explicitly changes this Task.
- Core/portable Tooling and bounded App purge cleanup are authorized by this recovery.
- VS Code source remains unchanged during Uppdrag 1 except if an actual executable V2 remnant is discovered by evidence; the current scan found none.
- Business may change only for durable Task/Evidence/Handoff continuity needed to preserve this work.
- Docs semantics are not modified unless implementation proves a genuine unresolved semantic gap that cannot be represented through existing Handoff Required Context / Relation / artifact authority.
- No remote GitHub mutation, commit, push, release, publication, deployment or registry write is authorized.

## Done Criteria

This Task is complete only when:

- active Handoff Package V2/recipient-v2 machinery is removed from the organization-owned executable surfaces found by the purge scan;
- `sha256-base64url-c14n-v2` remains supported;
- direct Core Package V1 manufacture/orient/ground exists without a V2 intermediate or verifier;
- cache uses deterministic adapter-native readable paths and no generic binary/hash mapping architecture;
- generic grounding dependencies support required Role/process/policy/Handoff context through carried Workspace/cache and explicit read-only host/manual recovery;
- physical single/multi Package V1 black-box matrix is green;
- anti-drift mutation tests are green;
- fresh LLM cold-start acceptance is green;
- Sigma accepts representative ZIP shape/usability;
- Core is frozen before VS Code implementation resumes;
- final hermetic empty-workspace challenge passes after the later thin-host phase.

## Interpretation Limits

- This Task does not claim the current fail-closed purge candidate already implements Package V1.
- A green non-package Core suite after purge proves only that unrelated Core behavior survived removal; it is not Uppdrag 1 acceptance.
- Historical V2 provenance is not executable V2 support and should not be rewritten merely to erase history.
- Location, package membership, cache presence, filenames and pointer names do not create semantic authority.
- A connector/tool fetch receipt is material input evidence, not permission for remote mutation.
- Sigma acceptance remains the human gate; Anchor owns architectural coherence and machine/LLM acceptance preparation.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [040-anchor-to-kodax-tooling-major-008-capable-exact-lockfile-build-g.trace.md](handoffs/040-anchor-to-kodax-tooling-major-008-capable-exact-lockfile-build-g.trace.md)
  - Value: lzWqa8FGDwRQ54gm9nnwAX3keMBIn293VqG7NNo_uME

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: cwm2qeefTfhCOkCKDjeP68fuN9bFu1RF6zixit3RFP0
