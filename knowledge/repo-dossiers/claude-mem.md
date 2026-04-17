# claude-mem

- Source: [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem)
- Category: Session memory and context compression
- Snapshot stars (2026-04-17): 61,104
- Language: TypeScript

## What it gives you

Captures agent activity, compresses session context, and re-injects memory in future sessions. Useful for long-running multi-repo work.

## Why this matters for Sol-HQ

- Strong fit for multi-day agent tasks across trading and agent infrastructure projects.
- Helps preserve technical continuity through model handoffs.
- Reduces repeated context-bootstrapping costs.

## Risks and caveats

- AGPL license implications can affect commercial distribution choices.
- Memory quality depends on compression strategy and relevance filters.
- Needs strict privacy controls when capturing execution data.

## Recommended usage

- Use for internal R&D workflows first.
- Keep memory storage segmented by repository and sensitivity.
- Add redaction filters for secrets and credentials.

## First implementation step

Run a pilot on one internal codebase and measure context reuse quality across 10 sessions before wider rollout.
