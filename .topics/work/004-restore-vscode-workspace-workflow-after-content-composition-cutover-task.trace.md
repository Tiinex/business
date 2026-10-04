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
  - Created At: 2026-10-04 19:11:21
  - Authors: Anchor; Sigma
  - Why: Return the operator's standard VS Code workflow without requiring Sigma to debug host integration regressions.
  - Summary: Restore Replace, Initialize, shared host runtime composition, Local/Latest development switching, and multi-Workspace Pack after the content-source/schema cutover.
  - Status: ready/local

---

# Restore VS Code Workspace Workflow After Content Composition Cutover

## Objective

Restore the ordinary VS Code operator workflow after the Core/Native content-source and schema-authority cutover so a human operator can again receive a Handoff Package, bind its Workspaces to already-open local repositories, initialize a missing primary Workspace entrypoint, and manufacture the next carrier without becoming the debugger.

The implementation is considered an Anchor candidate only after the actual host/CLI chain can be completed, not merely after unit-level behavior appears correct.

## Observed Regression

The post-cutover VS Code host could lose the same content/runtime composition used by Core Tooling across different host paths. The user-visible consequences included:

- Replace no longer recognizing an already-open matching local Workspace and instead asking the operator to locate/open a folder.
- Initialize Workspace blocking when the direct primary Workspace entrypoint was missing.
- diagnostics using a different Core/content binding than Replace or Initialize.
- local development switching only Core while leaving the broader Tiinex content/dependency composition mixed between local and published material.
- successful package manufacture being vulnerable to a Windows temporary-directory cleanup race reporting the overall operation as failed.

## Candidate Changes

- Use one shared host Core/content runtime boundary for Diagnostics, Replace, Initialize, Incoming, Outgoing, and Pack.
- Preserve open Workspace roots as candidate content sources and compose them with dependency-mode content roots instead of dropping them when Local Core is selected.
- Treat an ordinary non-Git VS Code Workspace root as a valid host location for local-directory diagnostics; Git repository presence is not a prerequisite for Tiinex Workspace qualification.
- Keep Workspace identity authoritative: Replace rediscovers and qualifies the already-open local Workspace through Core rather than inferring equivalence from repository layout or asking for a folder when an exact qualified candidate is already available.
- Initialize Workspace continues to support:
  - no Git -> local-directory;
  - Git without origin -> local-directory with repository-without-origin state;
  - Git with origin -> repository-backed github-tree identity.
- If only nested `.workspaces` discovery surfaces remain, Initialize creates a new direct primary under `.topics/.workspaces`; nested surfaces remain valid and discoverable but do not become primary merely because they exist.
- `Tiinex: Switch all to Local` and `Tiinex: Switch all to Latest` are real VS Code development tasks for the Tiinex dependency/content composition rather than aliases for Core-only switching.
- Local/latest switching is graph/content-source driven and does not introduce Core -> Native source dependencies or package-name special cases in Core.
- `Tiinex: Build linked extension` keeps its existing task contract: `Tiinex: npm install` preserves the selected dependency mode, then `dev:build` runs normally.
- Disposable Windows scratch cleanup retries and remains best-effort after a successful qualified/published carrier so `ENOTEMPTY` cannot mask success.

## Anchor Machine Acceptance

The current candidate passed one host-level acceptance chain using the actual VS Code TypeScript adapters and shared Core Tooling:

1. Dependency-mode dry-run proved `all-local` selects local Core plus local registered Tiinex content packages and `all-latest` restores the same composition to published/latest package references.
2. The `Tiinex: Build linked extension` task definition remained unchanged and still depends on `Tiinex: npm install`, which preserves the selected dependency mode.
3. Initialize passed for no Git, Git without origin, and Git with origin.
4. Initialize recreated a direct primary `.topics/.workspaces` entrypoint when only a nested `.workspaces` surface remained.
5. Replace automatically rediscovered and qualified the already-open real `app` Workspace without a folder prompt.
6. Editor assistance/diagnostics projected the Business Workspace through the composed Local Core + Native schema content runtime with qualified exact validation and no diagnostics.
7. The actual VS Code host package builder manufactured a pointerless carrier from `app`, `core`, `interop-openai`, and `native`; shared Core oriented it as ready with a valid bootstrap and no error findings.
8. The produced carrier passed physical ZIP extraction/repack and re-oriented as ready with the same four Workspaces.

The current execution environment could not complete a real npm registry install/build because `registry.npmjs.org` resolution returned `EAI_AGAIN`. This is an environment limitation, not treated as a Build pass or a product failure. The Build task shape and dependency-mode install contract were verified, and the real linked-extension build remains one bounded Sigma platform observation.

## Dependencies

- [Grounding And Continuity Readiness](.topics/initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- Current VS Code Workspace candidate carried by the resulting Handoff Package.
- Current Core and Native content/runtime composition used by VS Code Tooling.
- Existing portable Session Grounding And Continuity and Tiinex recipient-transfer discipline.

## Scope

- Restore the standard VS Code Workspace Replace/Initialize/Pack workflow.
- Restore coherent Local/Latest development composition for the relevant Tiinex package/content dependency graph.
- Preserve existing linked-extension build semantics.
- Add bounded durable regression coverage for dependency-mode switching, Workspace initialization source forms, primary recreation, Replace qualification, and shared diagnostics runtime selection.
- Transfer only the smallest remaining Windows/VS Code-host observations to Sigma after Anchor completes machine acceptance.

## Done Criteria

- Replace automatically offers an already-open exact qualified local Workspace when its Workspace identity matches the incoming selection; normal matching does not require a folder picker.
- Initialize creates a qualified direct primary Workspace artifact when primary is missing and preserves support for no Git, Git/no origin, and Git+origin source identities.
- Diagnostics, Replace, Initialize, Incoming, Outgoing, and Pack use the same composed host runtime boundary.
- `Switch all to Local` and `Switch all to Latest` switch the intended Tiinex dependency/content composition without requiring npm publication of local development changes.
- `Build linked extension` retains its existing task contract and can operate under the selected dependency mode in the real Windows development environment.
- Normal multi-Workspace Pack succeeds and a post-success Windows scratch cleanup race cannot convert that success into a false failure.
- Sigma can perform the remaining real-host observations without debugging implementation.

## Boundaries

- This repair does not make repository identity a substitute for Workspace identity.
- Nested registered `.workspaces` surfaces remain valid; the direct `.topics/.workspaces` coordinate is a conventional primary selection surface, not the only legal Workspace discovery location.
- Local dependency composition does not make Core depend on Native or any named first-party content package.
- Anchor's machine acceptance does not substitute for the remaining real Windows/VS Code linked-extension observation.
- No commit, push, publication, release, or other remote mutation is authorized by this Task.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: XPw_cPI3DeINAWZyiCLfjQo3AeUkDQt4wG-k13QofaQ