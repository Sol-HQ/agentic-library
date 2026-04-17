# cognee

- Source: [topoteretes/cognee](https://github.com/topoteretes/cognee)
- Category: Knowledge engine and memory graph
- Snapshot stars (2026-04-17): 16,133
- License: Apache-2.0
- Language: Python

## What it gives you

A memory engine that combines vector retrieval with graph relationships to improve context for agent decisions.

## Why this matters for Sol-HQ

- Good backbone for knowledge retrieval across docs, runbooks, and playbooks.
- Improves long-term memory for agent workflows.
- Can support structured context for trading and minting systems.

## Risks and caveats

- Requires careful schema design and indexing strategy.
- Can become noisy without ingestion quality rules.
- Must include data-governance controls for sensitive inputs.

## Recommended usage

- Start with curated internal docs as ingestion sources.
- Gate writes and enforce quality checks before ingestion.

## First implementation step

Build a small corpus (architecture docs, ops guides, incident notes) and benchmark retrieval relevance against your current setup.
