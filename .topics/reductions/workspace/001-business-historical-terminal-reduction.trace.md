# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-03 09:37:17
  - Trace: [001-project-wide-lineage-reduction-and-survivor-repair-task.trace.md](../project/001-project-wide-lineage-reduction-and-survivor-repair-task.trace.md)
  - Origin:
    - [relative](../project/001-project-wide-lineage-reduction-and-survivor-repair-task.trace.md)
- Current
  - Current Schema: [tiinex.reduction.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/reduction/tiinex.reduction.v1.schema.md)
  - Created At: 2026-10-03 09:42:26
  - Authors: Anchor
  - Summary: Reduce the exact 56 Business artifacts lying exclusively on previously qualified terminal/superseded branches while preserving current frontier ancestry.
  - Status: ready/local

---

# Business Historical Terminal Branch Reduction

## Source Context

- Classification Authority: qualified Reduction Major 001 project-wide leaf classification, reconciled against the current carrier-015 graph.
- Candidate Derivation: walk each B5/B6 terminal anchor toward Parent while excluding the ancestor-closed set of every current/non-terminal leaf; this reproduced exactly 56 Business candidates.
- Immutable Pre-delete Snapshot: `Tiinex/business@148a05e37b29baff8cdbe1d73293cfca1de8f9c7`.
- Snapshot Qualification: the entire baseline carrier-015 Business `.topics` Git tree exactly matches the immutable repository `.topics` tree at this commit.
- Current Project Task: `.topics/reductions/project/001-project-wide-lineage-reduction-and-survivor-repair-task.trace.md` remains outside the candidate set.

## Carry-Forward State

- The surviving current/non-terminal Business leaves and their ancestor closure remain in the Workspace.
- Reduction Major 001 remains the historical classification authority for its B5/B6 terminal leaves; this Reduction applies that classification only where the current graph contains no surviving non-terminal dependency through the candidate branch.
- The new project-wide Reduction Task carries the active cleanup/repair frontier.
- Removed source bytes remain recoverable from the immutable Business snapshot above.

## Loss And Uncertainty

- Intentional Loss: 56 historical Business trace artifacts will leave current HEAD if destructive eligibility qualifies and the exact candidate set is applied.
- Preserved Recovery: every candidate path is listed above and bound to the immutable Business commit.
- Unresolved/current material is excluded by construction and remains for later classification or repair.
- This Reduction does not authorize deletion of any Business artifact outside the exact manifest.

## Validation

### Exact Reduced Candidate Manifest

