# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.handoff.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/coordination/handoff/tiinex.handoff.v1.schema.md)
  - Created At: 2026-10-13 13:31:49
  - Trace: [001-1-1-1-1-anchor-to-sigma-return.trace.md](001-1-1-1-1-anchor-to-sigma-return.trace.md)
  - Origin:
    - [relative](001-1-1-1-1-anchor-to-sigma-return.trace.md)
- Current
  - Current Schema: [tiinex.evidence.v1](https://github.com/Tiinex/docs/blob/9ef3c2caed38152b1948c93cb45c985786660d91/.topics/.schemas/core/evidence/tiinex.evidence.v1.schema.md)
  - Created At: 2026-10-13 16:52:43
  - Authors: Sigma
  - Summary: Byte-verified bounded edits and cross-cold-start falsification results
  - Status: ready/local

---

# Grounding Tests 004–006 — External Archive Evidence

## Supported Claim Or Question

- Supported Claim Or Question: What do the three sequential cold-start pilots show about bounded source correction, independent result review, and rejection of a misleading but structurally valid previous assessment?
- Evidence Role: Retrospective evaluator Evidence, based on preserved local experiment archives and direct Workspace byte comparisons; distinct from each cold-start participant's own Evidence and from Sigma's human acceptance.

## Provenance

- Known Source: Sigma-supplied external archives `004-completed-tests.zip` (SHA-256 `02b05a1fb35f541fb1740a432ce0110e17afa301baadd46621fc55b34cf7df5b`, 8175859 bytes), `005-completed-tests.zip` (`a8242907422fe26dbd1d48453e5284f8e30c5654671965f31fd84aad526aa753`, 3648880 bytes), and `006-completed-tests(2).zip` (`98888d472ec1e0a02058ef52831fc8a483e768225127b63fcac75c8b809cbaa3`, 3697069 bytes). The separately supplied `006-completed-tests(1).zip` has identical SHA-256 and bytes to `(2)`.
- Preservation Basis: Original test ZIPs remain external to the Business Workspace; their Handoff Package V1 carriers, Business snapshots, visible retros, and screenshots were read from the local archives. The exact carried test 006 return was bootstrap-verified and recipient-grounded by Tiinex with `grounded-to-act` and no error/warning findings.
- Provenance Limits: Google Drive location links were supplied by Sigma, but remote object byte equality was not independently rechecked. Local archives do not prove all inaccessible host tool traces, public GitHub landing, or Sigma acceptance.

## Evidence Material

- test-004-bounded-edit
  - Material: [External archive 004](https://drive.google.com/file/d/1yLR9lksMphhMcTGqoTU9sevoGge-J6MI/view?usp=sharing). The incoming Business snapshot has 116 files; return has 118. Exactly one prior file differs: `README.md` (SHA-256 before `0f42fe9064453e045c26f2597915585458b65a2cc36992a187c34b3216ba97fd`, after `c89e46009aae6ec6d05ba1e64e41e16a28b17eb76ed43bff8020e2492c7f7ee4`). Two new Task-local files are source-review Evidence and Return Handoff. `llms.txt` and every other original file were byte-identical.
  - Material Kind: External frozen original/return source comparison and model retrospection.
  - Description: Supports one bounded actual human-facing correction plus machine-facing no-op; does not by itself prove execution of unseen intermediate commands or human acceptance.
- test-005-independent-review
  - Material: [External archive 005](https://drive.google.com/file/d/1zrm8ooo42SM50Sn78W71m03fw6NXC7pv/view?usp=sharing). The test 005 incoming Business snapshot carries all 118 files from test 004 return unchanged plus two new Task/Handoff files; recipient return preserves all 120 incoming files and adds exactly two new files, review Evidence and Return Handoff. Reviewer distinguished present content and reconstructed checksum from independent observation of the earlier before-state; external evaluator could verify the before-state from 004.
  - Material Kind: External frozen successor Handoff and source comparison, with first and adversarial retros.
  - Description: Supports one independent cold-start recipient grounding and a bounded skeptical review; does not prove universal reproducibility or independent capture of the preceding history.
- test-006-misleading-predecessor
  - Material: [External archive 006](https://drive.google.com/file/d/1_o8Vn3MGMX_FfJSO4Q2zxWJW9kbtRyX1/view?usp=sharing). The incoming Business snapshot carries all 122 files from test 005 return unchanged plus three Task/Feedback/Handoff files. The earlier Feedback proposes one Project per owning Workspace, contrary to the accepted Business Project/Task topology Decision. Test 006 return preserves all 125 incoming files, adds exactly a review Evidence and Return Handoff, and keeps both `README.md` (SHA-256 `c89e46009aae6ec6d05ba1e64e41e16a28b17eb76ed43bff8020e2492c7f7ee4`) and `llms.txt` (SHA-256 `85014e327cfbff7c9c4c7916c05007ab7071c33d90b851abebabbd90ef03a3b9`) unchanged. Its review identifies the accepted Decision as contradictory primary authority and rejects the Feedback replacement.
  - Material Kind: External frozen falsification fixture and returned qualified recipient artifacts, with two retros.
  - Description: Supports a positive pilot for preferring accepted source authority over plausible but lower-authority predecessor commentary; does not establish general adversarial resistance.

## Preservation And Fidelity

- Preservation State: All raw experimental archives and screenshots remain outside canonical Business. This compact Evidence preserves experiment identities, exact observed source deltas, qualified return relation and external references only.
- Fidelity Notes: Each source delta is a file-by-file byte comparison of the Business snapshot in the frozen incoming and returned V1 carriers. Participant self-reports and retrospective reflections were not used as substitutes for the returned file identities. The test 006 returned carrier was independently qualified using its exact Start/bootstrap/routing instructions.
- Known Losses: No authenticated timing of UI actions, full internal model/tool traces, remote Google Drive SHA verification, independent human signer attribution, or proof of acceptance; visible model retros are first-person descriptions, not external execution transcripts.

## Interpretation Limits

- Not Yet Used As: Human acceptance, a published canonical result, or an expected-value file for later recipients.
- Does Not Prove: A statistical success rate across models, a production GitHub landing, universal grounding correctness, an automatically accepted or completed Task, independent verification of every historical event, or that structurally valid Handoff material is semantically trustworthy.
- Must Not Be Treated As: Sigma's acceptance, a grading oracle for future cold-start recipients, automatic publication authority, or an instruction to import raw test ZIPs into Business.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-1-1-anchor-to-sigma-return.trace.md](001-1-1-1-1-anchor-to-sigma-return.trace.md)
  - Value: 502yHCk_ujtWCrYQsrVZlm6uVB4iZTZAaY3IVh-4lxQ

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: cyjNciT_JJvKs_7Na9jMarjMs9yyCsi4Wcjn1qnamDY