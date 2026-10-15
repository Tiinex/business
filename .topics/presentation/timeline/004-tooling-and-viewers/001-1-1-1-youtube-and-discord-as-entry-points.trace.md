# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Parent
  - Parent Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 22:03:25
  - Trace: [001-1-1-vision-slides-and-branding.trace.md](001-1-1-vision-slides-and-branding.trace.md)
  - Origin:
    - [relative](001-1-1-vision-slides-and-branding.trace.md)
- Current
  - Current Schema: [tiinex.topic.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/topic/tiinex.topic.v1.schema.md)
  - Created At: 2026-10-15 19:30:36
  - Authors: GPT-6 (reader-safe editorial revision for maintainer review)
  - Why: Public historical presentation. Editorial continuation, not an assertion of original historical causality.
  - Summary: A YouTube command bridge and Discord redirect were integration attempts, not a completed ingestion network.
  - Status: approved-for-publication

---

# Multiple surfaces, different responsibilities

In mid-May there were several public or semi-public *entry surfaces* around Tiinex, with materially different responsibilities.

- **YouTube:** [the May 14 VS Code language-model tool implementation](https://github.com/Tiinex/ai-vscode-tools/blob/6381e54c3b0fde45a0ac1d195a28d1d12d6df34a/src/languageModelTools.ts) includes a bounded YouTube host command interface: setup validation, image creation/viewing and feedback Topic operations such as adding evidence, decisions and focusing a Topic.
- **Discord:** [the May 14 site redirect file](https://github.com/Tiinex/site/blob/3c9b0d3718f058d6a01c81e7711b1364ade184c0/discord/index.html) points a Tiinex web path toward a Discord invite.
- **Durable records:** [the May 13 Topics README](https://github.com/Tiinex/docs/blob/53fe17ea23d3da3d994f14a2cda1d904ca478510/topics/README.md) recommends preserving feedback in a source-neutral Markdown shape.

The higher-level hypothesis was to let different platforms contribute signals without letting a platform become authority over a Tiinex Topic.

## What cannot be claimed

A command interface proves that code was written, **not** that users could rely on a complete integration. A redirect proves a link existed, **not** an operational Discord bot or feedback synchronization. The old separate `youtube`, `reddit` and `discord` repositories are named in legacy materials but were not accessible in this archaeology; treat their historical contents as unverified rather than inventing them.

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: [001-1-1-vision-slides-and-branding.trace.md](001-1-1-vision-slides-and-branding.trace.md)
  - Value: pEWjeDr-isAvezpVjw0slvCHjt23k7IBUXSF0BxQZbM

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: 35EOQKCcVyVEilLIo8zIaBYI3n9I3ouuMYNoEDxOXgw
