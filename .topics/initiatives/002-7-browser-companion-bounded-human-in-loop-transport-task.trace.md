# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.project.v1](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.schemas/coordination/project/tiinex.project.v1.schema.md)
  - Created At: 2026-08-26 22:24:00
  - Trace: [Tiinex Tooling](002-tooling-project.trace.md)
  - Origin:
    - [relative](002-tooling-project.trace.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/053d46ce082d4ec261b82abc44ecca403d61e240/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-08-27 12:25:00
  - Authors: Anchor; Sigma
  - Why: Tiinex already demonstrates compatible JavaScript surfaces in the browser and portable CLI. A thin browser adapter can improve human ergonomics, preserve observed host interaction evidence, and reduce repetitive manual Handoff transport without turning convenience into autonomous authority.
  - Summary: Epic work package for a browser-host Tiinex companion that observes interaction latency and provides bounded access-level-1 transport assistance while keeping the human explicitly in control.
  - Status: accepted/local

---

# Browser Companion And Bounded Human-In-The-Loop Transport

## Objective

Build a host-adapter architecture, with Chrome/Chromium as the first implementation, that opens a local Tiinex surface, observes bounded host UI events, records actual submit-to-next-ready latency, and supports explicitly delegated semi-automatic non-human Handoff transport with hard circuit breakers.

## Done Criteria

- The extension opens a local Tiinex surface that reuses shared Site/Tooling semantics instead of implementing a parallel hidden model.
- A thin content-script adapter can emit neutral observed interaction events such as submitted, busy, and ready without claiming access to hidden model/runtime timing.
- Observed wall-clock turn latency can be preserved as a truthful Tiinex artifact with host, timestamps, observation method, adapter version, and interpretation limits.
- Access-level-1 transport can proceed only inside an explicit user-approved delegation budget, excludes automatic transport to human roles, and stops for active human reauthorization at the configured circuit breaker.
- Chrome-specific DOM behavior is isolated behind a host adapter so the epic identity remains browser companion and bounded transport rather than one fragile ChatGPT DOM implementation.

## Scope

- Browser extension shell, local Tiinex tab/surface, content-script host adapters, observation events, local state, bounded transport ergonomics, delegation budgets, and circuit breakers.
- The old Chrome/VS Code experiment may be inspected as historical implementation inspiration only; it is not current architectural authority.
- Do not automate policy circumvention, infer hidden host state, or treat browser-session access as broad API/account authority.

## Dependencies

- Transport Access Level Model Decision.
- Shared Site/Tooling code that remains environment-portable.
- Portable Handoff semantics and host-specific observation evidence.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [Tiinex Tooling](002-tooling-project.trace.md)
  - Value: 0zVe7vLWB7VMnz_nU766CpSRIadi72v6t8oX4sxuCxY

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value:dBkdKLAe7SkyEF9tUUsjnnV2sqolVkJSiITnQR35AA0
