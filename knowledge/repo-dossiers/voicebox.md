# voicebox

- Source: [jamiepine/voicebox](https://github.com/jamiepine/voicebox)
- Category: Local-first voice synthesis and cloning studio
- Snapshot stars (2026-04-17): 19,591
- License: MIT
- Language: TypeScript

## What it gives you

A local voice stack with multiple TTS engines, multilingual support, effects, and an API-first architecture.

## Why this matters for Sol-HQ

- Add voice outputs to agent dashboards and execution alerts.
- Build voice-first onboarding or assistant workflows.
- Keep sensitive voice generation local when needed.

## Risks and caveats

- Hardware requirements vary by model/engine.
- Voice cloning workflows may trigger policy/compliance obligations.
- Production quality depends on model selection and tuning.

## Recommended usage

- Start with non-cloning TTS for alerts and summaries.
- Add strict content policy checks for generated audio.

## First implementation step

Prototype a local notification service that converts critical bot events into spoken alerts.
