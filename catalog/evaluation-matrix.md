# Evaluation Matrix

As-of snapshot: 2026-04-17.

| Project | Primary Value | Integration Effort | License Risk | Best Fit for Sol-HQ | Priority |
| --- | --- | --- | --- | --- | --- |
| claude-mem | Cross-session memory and compression | Medium | High (AGPL) | Internal R&D only; not embedded in closed/proprietary code | P1 |
| open-agents | Cloud runtime for coding agents | High | Low (MIT) | Agent infrastructure experiments and hosted coding workflows | P1 |
| cognee | Knowledge engine + graph memory | Medium | Low (Apache-2.0) | Agent memory layer for Solana workflows and docs retrieval | P1 |
| magika | AI file type detection + safety routing | Low | Low (Apache-2.0) | Upload pipelines, scanner inputs, and content validation | P1 |
| andrej-karpathy-skills | Better coding-agent behavior rules | Low | Unknown | Prompt/rule standards across all repos | P1 |
| GenericAgent | Self-evolving local automation | Medium | Low (MIT) | Internal automation bench, skill-tree ideas | P2 |
| evolver | Protocolized prompt evolution loop | Medium | Medium (GPL-3.0) | Research-only optimization workflow | P2 |
| voicebox | Local voice cloning/synthesis studio | Medium | Low (MIT) | Voice-enabled agents and notification pipelines | P2 |
| omi | Ambient capture + assistant stack | High | Low (MIT) | Product inspiration, not immediate drop-in | P3 |
| Kreo | Polymarket copy-trading bot | N/A | Closed-source | Operational benchmark only | P3 |

## Adoption guardrails

- Validate legal and license boundaries before mixing AGPL/GPL projects into production repos.
- Start with MIT/Apache projects for production-path prototypes.
- Keep closed-source services as benchmark references, not core dependencies.
