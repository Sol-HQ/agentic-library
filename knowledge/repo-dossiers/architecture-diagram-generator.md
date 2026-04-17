# architecture-diagram-generator

- Source: [Cocoon-AI/architecture-diagram-generator](https://github.com/Cocoon-AI/architecture-diagram-generator)
- Category: Architecture diagram generation skill
- Snapshot stars (2026-04-17): 3,294
- License: MIT
- Primary output: standalone HTML/SVG diagram assets

## What it gives you

A Claude skill that converts architecture descriptions into professional diagrams quickly, with an iterative chat loop for refinements.

## Why this matters for Sol-HQ

- Fast architecture artifacts for trading bots, minting systems, and agent infra.
- Repeatable diagram generation from plain-text project notes.
- Strong fit for documentation and onboarding velocity.

## Risks and caveats

- Requires a paid Claude tier for skills support.
- Output quality depends on completeness of architecture input text.
- Generated diagrams should be reviewed by engineers before publication.

## Recommended usage

- Standardize an input template: components, edges, protocols, storage, auth, external dependencies.
- Keep diagram versions in git with corresponding architecture notes.

## First implementation step

Use a single active Sol-HQ project log as input and generate v1 architecture + one revision cycle.
