# Constitution

> **Status: experimental, pre-1.0.** A constitution makes declared invariants and authority inspectable. It does not prove that the resulting system is correct, lawful, safe, or well governed.

`constitution` is a **standalone layer** for what must remain true while a human–AI system changes.

Use it for:

- non-negotiable invariants;
- the human authority root;
- prohibited actions and approval boundaries;
- amendment and override rules;
- composition rules between independently owned concerns.

Do not install a full organization merely to obtain a constitution.

```bash
npx architectonic@latest init my-boundary --preset constitution --source npm
```

Add doctrine, identity, project, knowledge, agents, or meta only when those concerns need their own durable homes.

See [`STANDALONE.md`](./STANDALONE.md) and [`constitution.md`](./constitution.md).
