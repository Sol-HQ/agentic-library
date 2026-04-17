# andrej-karpathy-skills

- Source: [forrestchang/andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills)
- Category: Agent behavior and coding guidelines
- Snapshot stars (2026-04-17): 53,738

## What it gives you

A compact `CLAUDE.md` rule set focused on reducing common LLM coding failures: bad assumptions, overengineering, and unrelated edits.

## Why this matters for Sol-HQ

- Standardizes agent behavior across trading, minting, and infra repos.
- Reduces accidental refactors and noisy diffs.
- Improves verification discipline (goal-driven loops).

## Risks and caveats

- License is not clearly specified in repository metadata.
- It is guidance, not executable runtime software.

## Recommended usage

- Keep as a policy baseline in every agent-enabled repository.
- Derive a Sol-HQ-specific version with project conventions.

## First implementation step

Create a shared `AGENT_RULES.md` in your org template repos using these four principles, then customize for Solana/agent workflows.
