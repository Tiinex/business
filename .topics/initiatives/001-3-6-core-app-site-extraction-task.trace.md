# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Viewer](001-3-viewer-project.trace.md)
  - Origin:
    - [relative](001-3-viewer-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-09-08 17:38:00
  - Authors: Anchor
  - Why: Preserve the user-requested source extraction and its actual qualification boundary.
  - Summary: Bound the Core/App/Site extraction and first full-source checkpoint without claiming closure.
  - Status: active/local

---

# Extract Core and App; unblock the Playthings consumer

## Objective

Extract the portable implementation into Tiinex/core and reusable Viewer and Verse hosting into Tiinex/app. Site consumes installed npm packages rather than maintaining copied implementations. Establish the read-only application data and resource contracts needed by the supplied Playthings headless foundations.

## Done Criteria

- Public Core/App entrypoints work from installed npm tarballs, not source links.
- Site is a deployment above App; existing Viewer behavior is tested after extraction.
- Playthings can consume the declared data and companion API without Site-internal imports.
- Dependency-equipped React/Vite build and browser mounting pass before calling Turn 1 ready for human Verse testing.
- A qualified full-source Handoff carries Business, Docs, Site, Playthings, Core and App with honest test evidence.

## Scope

Anchor owns implementation and qualification. Sigma supplies human observation and independently chooses whether to preserve, commit or publish a candidate; this does not assign technical/canonical authority. No remote repository mutation or npm publishing is authorized here. No new Playthings world runtime is implemented in this lane.

## Dependencies

- [Viewer initiative](001-3-viewer-project.trace.md)
- [Tooling initiative](001-2-tooling-project.trace.md)
- [Core initiative](001-1-core-project.trace.md)
- [Playthings initiative](001-9-playthings-project.trace.md)

The new Core repository is an implementation/distribution boundary, not a reassignment of canonical meaning from Docs. Historical Site reduction and CLI/Interop/Chrome/VS Code work remain Round 2.

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Viewer](001-3-viewer-project.trace.md)
  - Value: Z9OpOKoRrUw36W8_jOf7E3_-Ec36pqymqyIHKtYWIYc

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:SOxxB77pxLrbHBJ3AodTGDgynI770PNNulV-Ov0MPqQ