# claude-agent-sdk-python

- Source: [Cocoon-AI/claude-agent-sdk-python](https://github.com/Cocoon-AI/claude-agent-sdk-python)
- Category: Python SDK for Claude Agent workflows
- Snapshot stars (2026-04-17): 0
- License: MIT
- Language: Python

## What it gives you

Python-native access to Claude Agent flows, including async query streams, options control, and in-process SDK MCP tools.

## Why this matters for Sol-HQ

- Enables scripted pipeline automation around architecture generation workflows.
- Supports custom tool integration for repository parsing and project log extraction.
- Good bridge for internal Python automation services.

## Risks and caveats

- Requires Node.js and Claude Code runtime prerequisites.
- Production usage should include retries, timeout policies, and output validation.

## Recommended usage

- Use for orchestration scripts that parse repo/project notes and ask an LLM to produce structured architecture specs.
- Add deterministic post-processing for diagram-ready JSON/markdown outputs.

## First implementation step

Build a small Python script that ingests a repo summary file and emits a normalized architecture spec for diagram generation.
