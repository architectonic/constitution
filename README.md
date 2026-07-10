---
type: Entry Point
title: constitution
description: Composition contract for the Architectonic software ensemble.
tags: [constitution, architectonic, composition, okf]
okf_version: "0.2"
status: draft
---

# constitution

`constitution` defines how the Architectonic packages are composed into a coherent workspace for human-AI collaboration.

Install it with:

```bash
npx architectonic add constitution
```

`npx architectonic init` creates a workspace and installs the constitution ensemble.

## Ensemble

```text
doctrine          -- purpose, principles, ontology, epistemology, ethics, governance, incentives
identity          -- actors, roles, authority, delegation, incentives, privacy
project           -- operating-unit context, sources, decisions, risks, and continuity
skills            -- reusable procedures, verification, and failure handling
knowledge         -- claims, sources, evidence, uncertainty, and known unknowns
models            -- model capabilities, constraints, evaluations, cost, and routing evidence
agents            -- composed software actors with identity, skills, models, knowledge, and permissions
living-knowledge  -- governed maintenance of changing knowledge corpora
meta              -- audit, upkeep, drift review, and revision policy
```

## Role

A constitution is a composition contract. It identifies the packages that participate, defines their boundaries, and establishes how authority flows between them without making any package the source of truth for the others.

```text
constitution      -> composes the ensemble
doctrine          -> defines governing principles
identity          -> defines participating actors and authority
project           -> defines the concrete operating context
skills            -> defines reusable procedures
knowledge         -> defines retained claims and evidence
models            -> defines available computational capabilities and constraints
agents            -> composes actors, procedures, models, knowledge, and permissions
living-knowledge  -> defines maintenance of changing corpora
meta              -> defines audit, upkeep, and revision
```

## Boundary

This repository may contain:

```text
constitution.md
bundle metadata
composition rules
workspace scaffold instructions
```

It should not duplicate the full contents of the packages it composes.

## Composition principles

- Each concept has one primary home.
- More specific layers may narrow general rules but should not silently contradict them.
- Private instance data belongs in the instantiated workspace, not in public package templates.
- Generated indexes, summaries, embeddings, and graph projections remain derived from canonical sources.
- Authority, review gates, escalation paths, and stopping conditions should be explicit and proportionate to risk.
- An artifact should exist only when it changes future action, preserves evidence, defines authority, routes to source truth, or removes demonstrated ambiguity.

## Relationship to runtimes

Architectonic packages are runtime-neutral. Workframe, command-line agents, hosted services, and other execution environments may instantiate the same constitution while retaining their own runtime concerns.

## Status

Draft composition contract for the full Architectonic ensemble.