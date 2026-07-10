---
type: Entry Point
title: constitution
description: Composition contract for the Architectonic software ensemble.
tags: [constitution, architectonic, composition, okf]
okf_version: "0.2"
status: draft
---

# constitution

```bash
npx architectonic add constitution
```

`constitution` defines how Architectonic packages are composed into a coherent workspace for human-AI collaboration. It is the composition contract, not the source of truth for any layer it composes.

`npx architectonic init` creates a workspace and installs the full ensemble.

## In the ensemble

```text
constitution      composition contract for the ensemble
doctrine          purpose, principles, ontology, epistemology, ethics, governance, incentives
identity          actors, roles, authority, delegation, incentives, privacy
project           operating-unit context, sources, decisions, risks, continuity
skills            reusable procedures, verification, failure handling
knowledge         claims, sources, evidence, uncertainty, known unknowns
models            model metadata, evaluations, capability requirements, routing policy
agents            software actors composed from identity, skills, models, knowledge, permissions
living-knowledge  optional: governed maintenance of frequently changing corpora
meta              audit, upkeep, drift review, revision policy
```

```text
constitution      -> composes the ensemble
doctrine          -> defines governing principles
identity          -> defines participating actors and authority
project           -> defines the concrete operating context
skills            -> defines reusable procedures
knowledge         -> defines retained claims and evidence
models            -> defines computational capabilities and routing evidence
agents            -> composes actors, procedures, models, knowledge, and permissions
living-knowledge  -> defines maintenance of changing corpora
meta              -> defines audit, upkeep, and revision
```

## Commands

```bash
npx architectonic init                      # install full ensemble
npx architectonic add constitution
npx architectonic add <layer> --source npm
npx architectonic list
npx architectonic doctor
npx architectonic status
npx architectonic update
```

CLI: https://github.com/architectonic/architectonic

## Boundary

This repository may contain composition rules, bundle metadata, and workspace scaffold instructions. It should not duplicate the full contents of the packages it composes.

## Composition principles

- Each concept has one primary home.
- More specific layers may narrow general rules but should not silently contradict them.
- Private instance data belongs in instantiated workspaces, not in public package templates.
- Generated indexes, summaries, embeddings, and graph projections remain derived from canonical sources.
- Authority, review gates, escalation paths, and stopping conditions should be explicit and proportionate to risk.
- An artifact should exist only when it changes future action, preserves evidence, defines authority, routes to source truth, or removes demonstrated ambiguity.

Architectonic packages are runtime-neutral. Workframe, command-line agents, hosted services, and other environments may instantiate the same constitution while retaining their own runtime concerns.
