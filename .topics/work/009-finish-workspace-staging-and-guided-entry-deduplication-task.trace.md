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
  - Created At: 2026-10-04 22:42:42
  - Authors: Anchor; Sigma
  - Why: Finish the remaining operator-facing deviations without reopening the repaired packaging and Workspace workflow.
  - Summary: Close the final Stage All command responsibility mismatch and byte-identical Guided Entry duplication before the stable Major.
  - Status: ready/local

---

# Finish Workspace Staging And Guided Entry Deduplication Before Stable Major

## Objective

Close the two remaining operator-facing deviations observed after the repaired VS Code/Core boundary acceptance without reopening accepted packaging, lineage, Workspace, Replace, Initialize, or source-selection behavior.

## Observed Deviations

1. The requested operator convenience was a simple `Stage all workspaces` action, but the available multi-repository command opened a Tiinex review/commit/push workflow. That is a different responsibility and forces unnecessary form interaction.
2. Guided Entry still exposed byte-identical Entry definitions more than once when the same exact representation was carried from multiple Workspace sources. The receiving operator should not need to choose between semantically and byte-identical representations.

## Candidate Changes

### Stage All Workspaces

- Add `Tiinex: Stage All Workspaces` as a first-class VS Code command.
- Enumerate the Git repositories already known by VS Code's Git API.
- Run the ordinary Git staging operation equivalent to `git add -A` once per repository.
- Do not perform Tiinex semantic qualification, review, commit-message generation, commit, or push.
- Clean repositories are harmless no-ops; one repository failure is reported as a bounded staging failure rather than opening a review workflow.
- The existing advanced review/commit/push workflow remains a separate command and does not define Stage All semantics.

### Guided Entry exact-byte deduplication

- Core remains the owner of Entry projection semantics.
- After read qualification and carried-lineage leaf selection, group qualified Entry representations by exact Markdown bytes.
- If byte-identical representations exist, select one deterministic representation.
- A carried/embedded representation wins over a reusable external/content-source copy.
- When multiple carried representations are byte-identical, preserve the first carried representation in qualified carrier order; the host does not invent a semantic preference.
- Non-identical representations remain distinct and are not collapsed merely because labels or canonical identifiers match.

## Acceptance Evidence

Anchor verified the candidate using focused behavior paths:

- `Stage All Workspaces` low-level Git seam invokes only `git add -A`.
- The real Git operation was executed over two independent temporary repositories; modified and untracked files became staged in both with no unstaged remainder.
- A real pointerless Workspace carrier containing byte-identical Explore/Resume/Start Entry material from Core-carried and Native-carried sources was manufactured.
- The repaired Core Guided Entry projection returned exactly one Explore, one Resume and one Start plus Custom; the deterministic carried Core representation won for the byte-identical candidates.
- Modified TypeScript files transpiled without syntax diagnostics and modified Core JavaScript parsed successfully.

## Full-Test Observation

Sigma's full silent-video acceptance of the preceding 008 candidate showed the previously blocking workflow restored: Handoff Markdown Preview was read-first, Incoming/qualified matches were usable, Parent/Local Outgoing selection was workable under the intended Mark All semantics, manufacture completed, and a 17-Workspace `022` Major carrier was produced. The remaining visible deviations were the staging-command responsibility mismatch and duplicate Guided Entry choices addressed by this Task.

## Parallel Audit Boundary

A parallel low-pre-context Anchor audit identifies Core ↔ host contract fragmentation and verification debt as the next structural priority. This Task does not start that broad work. It closes the last observed current-workflow deviations so the next stable Major can begin the grounding/boundary-verification continuation from a usable operator baseline.

## Scope

- One simple multi-repository stage command in the VS Code host.
- Core-owned exact-byte Entry projection deduplication for Guided Entry.
- Focused behavior acceptance only.

## Dependencies

- [Grounding And Continuity Readiness](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
- [Close VS Code Core Host Boundary Regressions Before Stable Major](008-close-vscode-core-host-boundary-regressions-task.trace.md)
- Current carried Core, VS Code, Native, and Business Workspaces.

## Done Criteria

- `Tiinex: Stage All Workspaces` stages every VS Code-known Git repository without opening repository-selection, review, commit, or push forms.
- The command performs no commit or push.
- Guided Entry does not show byte-identical Core/Native Entry duplicates.
- Exact-byte carried material wins deterministically and non-identical Entry material remains distinct.
- Existing Handoff Preview, Incoming matching, Outgoing selection, Pack, Major allocation, Replace and Initialize behavior are not reopened.
- Sigma can confirm the two visible fixes without debugging implementation.

## Boundaries

- No artifact-lineage, Parent ancestry, Workspace identity, carrier-lineage model, Package V1 topology, Major allocation, Replace, Initialize, or Outgoing source-selection semantics are changed.
- The broad audit work around Core↔host protocol consolidation, test-baseline migration, artifactTree ownership, operatorTrees decomposition, and Core primitive deduplication is explicitly deferred to the next Major.
- No commit, push, publication, release, deployment, or remote mutation is authorized by this Task.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [007-grounding-and-continuity-readiness-project.trace.md](../initiatives/007-grounding-and-continuity-readiness-project.trace.md)
  - Value: zUnREYS9Z7wds7wltbyds-e2-I-2sTpJokYXWTGH2QM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: ULM76gVrfi5htrSzvQuUf3WpJPM3fFmJrzu2OJdgw5c