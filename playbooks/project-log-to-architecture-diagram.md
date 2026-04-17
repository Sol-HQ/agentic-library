# Project Log to Architecture Diagram

This playbook turns project logs or codebase summaries into architecture diagrams for any project.

## Goal

Create a repeatable pipeline where an agent can:

1. Read project logs and repository structure.
2. Produce a normalized architecture specification.
3. Generate and iterate architecture diagrams.
4. Store diagram artifacts with traceable versions.

## Inputs

- Project logs/changelogs/handoff notes.
- Repository README + top-level structure.
- Key config files (`docker-compose`, infra files, env docs, CI workflows).
- Runtime paths (APIs, workers, queues, DBs, external integrations).

## Normalized architecture spec format

Use this markdown skeleton before diagram generation:

- System boundary
- User-facing clients
- Core services
- Data stores
- Messaging/streaming
- External dependencies
- Security/auth boundaries
- Deployment/runtime platform
- Observability components
- Critical data/control flows

## Pipeline (recommended)

1. **Extract**
   - Agent reads logs and code summaries.
   - Agent outputs structured architecture bullets.

2. **Normalize**
   - Convert extracted notes into the architecture spec format above.
   - Resolve naming inconsistencies and remove duplicates.

3. **Generate diagram**
   - Use `architecture-diagram-generator` skill with the normalized spec.
   - Export standalone HTML/SVG output.

4. **Review and iterate**
   - Engineers verify missing components, wrong edges, and boundary mistakes.
   - Regenerate until approved.

5. **Version and publish**
   - Store source spec + generated diagram in git.
   - Tag by date/version and link in project docs.

## Automation option with Python SDK

Use `claude-agent-sdk-python` to automate extraction and normalization:

- Step A: parse repo + logs into an architecture JSON object.
- Step B: ask Claude to convert JSON into diagram-ready architecture prompt text.
- Step C: run manual or semi-automated diagram generation with Cocoon skill.

## Quality checklist

- Every major service appears exactly once.
- Every DB/cache/queue has at least one producer and consumer edge.
- Auth and trust boundaries are explicit.
- External systems are visually separated.
- Critical flows are labeled (write path, read path, async path).

## Minimum deliverables per project

1. `architecture-spec.md`
2. `architecture-diagram-v1.html`
3. `architecture-diagram-v1.svg`
4. `architecture-notes.md` (assumptions + unresolved questions)
