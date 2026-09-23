# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-09-22 15:23:19
  - Trace: [026-anchor-to-kodax-tooling-major-008-native-vs-code-handoff-ux.trace.md](handoffs/026-anchor-to-kodax-tooling-major-008-native-vs-code-handoff-ux.trace.md)
  - Origin:
    - [relative](handoffs/026-anchor-to-kodax-tooling-major-008-native-vs-code-handoff-ux.trace.md)
- Current
  - Current Schema: tiinex.evidence.v1
  - Created At: 2026-09-22 15:57:13
  - Authors: Kodax
  - Why: Return the first exact shared-Core capability blocker required by the selected Anchor-to-Kodax Handoff without mutating VS Code or Core source.
  - Summary: Kodax proves the exact carried Core cannot yet persist qualified Handoff endpoint References through the shared creation contract, so VS Code must stop before a host-private workaround.
  - Status: ready/local

---

# Tooling Major 008 — Kodax Shared-Core Endpoint Authoring Blocker

## Supported Claim Or Question

- Supported Claim Or Question: Can the exact carried Core currently persist a qualified VS Code From/To Role selection as durable canonical `From Reference` / `To Reference` fields through the shared Handoff creation path required by Tooling Major 008?
- Evidence Role: exact Kodax blocker evidence for the first shared-Core capability gap encountered before any host-private workaround or VS Code product mutation.

## Provenance

- Known Source: exact qualified `core` and `vscode` Workspace snapshots carried by `business-001-1-anchor-to-kodax.handoff-package.zip` and materialized only after Tiinex grounding of `001-3-1-1-1-handoff-pointer.trace.md`.
- Preservation Basis: the carried Core and VS Code source snapshots were inspected read-only; no product source byte was changed.
- Provenance Limits: this Evidence proves the exact current creation-contract/interface blocker only. It does not substitute for Loom implementation, integrated machine acceptance, or Sigma real-host acceptance.

## Evidence Material

- Material Kind: exact carried Core creation-contract projection plus exact renderer/source inspection.
- Material: `node tools/tiinex-portable.mjs inspect-creation-contract --schema tiinex.handoff.v1` executed from the exact carried Core Workspace, together with the carried Handoff runtime schema and generic creation renderer.

### Exact first blocker

- The canonical Handoff runtime shape recognizes optional `From Reference` and `To Reference` fields under `Handoff Parties`.
- The exact carried Core creation contract for `tiinex.handoff.v1` reports `optionalInputs: []`.
- Its `inputBindings` include `Purpose`, `From`, `From Kind`, `To`, `To Kind`, and the remaining required Handoff sections, but contain no binding for `From Reference` or `To Reference`.
- The shared generic creation renderer emits ordinary fields only by iterating those creation `inputBindings`; unbound endpoint Reference values therefore cannot be persisted through the qualified shared creation path.
- The VS Code authoring panel already retains exact qualified endpoint candidate identity (`reference`, `workspaceId`, `path`) in its host submission, but passing or formatting those References itself would make VS Code a second semantic authoring implementation, which the controlling Major explicitly forbids.
- Therefore Kodax cannot satisfy durable qualified endpoint authoring, restart reconstruction, or endpoint-material correctness without a shared-Core authoring capability that accepts exact qualified endpoint selections/References and renders/validates the canonical optional Handoff Reference fields.

### Adjacent participant seam observed but not promoted ahead of the first blocker

- The exact carried Core manufacture path also treats route-level `participantRoles` as validation input that must match an already established semantic participant set from the controlling current-work Task; it rejects explicit route participant input when no such semantic declaration exists.
- Tooling Major 008 requires Attach-time explicit zero/one/many additional Role selection as operator input authority. This remains a likely subsequent shared-Core interface seam, but the durable endpoint creation gap above is the first blocker and is sufficient for this return.

## Preservation And Fidelity

- Preservation State: no Core source, VS Code source, schema, fixture, package representation, or product runtime byte was changed.
- Fidelity Notes: the blocker is derived from the exact carried Core contract at the selected route frontier, not from an older audit or repository assumption.
- Known Losses: no integrated Loom repair is present in this carrier, so Kodax cannot exercise the final durable-reference or participant-selection machine scenarios yet.

## Interpretation Limits

- Does Not Prove: that canonical Handoff semantics are wrong, that endpoint References must become mandatory, that VS Code should construct References, or that Package V1 requires redesign.
- Must Not Be Treated As: permission for a VS Code-private semantic layer, recursive repository discovery, manual Reference string synthesis, participant authority from Role carriage, or a Sigma acceptance result.
- Not Yet Used As: Tooling Major 008 completion or real-host acceptance.

## Review Notes

Loom/Core needs to expose a shared qualified creation/update surface that can receive exact endpoint Role/Party selections and persist optional canonical `From Reference` / `To Reference` fields while keeping identity-less endpoints valid. Once that exact shared capability is carried back, Kodax can implement the remaining thin-host selector/reload/Attach/preview work without duplicating semantic logic.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [026-anchor-to-kodax-tooling-major-008-native-vs-code-handoff-ux.trace.md](handoffs/026-anchor-to-kodax-tooling-major-008-native-vs-code-handoff-ux.trace.md)
  - Value: MDWEfdxZ810SqwNJg2FD0GGHep1cHa0FAFvl5SrlH58

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 7puWLfXPheAtlym14pPrfkZOQCiYQonN5Zf0XBdoNFA