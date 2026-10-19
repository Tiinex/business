# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-12 23:07:16
  - Trace: [001-grounding-validation-and-acceptance.trace.md](../001-grounding-validation-and-acceptance.trace.md)
  - Origin:
    - [relative](../001-grounding-validation-and-acceptance.trace.md)
- Current
  - Current Schema: [tiinex.evidence.v1](https://github.com/Tiinex/docs/blob/9ef3c2caed38152b1948c93cb45c985786660d91/.topics/.schemas/core/evidence/tiinex.evidence.v1.schema.md)
  - Created At: 2026-10-17 12:13:13
  - Authors: Anchor (bounded explicit-session)
  - Summary: Anchor 028 Guided Entry source fix, complete recovery and manual replay; Sigma acceptance pending
  - Status: ready/local

---

# Guided Entry Primary Session Role — 028 Cold-Start Repair And Manual Replay

## Supported Claim Or Question

- Supported Claim Or Question: Can a user-selected Guided Entry Primary Role operate as the chosen bounded session Role on a fresh ChatGPT Web-oriented cold start, without mistakenly claiming Handoff transfer or additional authority?
- Evidence Role: Local Anchor source-candidate change and independent Tooling/receiver reproduction for Sigma's final acceptance; not final behavioral acceptance, repository publication, or a routed formal Handoff.

## Provenance

- Known Source: Complete qualified route-less `tiinex-028.handoff-package.zip`, 17 Workspaces; Start-directed exact SHA-verified embedded bootstrap; selected Native Explore, OpenAI ChatGPT Web, carried Business Anchor and Sigma Roles; Sigma's fresh in-conversation drift observations on October 17, 2026.
- Governing Work: Existing Business Grounding And Continuity Readiness Project and its Grounding Validation And Acceptance Task. Core owns projection implementation and regression tests; VS Code owns human UI language; Docs owns canonical Assignment Modes; Sigma owns final human acceptance.
- Authority: Sigma explicitly assigned Anchor bounded `explicit-session` capacity in the existing conversation. This does not assert a permanent holder, Handoff recipient, Source landing authority or remote mutation permission.
- Preservation Basis: Complete original Core-manufactured carrier and receiver-only verified successor closure; the external conversation video and Sigma direct observations remain contextual evidence, not package authority.
- Provenance Limits: Local source modifications come from the carried Core Workspace, not fetched or committed public GitHub state. Manual cold receiver exercise validates transport content and package recovery, not an independent model's autonomous behavior.

## Evidence Material

- Guided Entry source fix and replay
  - Material: [Carried Anchor Role with explicit-session Assignment Mode](../../../roles/001-1-anchor-role.trace.md)
  - Material Kind: local Core implementation, regression coverage, qualified ZIP carrier and manually inspected Tooling receipts
  - Description: Exact qualified Primary Role context; separately the local candidate source and test modifications, original 028 carrier, and successor receiver replay are preserved in the complete 028-1 carrier, not as loose Business attachments.

**A-001 observed failure:** Guided Entry selection `Primary Role: Anchor` was transported as `Session Role: Anchor` alongside `presentation only`; the receiving model read Roles but reported not operating as Anchor, requiring Sigma's corrective assignment. Core's existing test asserted the old text. The carrying 028 package itself oriented cleanly and was not a routed Handoff.

**A-001 current-source fix:** In carried `core/src/tooling/portable/handoff/workspaceEntryProjection.js`, reuse the existing `parseRoleMaterial` canonical schema qualification to require carried Primary Roles to authorize `explicit-session` and reject disallowed/unresolved ones. For a commit-pinned external Role, require receiver-side exact qualification. Generated transport positively instructs bounded Role operation, separately describing Participant as context only; it explicitly denies permanent holder, routing, recipient transfer, acceptance, Project/Task control and remote mutation.

**Regression:** Existing `core/test/workspace-entry-projection.test.mjs` was updated to expect positive activation and now includes carried `handoff`-only Role rejection and participant-only nonactivation. Targeted run: 13/13 PASS (October 17). Full `npm test` was attempted and exceeded the runtime timeout after 238 passing tests had appeared; this is NOT a full-suite PASS.

**A-002 predecessor preservation:** Original attempt with only current Core root was correctly blocked with missing predecessor Workspaces. Retried through existing Core CLI using explicit `--additional-workspaces` + `--workspace-targets` for all original workspace snapshots, not a new packaging protocol. Manufacture receipt: 17 Workspaces qualified, `packageInspection: valid`, `roundtrip: passed`, predecessor coverage `all-previous-workspace-ids-present`, no errors, carrier lineage `028-1` parent `028`.

**Manual end-to-end:** Extracted only the SHA-verified embedded Tooling bootstrap from a newly manufactured successor into a separate receiver root; its `orient` returned `ready` with 17 qualified Workspaces and clean findings. The recipient's own `project-workspace-carrier-entry`, given exact carried Anchor/Sigma Roles, `EXPLORE` and ChatGPT Web target, returned `ready`, selected the correct carrier references, emitted `Primary Session Role: Anchor`, and instructed `operate as the selected Role` conditional on canonical `explicit-session`, without a route/recipient transfer claim.

**Portability:** Patched Core module and tests were confirmed present in the successor Core Workspace archive, and patched module present in its exact embedded bootstrap. Session-local JSON CLI input files are disposable runtime arguments outside Workspace and are not carried as source, status sidecars, or new semantic records.

## Preservation And Fidelity

- Preservation State: This evidence is a qualified child of the existing Business validation Task, carried within the complete successor alongside exact owning Core local source and tests. No new owning Project, alternate Role registry, JSON sidecar, or extra durable Workspace was introduced.
- Operator Constraints: Avoid new technical debt and ownership growth; preserve Tiinex conventions; deliver only a complete verified Handoff Package carrier (route-less checkpoint when there is no transfer); Sigma is the final acceptor, never the debugger.
- Expected Human-Visible Change: A new cold receiver given only the generated transport and successor ZIP should qualify and operate as Anchor without Sigma's reminder, execute bounded discovery/verification, disclose blockers, and request Sigma only for final acceptance. A secondary control with no Primary Role should not self-assign Anchor. An unauthorized Primary Role should be rejected.
- Fidelity Notes: Targeted 13/13 PASS; independently rebuilt 17-Workspace carrier valid/roundtrip and cold-receiver orientation ready; full npm test timed out and ChatGPT Web behavioral outcome awaits Sigma.
- Known Losses: No true independent GPT Web cold-start behavior or Sigma human acceptance has yet occurred; the attempted broad test run did not complete. This is local candidate source, not repository publication. Do not conflate technical projection success with semantic/behavioral acceptance.
- Recovery Boundary: The successor must preserve complete 17-Workspace closure, parent dimension 028, embedded patched Tooling and both Business evidence plus Core source. Link and display only the exact Core-projected canonical filename.

## Interpretation Limits

- Does Not Prove: public GitHub landing, permanent Role holder identity, delegated specialist authority, formal Handoff/recipient transfer, remote mutation, general model reliability, Sigma acceptance, or broad Core test-suite PASS.
- Not Yet Used As: final grounding gate closure or permission to promote draft Role candidates globally.
- Must Not Be Treated As: a new project/task owner, a second packaging protocol, an instruction to create loose artifacts, or a substitute for an actual fresh Web conversation test.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-grounding-validation-and-acceptance.trace.md](../001-grounding-validation-and-acceptance.trace.md)
  - Value: EQCmmsJdhNwzxbzRoaT82XPMIRujdkIw4q9VFQ-UCTY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: HELMnbpJ4wbAWTw6OZIO-2yfLZMoYfWm1njI-1pR1I8