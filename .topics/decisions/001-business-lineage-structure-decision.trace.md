# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.party.organization.v1](tiinex.party.organization.v1.schema.md)
  - Created At: 2026-08-26 14:55:00
  - Trace: [001-tiinex.trace.md](../001-tiinex.trace.md)
  - Origin:
    - [relative](../001-tiinex.trace.md)
- Current
  - Current Schema: [tiinex.decision.v1](https://github.com/Tiinex/docs/blob/e713557f8be630967571d11a73f9ecd05ae329ce/.topics/.schemas/core/decision/tiinex.decision.v1.schema.md)
  - Created At: 2026-08-26 15:04:00
  - Authors: Anchor
  - Summary: Business lineage structure
  - Status: draft/local
  - Why: Materialized from the current Anchor/Sigma business design conversation under the received Anchor-to-Anchor Handoff.

---

# Business Lineage Structure

## Decision

- State: accepted
- Subject: semantic directory lineage in tiinex/business
- Decision: every semantic directory has a local anchor artifact. `.topics/001-tiinex.trace.md` is the organization root; each non-root directory anchor declares the nearest semantic parent directory's anchor as its Tiinex Parent. Directory paths aid navigation but do not own semantic authority.

## Basis

- This keeps every branch understandable without path-only meaning, avoids empty semantic directories, and lets lineage traversal recover the business structure.
- Topic is used for subject-branch anchors; when a directory represents an actual semantic thing, that thing uses its own schema instead.

## Consequences

- Roles, Initiatives, Financing, Funds, and Tips are Topic anchors.
- Tiinex is an Organization artifact.
- Concrete funds are Resource artifacts; concrete roles and initiatives use their own Role and Project schemas when they exist.
- No semantic directory should be created only as an empty taxonomy placeholder.

## Review Conditions

- Review if Tiinex gains an explicit branch-anchor schema or another declared authority that supersedes this local anchor convention.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-tiinex.trace.md](../001-tiinex.trace.md)
  - Value: I5bYzRG0q6hwwKntzZFHteClGsiGQRVN7yr7uo9TcFI

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: AtqJa1U-F9z6EymepGN2qcHlHErunTbI3SJewgerX8Y
