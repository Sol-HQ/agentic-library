# evolver

- Source: [EvoMap/evolver](https://github.com/EvoMap/evolver)
- Category: GEP-based agent evolution engine
- Snapshot stars (2026-04-17): 3,793
- License: GPL-3.0
- Language: JavaScript

## What it gives you

An auditable evolution loop that turns runtime signals into constrained evolution prompts and tracks events over time.

## Why this matters for Sol-HQ

- Strong pattern for systematic prompt and behavior optimization.
- Good fit for internal experimentation on agent improvement loops.

## Risks and caveats

- GPL-3.0 can affect distribution and integration strategy.
- Should be paired with robust evaluation datasets, not only heuristic logs.

## Recommended usage

- Use in a research lane first.
- Export ideas (auditability and evolution events) into internal tooling.

## First implementation step

Define a small evaluation benchmark and run controlled evolution cycles with change logs and rollback criteria.
