# Standalone Constitution

A constitution is justified when the primary problem is not project planning or knowledge retrieval, but **what may never change silently**.

## Minimum useful contents

```text
purpose boundary
invariants
human authority root
prohibited actions
approval and stopping rights
amendment rule
```

## Standalone examples

- safety boundaries for an agent-enabled repository;
- ownership and amendment rules for a shared protocol;
- non-negotiable privacy or spending constraints;
- a compact contract shared by several independent projects.

## Add other layers only when needed

- Add `doctrine` for general decision rules.
- Add `identity` when actor-specific authority or privacy matters.
- Add `project` for a bounded operating unit.
- Add `meta` when the constitution itself needs scheduled review and migration policy.

A constitution should remain small. Operational details belong in the layer that owns them.
