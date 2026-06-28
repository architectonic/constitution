---
type: Entry Point
title: constitution
description: Root constitutional scaffold for composing doctrine, identity, project, skills, knowledge, and meta layers.
tags: [constitution, architectonic, scaffold, okf]
okf_version: "0.1"
status: draft
---

# constitution

`constitution` is the default Architectonic scaffold for a human-agent system.

Install it with:

```bash
npx architectonic add constitution
```

`npx architectonic init` is an alias for adding the constitution scaffold into a new workspace.

The default scaffold installs the core stack:

```text
doctrine   -- governing principles, purpose, ethics, ontology, epistemology, governance, incentives
identity   -- actors, roles, authority, delegation, incentives, privacy
project    -- operating-unit context, sources, decisions, risks, artifacts
skills     -- reusable procedures and verification
knowledge  -- disclosed corpus of knowledge and evidence
meta       -- self-observation, upkeep, drift control, recursive improvement
```

Optional addon:

```bash
npx architectonic add living-knowledge
```

`living-knowledge` is not part of the default constitution install. It is a separate maintenance layer for teams that want explicit corpus campaigns and publication gates.

## Role

A constitution is the governing scaffold that binds the system's purpose, actors, operating unit, reusable skills, knowledge corpus, and upkeep procedures without making any one layer the source of truth for the others.

The constitution bundle is composed from canonical source packages:

```text
doctrine   -- governing principles, purpose, ethics, ontology, epistemology, governance, incentives
identity   -- actors, roles, authority, delegation, incentives, privacy
project    -- operating-unit context, sources, decisions, risks, artifacts
skills     -- reusable procedures and verification
knowledge  -- disclosed corpus of knowledge and evidence
meta       -- self-observation, upkeep, drift control, recursive improvement
```

`constitution` is not a replacement for those packages. It is the root contract that composes them.

## How the packages fit together

```text
constitution      = root scaffold
doctrine          = why and by what rules the system operates
identity          = who participates
project           = where a concrete operating unit does its work
skills            = how repeatable procedures are performed
knowledge         = what claims, sources, and evidence are retained
meta              = how the system audits and improves itself
living-knowledge  = optional addon for campaign-based maintenance of knowledge
```

## Boundary

This repository may contain:

```text
constitution.md
bundle metadata
root scaffold instructions
composition rules
```

It must not duplicate the full content of `doctrine`, `identity`, `project`, `skills`, `knowledge`, or `meta`.

## Relationship to Workframe

Workframe is not part of the constitution package. Workframe is an execution environment where one or more constitutions may be instantiated as governed human-agent workspaces.

## Status

Draft root scaffold. The CLI should install this package and the canonical layer packages directly from their source repositories.
