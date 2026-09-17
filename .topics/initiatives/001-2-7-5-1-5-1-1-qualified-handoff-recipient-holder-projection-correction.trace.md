# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-16 12:52:29
  - Trace: [001-2-7-5-1-5-1-downstream-delegate-selection-projection-correction.trace.md](001-2-7-5-1-5-1-downstream-delegate-selection-projection-correction.trace.md)
  - Origin:
    - [relative](001-2-7-5-1-5-1-downstream-delegate-selection-projection-correction.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-16 20:10:02
  - Authors: Anchor
  - Why: Fresh Master Anchor and fresh Loom both recovered correctly but had to self-supply explicit session holder binding because normal grounding does not yet consume canonical handoff assignment authority.
  - Summary: Project bounded holder assignment from exact selected qualified Handoff consumption when the recipient Role authorizes the canonical handoff mode.
  - Status: ready/local

---

# Qualified Handoff Recipient Holder Projection Correction

## Objective

Remove the remaining fresh-cold-start friction in canonical holder grounding without restoring chat acknowledgements, self-binding heuristics, transport inference, or legacy Role mappings.

Current canonical Roles already authorize the `handoff` assignment mode, and the accepted Axiom holder semantics already define that mode as a bounded Role assignment established through exact qualified Handoff-bounded assignment authority. Real fresh Master Anchor and fresh Loom runs nevertheless required the consuming model to inject `--holder-role <Role>` itself because normal `ground` projects only `explicit-session` input and does not project the selected qualified Handoff consumption as bounded holder-assignment evidence.

The desired human-first behavior is that a recipient can consume one exact qualified selected Handoff route and become boundedly assigned to that Handoff's qualified recipient Role when, and only when, the exact Role authorizes `handoff`. No conversational acknowledgement line should be required.

## Done Criteria

- Normal `ground <package> --route <selected-route>` reaches act-ready holder binding without `--holder-role` when all of these are true: the selected route and Handoff qualify; the Handoff recipient is exactly one qualified Role; exact recipient Role material qualifies; that Role's canonical `Assignment Modes` includes `handoff`; and the current Tooling invocation is actively consuming that exact selected route.
- The positive holder projection is attributed to an exact bounded Handoff-consumption basis, not to package delivery, ZIP recipient, Handoff endpoint presence alone, filename, provider/model/chat identity, Role cache presence, or current assistant position.
- The holder projection records exact Handoff path/digest, selected route pointer, exact recipient Role path/digest/schema, canonical assignment mode `handoff`, and the bounded consumption basis.
- The result establishes only bounded current-session Role assignment for this selected Handoff. It does not establish durable Party/model identity, participant membership, delegation authority, process applicability, implementation-source authority, completion, acceptance beyond taking the bounded work, or wider organizational membership.
- A Role recipient whose exact canonical Assignment Modes does not include `handoff` remains discussion-only unless another independently qualified assignment mechanism is supplied.
- A merely carried/cached Role, an unselected sibling Handoff, orientation/package delivery without selected-route grounding, a mismatched recipient, ambiguous/unqualified recipient material, or missing exact Role material must not establish holder binding.
- Existing explicit assignment inputs remain supported as a separate mechanism; explicit mismatches continue to fail closed and must not be silently repaired by Handoff assignment.
- No prose parsing, Role-name/path whitelist, provider/chat special case, durable identity invention, new holder schema family, or legacy positive authorization path is introduced.
- The existing canonical holder, downstream-delegate, blank/minimal Workspace and full Core regressions remain green; add real carrier regressions covering fresh Anchor and fresh Loom shapes with no `--holder-role` input.
- Loom returns qualified Evidence and one Loom-to-Anchor Handoff. If exact existing Axiom/Role/Handoff semantics cannot support the bounded consumption evidence above without semantic invention, Loom must fail closed and return that exact semantic blocker rather than broaden Core locally.

## Scope

Core holder-binding projection for exact selected qualified Handoff consumption plus focused/adversarial regressions. No Business Role rewrite, no Docs schema/semantic rewrite, no delegation redesign, no product work, no durable identity system, and no general acceptance workflow.

## Dependencies

- Axiom `Canonical Holder Assignment Mode Semantic Disposition`, especially canonical `handoff` mode and Handoff isolation.
- Current `tiinex.party.role.v1` contract requiring exact qualified Handoff-bounded assignment evidence rather than endpoint/package-recipient inference.
- Canonical active Anchor and Loom Roles carrying direct `Assignment Modes` including `handoff`.
- Loom `Downstream Delegate Selection Projection Qualification` and its fresh return.
- Black-box fresh Master Anchor and fresh Loom runs that both recovered the correct frontier but had to self-supply explicit session holder binding because normal grounding did not project a Handoff-mode binding.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-2-7-5-1-5-1-downstream-delegate-selection-projection-correction.trace.md](001-2-7-5-1-5-1-downstream-delegate-selection-projection-correction.trace.md)
  - Value: yCIqwxGqU4bka7SwoGorNSXFIEWAv_qdzbkyfRgQlCo

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 7vWcdLQcpOjLT77Z0oNWSbHHTqAJsK9rOkyM02BmsWQ