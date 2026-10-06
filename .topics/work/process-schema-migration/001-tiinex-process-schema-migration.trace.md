# Continuity Context

- Envelope Schema: [tiinex.root.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/tiinex.root.v1.schema.md)
- Current
  - Current Schema: [tiinex.task.v1](https://github.com/Tiinex/docs/blob/302506f90537dc23d6f88ad0bd0bb9c97c6cf9f6/.topics/.schemas/core/task/tiinex.task.v1.schema.md)
  - Created At: 2026-10-06 18:13:25
  - Authors: Anchor; Sigma
  - Why: Restore schema-as-truth across Tiinex Process surfaces after the dedicated Process-root schema became ready for use.
  - Summary: Migrate maintained Process roots and legacy executable Topic positions to their dedicated Process/Transition schemas while preserving genuine Topic catalogs.
  - Status: ready/local

---

# Tiinex Process Schema Migration

## Objective

Migrate maintained reusable Tiinex Process definitions away from generic Topic typing now that `tiinex.process.v1` is published, synchronized, and authorable.

## Done Criteria

- reusable Process roots use `tiinex.process.v1`
- executable legacy Topic positions use `tiinex.transition.definition.v1`
- durable Relation artifacts remain `tiinex.relation.v1`
- genuine process catalog/index Topics remain `tiinex.topic.v1`
- Parent schema references and continuity integrity are consistent after migration
- all affected Process surfaces audit clean through the synchronized published schema source

## Scope

- Business, Docs, Interop OpenAI, and Native Process surfaces carried in the 029 Workspace representation
- preserve existing filenames and semantic Parent lineage
- preserve legacy prose as migration notes/legacy definition notes when structured schema contracts replace generic Topic bodies
- no remote commit/push or broad non-Process Topic migration

## Dependencies

- published `tiinex.process.v1` at Docs commit `2262a1c4b35e887d116d0d01a864074a9f1641c2`
- synchronized Native published schema surface
- Process Development And Maintenance process

---

# Continuity Integrity

- [sha256-base64url-c14n-v2](https://github.com/Tiinex/docs/blob/3988951208eb9a8926e84ab42625d4b42fa00c2d/.topics/.validators/sha256-base64url-c14n-v2.validator.md)
  - Towards: self
  - Value: QUWXiEBjNJ_Xl1HxUvESG-3fcgvYeWh6x-QyXvSu2RQ