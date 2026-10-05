# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-10-04 02:20:00
  - Trace: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Origin:
    - [relative](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-05 01:26:02
  - Authors: Anchor; Sigma
  - Why: Keep the build contract portable while distinguishing required published dependencies from optional registered content sources.
  - Summary: Make Local/Latest linked builds reusable npm flows and let Latest omit genuinely unpublished optional content sources without falling back to Local bytes.
  - Status: ready/local

---

# Make Local And Latest Linked Builds Portable NPM Flows

## Objective

Repair the linked-build shortcuts by making Local/Latest composition reusable npm flows instead of VS Code-only task choreography, while keeping Latest truthful when optional Tiinex content sources have not yet been published to npm.

The existing neutral linked build remains unchanged.

## Observed Regressions

Two related regressions were observed during Sigma acceptance:

1. VS Code hid `Tiinex: Build linked extension (Local)` when Local and Latest were both npm tasks targeting the same `dev:build` script. Distinct labels were not sufficient because VS Code deduplicated the underlying task definitions.
2. After moving Local/Latest composition into distinct npm scripts, `all-latest` attempted to install every registered Tiinex content source as `<package>@latest`. `@tiinex/interop-openai` is not currently published in the npm registry, so the Latest build failed with npm `E404` even though OpenAI interop is a registered optional content source rather than a required extension dependency.

## Candidate Change

### Portable build scripts

Add two explicit package scripts:

- `dev:build:local`: `node scripts/core-mode.mjs all-local && npm run dev:build`
- `dev:build:latest`: `node scripts/core-mode.mjs all-latest && npm run dev:build`

Expose those scripts through distinct VS Code npm tasks:

- `Tiinex: Build linked extension (Local)` -> `dev:build:local`
- `Tiinex: Build linked extension (Latest)` -> `dev:build:latest`

Keep `Tiinex: Build linked extension` -> `dev:build` unchanged.

### Latest dependency/content-source boundary

`all-latest` now distinguishes declared package dependencies from registered Tiinex content sources:

- declared Tiinex dependencies remain required and are installed as `@latest`; their installation remains fail-closed;
- each registered content source is probed for an actual npm `latest` version;
- a published content source is installed as `@latest`;
- an npm `E404` / not-in-registry result means that optional content source is omitted from Latest rather than blocking the build;
- any stale Local installation/link for an omitted content source is explicitly removed so Latest never silently falls back to Local bytes;
- registry failures other than a qualified not-published result remain blocking rather than being misclassified as “unpublished”.

The dependency-mode state may retain the registered content-source identities, but the Latest runtime composes only packages actually materialized in `node_modules`. If a content source is published later, the same flow automatically starts installing its published `latest` version.

`all-local` remains unchanged: it composes the complete locally available Tiinex dependency/content-source surface from sibling checkouts.

## Acceptance Evidence

Anchor verified the repair with executable dependency-mode harnesses:

- when both Native and OpenAI Interop are reported as unpublished, `all-latest` installs required `@tiinex/core@latest`, removes stale Local Native/OpenAI links, omits both content sources, and completes successfully;
- when Native is reported as published but OpenAI Interop is unpublished, `all-latest` installs `@tiinex/native@latest`, omits/removes only OpenAI Interop, and still installs required Core latest;
- `all-local` continues to install `file:../core`, `file:../native`, and `file:../interop-openai` together;
- unavailable content sources are reported explicitly to the operator rather than hidden behind a local fallback;
- non-E404 registry failures remain errors.

The earlier dry-run could only prove generated package coordinates; it could not prove that those package names were actually published. This acceptance closes that gap with registry-result behavior rather than assuming publication from local package metadata.

## Scope

- VS Code extension `package.json` build-mode scripts.
- VS Code `.vscode/tasks.json` Local/Latest shortcut definitions.
- VS Code `scripts/core-mode.mjs` dependency-mode composition and registry-availability behavior.
- Focused executable acceptance of Local and Latest composition.

## Dependencies

- [Final VS Code Pre-Major Acceptance](014-final-vscode-pre-major-acceptance-task.trace.md)
- Existing Tiinex dependency-mode state and registered content-source convention.
- Existing neutral `dev:build` linked-extension build.

## Done Criteria

- All three build choices are independently visible to VS Code task discovery.
- `npm run dev:build:local` owns Local mode composition plus the existing build.
- `npm run dev:build:latest` owns Latest mode composition plus the existing build.
- Required Tiinex package dependencies use published `@latest` and remain fail-closed.
- Published registered content sources use `@latest`.
- Unpublished registered content sources do not block Latest and cannot remain as stale Local links.
- The neutral `npm run dev:build` path and `Tiinex: Build linked extension` remain unchanged.
- The flows are usable outside VS Code through npm and require no fake task/script differences.

## Boundaries

- No Core, carrier, Package V1, Workspace identity, Replace, Guided Entry, source-preset, or Major-allocation semantics change.
- “Latest” must not silently substitute Local bytes for an unavailable published content source.
- No remote mutation is authorized.
- Broader next-Major grounding/audit work remains deferred until stable acceptance.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: arLyKrZ3g2TBsSLPhYPwjkLCswnEE9ASW_eFAj_g4xE