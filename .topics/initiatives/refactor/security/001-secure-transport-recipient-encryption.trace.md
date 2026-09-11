# Continuity Context

- Envelope Schema: tiinex.root.v1
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-09-09 14:17:46
  - Trace: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Origin:
    - [relative](../001-turn-2-stable-full-source-frontier.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-09 23:48:32
  - Authors: Anchor
  - Why: Preserve a durable cross-repository security outcome before VS Code and later hosts begin transporting complete Workspace source as a routine operator workflow.
  - Summary: Password-based Workspace-sealed transport capability with shared Docs/Core ownership and host exposure only after qualification.
  - Status: active/local

---

# Secure Transport & Recipient Encryption

## Objective

Establish the cross-repository outcome for password-protected Tiinex transport before any host exposes encryption as a normal operator capability. The first qualified capability must protect carried Workspace source without changing Artifact, Parent, Workspace, Handoff, or provenance semantics.

## V1 Product Decision

V1 is password-based and Workspace-sealed.

- Support password-protected transport for one or more carried Workspaces.
- Seal each protected Workspace byte tree as an opaque encrypted payload so internal filenames, directories, `.topics` structure, and lineage layout are not disclosed by the outer carrier.
- Use a fresh random content-encryption key per protected Workspace and authenticated encryption for the sealed payload; AES-GCM is the intended V1 payload profile unless canonical Docs/Core qualification identifies a narrower portability constraint.
- A password derives or unlocks a wrapping key for the Workspace content key. A password must not be used directly as the payload encryption key.
- The password KDF contract must be explicit and versioned, including algorithm, salt, parameters, and profile version. The exact default KDF and cost parameters are implementation/qualification work and must not be guessed into Business semantics.
- Allow multiple password recipient slots to wrap the same Workspace content key without duplicating the encrypted Workspace payload.
- Allow a multi-Workspace carrier to contain unprotected and protected Workspaces, and to use different recipient/password sets for different protected Workspaces.

## Explicit Exclusions

The first capability does not include:

- ZipCrypto or Windows Explorer password-ZIP compatibility as a security target.
- Passkeys, WebAuthn, biometrics, hardware/security keys, or password-manager-specific integrations.
- Cryptographic artifact signing or identity attestation; signing remains a separate concern from confidentiality.
- Carrier-sealed mode that hides the outer Handoff route and Workspace inventory. V1 protects selected Workspace payloads while leaving the carrier able to route and explain what protected material exists.

## Semantic Boundary

Encryption is a transport/representation concern, not semantic authority.

- Decryption must recover the exact carried Workspace bytes that are then interpreted and validated by normal Tiinex semantics.
- Encryption, password success, AEAD authentication, hashes, and checksums must not be used to claim that semantic Parent, provenance, authority, or content meaning is true.
- Existing unencrypted carriers remain valid and must not be reinterpreted as weaker semantic truth.
- Cryptographic output is intentionally randomized by fresh keys/nonces; deterministic Tiinex behavior means deterministic validation, qualification, and recovery rules, not deterministic ciphertext bytes.

## Ownership And Implementation Order

1. **Docs** owns canonical disclosure, sealed-representation, recipient-slot, password/KDF, recovery, and interpretation semantics.
2. **Core** owns host-neutral seal/open mechanics, content-key generation, password KDF/key wrapping, authenticated-encryption profiles, package representation, fail-closed validation, and exact-byte roundtrip qualification.
3. **CLI** proves the same Core capability headlessly before graphical hosts depend on it.
4. **extension-vscode** may expose Workspace selection, protection configuration, password entry, manufacture, and open/decrypt UX only after the shared primitives are qualified.
5. **App/Site** may later expose the same shared capability; they must not invent a competing encryption format.
6. Providers remain source-access boundaries and do not become cryptographic authority.

## Done Criteria

Before V1 is considered available to normal hosts, qualification must demonstrate at minimum:

- Correct password opens a protected Workspace and reproduces its exact original byte tree.
- Wrong password, corrupted ciphertext, modified authentication data, truncated payload, unsupported profile, and malformed recipient metadata fail closed without partial landing.
- Protected Workspace filenames and directory structure are absent from the outer carrier representation.
- Multiple password recipient slots can independently unlock the same exact encrypted Workspace payload.
- Multiple protected Workspaces can use independent content keys and independent recipient sets in one carrier.
- Plain and protected Workspaces can coexist without changing normal Handoff/Workspace semantics.
- Temporary plaintext handling is bounded and does not silently persist decrypted Workspace material outside the explicit destination/recovery contract.
- Passwords and derived key material are never serialized into durable Tiinex artifacts, logs, routing text, or carrier metadata.
- A CLI roundtrip proves seal -> transport -> open -> exact-byte recovery before VS Code/App/Site UX is promoted.

## Recovery And Human UX Direction

Password loss has no hidden recovery bypass. Recovery must come only from another explicitly authorized password recipient slot or a future separately designed recovery mechanism. Hosts should make protection scope and failure state explicit, never silently downgrade a requested protected Workspace to plaintext transport.

## Scope

Cross-repository planning and qualification boundary for Docs, Core, CLI, extension-vscode, and later App/Site support for password-based Workspace-sealed transport. This Business Task defines the outcome and ownership order; implementation remains repo-local.

## Dependencies

- Current Turn-2 stable full-source frontier and qualified Handoff/Workspace packaging semantics.
- Canonical Docs authority for Artifact, Workspace, Handoff, representation, and integrity semantics.
- Current Core package/Handoff mechanics as the host-neutral implementation boundary.
- A qualified headless CLI proof before graphical host exposure.

## Repo Decomposition Gate

This Business Task authorizes later repo-local Tasks for Docs, Core, CLI, extension-vscode, and eventually App/Site. It does not itself authorize implementation changes or host exposure before the owning lower-layer capability is qualified.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-turn-2-stable-full-source-frontier.trace.md](../001-turn-2-stable-full-source-frontier.trace.md)
  - Value: J7eMDpiRtxZpCqeB-lUxH-EtODAqs4XIYFcndqClJnI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: mE5p0IRNHqTZSCit6271ytohhQB8ly1yCGlOpgkPPw8