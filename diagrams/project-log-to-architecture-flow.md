# Project Log to Architecture Flow

```mermaid
flowchart TD
    A[Project Logs and Handoff Notes] --> B[Repository Scan README Structure Key Config]
    B --> C[Architecture Extraction Agent]
    C --> D[Normalized Architecture Spec]
    D --> E[Diagram Prompt Builder]
    E --> F[Cocoon Architecture Diagram Generator]
    F --> G[HTML and SVG Diagram Artifacts]
    G --> H[Engineer Review]
    H --> I[Revision Loop]
    I --> F
    H --> J[Approved Architecture Package]
    J --> K[Commit to Repo and Publish Docs]

    L[Optional Python Automation via claude-agent-sdk-python] --> C
    L --> E
```

## Usage

- Fill `playbooks/architecture-spec-template.md` first.
- Feed the resulting architecture block into `architecture-diagram-generator`.
- Save outputs as versioned artifacts next to project docs.