- 1. [`.topics/business-development/002-1-1-anchor-to-sigma-lineage-projection-correction-retry-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/business-development/002-1-1-anchor-to-sigma-lineage-projection-correction-retry-handoff.trace.md)
- 2. [`.topics/business-development/002-1-anchor-to-sigma-business-major-checkpoint-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/business-development/002-1-anchor-to-sigma-business-major-checkpoint-handoff.trace.md)
- 3. [`.topics/business-development/002-anchor-foundation-tooling-closure-and-workflow-automation-task.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/business-development/002-anchor-foundation-tooling-closure-and-workflow-automation-task.trace.md)
- 4. [`.topics/business-development/003-anchor-to-anchor-foundation-reanchor-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/business-development/003-anchor-to-anchor-foundation-reanchor-handoff.trace.md)
- 5. [`.topics/initiatives/001-3-6-1-1-anchor-to-sigma-full-source-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-1-1-anchor-to-sigma-full-source-handoff.trace.md)
- 6. [`.topics/initiatives/001-3-6-1-extraction-checkpoint-evidence.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-1-extraction-checkpoint-evidence.trace.md)
- 7. [`.topics/initiatives/001-3-6-2-1-anchor-to-sigma-full-source-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-2-1-anchor-to-sigma-full-source-handoff.trace.md)
- 8. [`.topics/initiatives/001-3-6-2-extraction-qualification-evidence.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-2-extraction-qualification-evidence.trace.md)
- 9. [`.topics/initiatives/001-3-6-3-2-anchor-to-sigma-parity-source-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-3-2-anchor-to-sigma-parity-source-handoff.trace.md)
- 10. [`.topics/initiatives/refactor/extensions/handoffs/001-refactor-anchor-to-vs-code-anchor-current-shared-context-refresh.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/extensions/handoffs/001-refactor-anchor-to-vs-code-anchor-current-shared-context-refresh.trace.md)
- 11. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-after-glimmer-stream-delegation.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-after-glimmer-stream-delegation.trace.md)
- 12. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-glimmer-stream-7-audience-narration.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-to-glimmer-stream-7-audience-narration.trace.md)
- 13. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-recovery-after-kodax-pack-authoring-delegation.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-recovery-after-kodax-pack-authoring-delegation.trace.md)
- 14. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-successor-pack-fix-recovery.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-successor-pack-fix-recovery.trace.md)
- 15. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-refactor-anchor-successor-after-vscode-pack-dogfood.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-refactor-anchor-successor-after-vscode-pack-dogfood.trace.md)
- 16. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-2-1-sigma-pack-fix-full-source.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-2-1-sigma-pack-fix-full-source.trace.md)
- 17. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-2-anchor-to-sigma-full-source-mega-replace.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-2-anchor-to-sigma-full-source-mega-replace.trace.md)
- 18. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-refactor-recovery-after-vs-code-emergency-wip-and-kodax-delegati.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-refactor-recovery-after-vs-code-emergency-wip-and-kodax-delegati.trace.md)
- 19. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-refactor-recovery-after-vs-code-native-operator-audit.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-refactor-recovery-after-vs-code-native-operator-audit.trace.md)
- 20. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-refactor-recovery-after-source-frontier-comparison-acceptance.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-refactor-recovery-after-source-frontier-comparison-acceptance.trace.md)
- 21. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-refactor-recovery-after-source-frontier-comparison-delegation.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-refactor-recovery-after-source-frontier-comparison-delegation.trace.md)
- 22. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-refactor-recovery-after-secure-transport-cli-headless-acceptance.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-refactor-recovery-after-secure-transport-cli-headless-acceptance.trace.md)
- 23. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-refactor-recovery-after-secure-transport-core-conformance-accept.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-refactor-recovery-after-secure-transport-core-conformance-accept.trace.md)
- 24. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-refactor-recovery-after-axiom-secure-transport-profile-review.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-refactor-recovery-after-axiom-secure-transport-profile-review.trace.md)
- 25. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-refactor-recovery-after-secure-transport-core-acceptance.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-refactor-recovery-after-secure-transport-core-acceptance.trace.md)
- 26. [`.topics/initiatives/refactor/handoffs/001-1-1-1-1-refactor-recovery-after-secure-transport-docs-acceptance.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-refactor-recovery-after-secure-transport-docs-acceptance.trace.md)
- 27. [`.topics/initiatives/refactor/handoffs/001-1-1-1-refactor-anchor-conversation-successor-and-recovery-checkpoint.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-refactor-anchor-conversation-successor-and-recovery-checkpoint.trace.md)
- 28. [`.topics/initiatives/refactor/handoffs/001-1-1-anchor-to-sigma-cli-establishment-and-post-landing-reconciliatio.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-anchor-to-sigma-cli-establishment-and-post-landing-reconciliatio.trace.md)
- 29. [`.topics/initiatives/refactor/handoffs/001-1-anchor-to-sigma-renamed-repositories-and-runtime-bootstrap-progr.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-anchor-to-sigma-renamed-repositories-and-runtime-bootstrap-progr.trace.md)
- 30. [`.topics/initiatives/refactor/handoffs/001-anchor-to-sigma-turn-2-commitable-full-source-progression.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-anchor-to-sigma-turn-2-commitable-full-source-progression.trace.md)
- 31. [`.topics/initiatives/refactor/handoffs/002-anchor-full-recovery-after-stream-orchestration-and-playthings-d.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/002-anchor-full-recovery-after-stream-orchestration-and-playthings-d.trace.md)
- 32. [`.topics/initiatives/refactor/handoffs/003-anchor-full-recovery-after-stream-orchestration-playthings-and-v.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/003-anchor-full-recovery-after-stream-orchestration-playthings-and-v.trace.md)
- 33. [`.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-1-loom-to-anchor-carrier-major-002-lineage-safety-hardening-return.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-1-loom-to-anchor-carrier-major-002-lineage-safety-hardening-return.trace.md)
- 34. [`.topics/initiatives/refactor/handoffs/004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-2-anchor-full-recovery-after-loom-route-leaf-correction.trace.md)
- 35. [`.topics/initiatives/refactor/orchestration/chrome/001-extension-chrome-carrier-major-002-bounded-operator-automation-foundation.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/chrome/001-extension-chrome-carrier-major-002-bounded-operator-automation-foundation.trace.md)
- 36. [`.topics/initiatives/refactor/orchestration/handoffs/001-1-anchor-to-playthings-carrier-major-001-refactor-reality-check.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/001-1-anchor-to-playthings-carrier-major-001-refactor-reality-check.trace.md)
- 37. [`.topics/initiatives/refactor/orchestration/handoffs/001-anchor-to-playthings-anchor-carrier-major-001-refactor-reality-c.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/001-anchor-to-playthings-anchor-carrier-major-001-refactor-reality-c.trace.md)
- 38. [`.topics/initiatives/refactor/orchestration/handoffs/002-anchor-to-kodax-vs-code-carrier-major-001-operator-trust-and-erg.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/002-anchor-to-kodax-vs-code-carrier-major-001-operator-trust-and-erg.trace.md)
- 39. [`.topics/initiatives/refactor/orchestration/handoffs/003-anchor-to-kodax-viewer-carrier-major-002-poc-replacement-reconci.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/003-anchor-to-kodax-viewer-carrier-major-002-poc-replacement-reconci.trace.md)
- 40. [`.topics/initiatives/refactor/orchestration/handoffs/004-anchor-to-prism-verse-playthings-carrier-major-002-browser-reali.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/004-anchor-to-prism-verse-playthings-carrier-major-002-browser-reali.trace.md)
- 41. [`.topics/initiatives/refactor/orchestration/handoffs/005-anchor-to-kodax-extension-vs-code-carrier-major-002-operator-com.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/005-anchor-to-kodax-extension-vs-code-carrier-major-002-operator-com.trace.md)
- 42. [`.topics/initiatives/refactor/orchestration/handoffs/006-anchor-to-glimmer-stream-audience-grounding-refresh.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/006-anchor-to-glimmer-stream-audience-grounding-refresh.trace.md)
- 43. [`.topics/initiatives/refactor/orchestration/handoffs/007-anchor-full-recovery-carrier-major-002-parallel-lanes-after-rout.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/007-anchor-full-recovery-carrier-major-002-parallel-lanes-after-rout.trace.md)
- 44. [`.topics/initiatives/refactor/orchestration/handoffs/008-1-kodax-to-anchor-extension-chrome-carrier-major-002-bounded-opera.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/008-1-kodax-to-anchor-extension-chrome-carrier-major-002-bounded-opera.trace.md)
- 45. [`.topics/initiatives/refactor/orchestration/handoffs/008-anchor-to-kodax-extension-chrome-carrier-major-002-bounded-automation.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/008-anchor-to-kodax-extension-chrome-carrier-major-002-bounded-automation.trace.md)
- 46. [`.topics/initiatives/refactor/orchestration/handoffs/009-1-1-anchor-full-recovery-carrier-major-002-after-loom-lineage-safety.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/009-1-1-anchor-full-recovery-carrier-major-002-after-loom-lineage-safety.trace.md)
- 47. [`.topics/initiatives/refactor/orchestration/handoffs/009-1-anchor-full-recovery-accepted-prism-and-chrome-returns.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/009-1-anchor-full-recovery-accepted-prism-and-chrome-returns.trace.md)
- 48. [`.topics/initiatives/refactor/orchestration/handoffs/009-anchor-full-recovery-carrier-major-002-after-chrome-lane-launch.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/009-anchor-full-recovery-carrier-major-002-after-chrome-lane-launch.trace.md)
- 49. [`.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-site005-return-sigma-browser-gate.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-site005-return-sigma-browser-gate.trace.md)
- 50. [`.topics/initiatives/refactor/orchestration/handoffs/011-anchor-full-recovery-authoring-accepted-grounding-hardening-acti.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/011-anchor-full-recovery-authoring-accepted-grounding-hardening-acti.trace.md)
- 51. [`.topics/processes/gpt/grounding/001-1-2-1-1-2-anchor-to-anchor-standard-successor-grounding-acceptance-return.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-1-1-2-anchor-to-anchor-standard-successor-grounding-acceptance-return.trace.md)
- 52. [`.topics/processes/gpt/grounding/001-1-2-2-1-2-fresh-anchor-to-anchor-perturbed-successor-grounding-acceptance.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-2-1-2-fresh-anchor-to-anchor-perturbed-successor-grounding-acceptance.trace.md)
- 53. [`.topics/processes/gpt/grounding/001-1-2-4-1-2-anchor-to-anchor-coverage-corrected-standard-successor-return.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-1-2-anchor-to-anchor-coverage-corrected-standard-successor-return.trace.md)
- 54. [`.topics/processes/gpt/grounding/001-1-2-4-2-2-anchor-to-anchor-coverage-corrected-perturbed-successor-return.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-2-2-anchor-to-anchor-coverage-corrected-perturbed-successor-return.trace.md)
- 55. [`.topics/processes/gpt/grounding/001-1-2-4-5-1-anchor-to-anchor-selector-isolated-standard-successor-replay-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-5-1-anchor-to-anchor-selector-isolated-standard-successor-replay-handoff.trace.md)
- 56. [`.topics/processes/gpt/grounding/001-1-2-4-5-fresh-anchor-selector-isolated-standard-replay-task.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-5-fresh-anchor-selector-isolated-standard-replay-task.trace.md)

### Reduced Leaves / Expansion Boundary

- **Leaf 1**
  - Leaf: [.topics/business-development/002-1-1-anchor-to-sigma-lineage-projection-correction-retry-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/business-development/002-1-1-anchor-to-sigma-lineage-projection-correction-retry-handoff.trace.md)
  - Collapse To: [.topics/business-development/001-business-development-project.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/business-development/001-business-development-project.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 2**
  - Leaf: [.topics/business-development/003-anchor-to-anchor-foundation-reanchor-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/business-development/003-anchor-to-anchor-foundation-reanchor-handoff.trace.md)
  - Collapse To: [.topics/initiatives/001-6-foundation-readiness-operating-reconciliation-task.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-6-foundation-readiness-operating-reconciliation-task.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 3**
  - Leaf: [.topics/initiatives/001-3-6-1-1-anchor-to-sigma-full-source-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-1-1-anchor-to-sigma-full-source-handoff.trace.md)
  - Collapse To: [.topics/initiatives/001-3-6-core-app-site-extraction-task.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-core-app-site-extraction-task.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 4**
  - Leaf: [.topics/initiatives/001-3-6-2-1-anchor-to-sigma-full-source-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-2-1-anchor-to-sigma-full-source-handoff.trace.md)
  - Collapse To: [.topics/initiatives/001-3-6-core-app-site-extraction-task.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-core-app-site-extraction-task.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 5**
  - Leaf: [.topics/initiatives/001-3-6-3-2-anchor-to-sigma-parity-source-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-3-2-anchor-to-sigma-parity-source-handoff.trace.md)
  - Collapse To: [.topics/initiatives/001-3-6-3-playthings-parity-master-publishing-task.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-3-playthings-parity-master-publishing-task.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 6**
  - Leaf: [.topics/initiatives/refactor/extensions/handoffs/001-refactor-anchor-to-vs-code-anchor-current-shared-context-refresh.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/extensions/handoffs/001-refactor-anchor-to-vs-code-anchor-current-shared-context-refresh.trace.md)
  - Collapse To: [.topics/initiatives/refactor/extensions/001-extension-repository-frontier.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/extensions/001-extension-repository-frontier.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 7**
  - Leaf: [.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-after-glimmer-stream-delegation.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-after-glimmer-stream-delegation.trace.md)
  - Collapse To: [.topics/initiatives/refactor/001-turn-2-stable-full-source-frontier.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/001-turn-2-stable-full-source-frontier.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 8**
  - Leaf: [.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-2-1-sigma-pack-fix-full-source.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/001-1-1-1-1-1-1-1-1-1-1-1-1-2-1-sigma-pack-fix-full-source.trace.md)
  - Collapse To: [.topics/initiatives/refactor/001-turn-2-stable-full-source-frontier.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/001-turn-2-stable-full-source-frontier.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 9**
  - Leaf: [.topics/initiatives/refactor/handoffs/002-anchor-full-recovery-after-stream-orchestration-and-playthings-d.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/002-anchor-full-recovery-after-stream-orchestration-and-playthings-d.trace.md)
  - Collapse To: [.topics/initiatives/refactor/orchestration/001-stream-day-parallel-major-001-orchestration.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/001-stream-day-parallel-major-001-orchestration.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 10**
  - Leaf: [.topics/initiatives/refactor/handoffs/003-anchor-full-recovery-after-stream-orchestration-playthings-and-v.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/003-anchor-full-recovery-after-stream-orchestration-playthings-and-v.trace.md)
  - Collapse To: [.topics/initiatives/refactor/orchestration/vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 11**
  - Leaf: [.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-1-loom-to-anchor-carrier-major-002-lineage-safety-hardening-return.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-1-loom-to-anchor-carrier-major-002-lineage-safety-hardening-return.trace.md)
  - Collapse To: [.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-anchor-to-loom-carrier-major-002-lineage-safety-hardening-retry.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-anchor-to-loom-carrier-major-002-lineage-safety-hardening-retry.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 12**
  - Leaf: [.topics/initiatives/refactor/orchestration/handoffs/003-anchor-to-kodax-viewer-carrier-major-002-poc-replacement-reconci.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/003-anchor-to-kodax-viewer-carrier-major-002-poc-replacement-reconci.trace.md)
  - Collapse To: [.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 13**
  - Leaf: [.topics/initiatives/refactor/orchestration/handoffs/004-anchor-to-prism-verse-playthings-carrier-major-002-browser-reali.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/004-anchor-to-prism-verse-playthings-carrier-major-002-browser-reali.trace.md)
  - Collapse To: [.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 14**
  - Leaf: [.topics/initiatives/refactor/orchestration/handoffs/005-anchor-to-kodax-extension-vs-code-carrier-major-002-operator-com.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/005-anchor-to-kodax-extension-vs-code-carrier-major-002-operator-com.trace.md)
  - Collapse To: [.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 15**
  - Leaf: [.topics/initiatives/refactor/orchestration/handoffs/006-anchor-to-glimmer-stream-audience-grounding-refresh.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/006-anchor-to-glimmer-stream-audience-grounding-refresh.trace.md)
  - Collapse To: [.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 16**
  - Leaf: [.topics/initiatives/refactor/orchestration/handoffs/008-1-kodax-to-anchor-extension-chrome-carrier-major-002-bounded-opera.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/008-1-kodax-to-anchor-extension-chrome-carrier-major-002-bounded-opera.trace.md)
  - Collapse To: [.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 17**
  - Leaf: [.topics/initiatives/refactor/orchestration/handoffs/009-1-1-anchor-full-recovery-carrier-major-002-after-loom-lineage-safety.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/009-1-1-anchor-full-recovery-carrier-major-002-after-loom-lineage-safety.trace.md)
  - Collapse To: [.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 18**
  - Leaf: [.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-site005-return-sigma-browser-gate.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-1-anchor-full-recovery-site005-return-sigma-browser-gate.trace.md)
  - Collapse To: [.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-anchor-full-recovery-vscode0031-site005-launch.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-anchor-full-recovery-vscode0031-site005-launch.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 19**
  - Leaf: [.topics/initiatives/refactor/orchestration/handoffs/011-anchor-full-recovery-authoring-accepted-grounding-hardening-acti.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/011-anchor-full-recovery-authoring-accepted-grounding-hardening-acti.trace.md)
  - Collapse To: [.topics/processes/gpt/grounding/002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 20**
  - Leaf: [.topics/processes/gpt/grounding/001-1-2-1-1-2-anchor-to-anchor-standard-successor-grounding-acceptance-return.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-1-1-2-anchor-to-anchor-standard-successor-grounding-acceptance-return.trace.md)
  - Collapse To: [.topics/processes/gpt/grounding/001-1-2-1-1-anchor-to-anchor-standard-successor-grounding-acceptance-correction-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-1-1-anchor-to-anchor-standard-successor-grounding-acceptance-correction-handoff.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 21**
  - Leaf: [.topics/processes/gpt/grounding/001-1-2-2-1-2-fresh-anchor-to-anchor-perturbed-successor-grounding-acceptance.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-2-1-2-fresh-anchor-to-anchor-perturbed-successor-grounding-acceptance.trace.md)
  - Collapse To: [.topics/processes/gpt/grounding/001-1-2-2-1-anchor-to-anchor-perturbed-successor-grounding-acceptance-correction-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-2-1-anchor-to-anchor-perturbed-successor-grounding-acceptance-correction-handoff.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 22**
  - Leaf: [.topics/processes/gpt/grounding/001-1-2-4-1-2-anchor-to-anchor-coverage-corrected-standard-successor-return.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-1-2-anchor-to-anchor-coverage-corrected-standard-successor-return.trace.md)
  - Collapse To: [.topics/processes/gpt/grounding/001-1-2-4-1-anchor-to-anchor-coverage-corrected-standard-successor-probe-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-1-anchor-to-anchor-coverage-corrected-standard-successor-probe-handoff.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 23**
  - Leaf: [.topics/processes/gpt/grounding/001-1-2-4-2-2-anchor-to-anchor-coverage-corrected-perturbed-successor-return.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-2-2-anchor-to-anchor-coverage-corrected-perturbed-successor-return.trace.md)
  - Collapse To: [.topics/processes/gpt/grounding/001-1-2-4-2-anchor-to-anchor-coverage-corrected-perturbed-successor-probe-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-2-anchor-to-anchor-coverage-corrected-perturbed-successor-probe-handoff.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

- **Leaf 24**
  - Leaf: [.topics/processes/gpt/grounding/001-1-2-4-5-1-anchor-to-anchor-selector-isolated-standard-successor-replay-handoff.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-5-1-anchor-to-anchor-selector-isolated-standard-successor-replay-handoff.trace.md)
  - Collapse To: [.topics/processes/gpt/grounding/001-1-2-4-fresh-anchor-successor-acceptance-coverage-corrected-replay-task.trace.md](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-fresh-anchor-successor-acceptance-coverage-corrected-replay-task.trace.md)
  - Disposition: `terminal-or-superseded-historical`
  - Why: Reduction Major 001 classifies the controlling branch as B5/B6 terminal/superseded and current graph reconciliation leaves no surviving non-terminal dependency inside this candidate span.
  - Expansion Span: exact Parent span from this disappearing leaf through the declared candidate set to the nearest surviving Business boundary

### Surviving Closure Endpoints

- [`.topics/business-development/001-business-development-project.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/business-development/001-business-development-project.trace.md)
- [`.topics/initiatives/001-3-6-3-playthings-parity-master-publishing-task.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-3-playthings-parity-master-publishing-task.trace.md)
- [`.topics/initiatives/001-3-6-core-app-site-extraction-task.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-3-6-core-app-site-extraction-task.trace.md)
- [`.topics/initiatives/001-6-foundation-readiness-operating-reconciliation-task.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/001-6-foundation-readiness-operating-reconciliation-task.trace.md)
- [`.topics/initiatives/refactor/001-turn-2-stable-full-source-frontier.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/001-turn-2-stable-full-source-frontier.trace.md)
- [`.topics/initiatives/refactor/extensions/001-extension-repository-frontier.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/extensions/001-extension-repository-frontier.trace.md)
- [`.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-anchor-to-loom-carrier-major-002-lineage-safety-hardening-retry.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-1-anchor-to-loom-carrier-major-002-lineage-safety-hardening-retry.trace.md)
- [`.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/handoffs/004-1-1-1-1-anchor-full-recovery-after-carrier-major-002-loom-lineage-safety.trace.md)
- [`.topics/initiatives/refactor/orchestration/001-stream-day-parallel-major-001-orchestration.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/001-stream-day-parallel-major-001-orchestration.trace.md)
- [`.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-anchor-full-recovery-vscode0031-site005-launch.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/handoffs/010-1-1-1-1-1-1-1-1-1-anchor-full-recovery-vscode0031-site005-launch.trace.md)
- [`.topics/initiatives/refactor/orchestration/vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/initiatives/refactor/orchestration/vscode/001-vs-code-carrier-major-001-operator-trust-and-ergonomics.trace.md)
- [`.topics/processes/gpt/grounding/001-1-2-1-1-anchor-to-anchor-standard-successor-grounding-acceptance-correction-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-1-1-anchor-to-anchor-standard-successor-grounding-acceptance-correction-handoff.trace.md)
- [`.topics/processes/gpt/grounding/001-1-2-2-1-anchor-to-anchor-perturbed-successor-grounding-acceptance-correction-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-2-1-anchor-to-anchor-perturbed-successor-grounding-acceptance-correction-handoff.trace.md)
- [`.topics/processes/gpt/grounding/001-1-2-4-1-anchor-to-anchor-coverage-corrected-standard-successor-probe-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-1-anchor-to-anchor-coverage-corrected-standard-successor-probe-handoff.trace.md)
- [`.topics/processes/gpt/grounding/001-1-2-4-2-anchor-to-anchor-coverage-corrected-perturbed-successor-probe-handoff.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-2-anchor-to-anchor-coverage-corrected-perturbed-successor-probe-handoff.trace.md)
- [`.topics/processes/gpt/grounding/001-1-2-4-fresh-anchor-successor-acceptance-coverage-corrected-replay-task.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/001-1-2-4-fresh-anchor-successor-acceptance-coverage-corrected-replay-task.trace.md)
- [`.topics/processes/gpt/grounding/002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md`](https://github.com/Tiinex/business/blob/148a05e37b29baff8cdbe1d73293cfca1de8f9c7/.topics/processes/gpt/grounding/002-anchor-grounding-recovery-and-recipient-projection-hardening.trace.md)

- Baseline carrier-015 Business `.topics` tree SHA matched immutable Git tree SHA `ffbcbe625f824af1cb16cda8dda699c0b3ea3e9f`.
- Rebuilt project prune projection reproduced the same 56 Business candidates recovered before the sandbox reset.
- Candidate closure resolves to 17 surviving Business endpoints.
- Destructive apply remains gated by Core `reduction-preflight`; the Reduction itself is not deletion authority.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-project-wide-lineage-reduction-and-survivor-repair-task.trace.md](../project/001-project-wide-lineage-reduction-and-survivor-repair-task.trace.md)
  - Value: 3rSxxVEUc3iIPBmND7UP-pvCcsyKr-wGQojfunOWiFo

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: QNYJ9GmiyXDNW29loVCtDfC0ueqYQscWZieIGMIiEVc