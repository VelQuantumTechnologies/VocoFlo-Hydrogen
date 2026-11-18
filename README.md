# VocoFlo — Hydrogen handoff

VocoFlo is an audio-first speaking coach for adults who stammer. Coco teaches authored tools, listens, supports practice and remembers what the learner chooses to share. Founded by Chetan, VelQuantum Technologies.

This repository starts a fresh implementation. It contains product requirements from the November 18, 2026 conversation and the existing authored curriculum only. Hydrogen owns the architecture, visual design and implementation decisions within these requirements.

## Start here

1. Read [AGENTS.md](AGENTS.md), then [SPEC.md](SPEC.md).
2. Read [Phase 1](docs/phase-1.md) and [Coco behaviour](docs/coco-behaviour.md).
3. Read [Speech analysis](docs/speech-analysis.md), [data and telemetry](docs/data-and-telemetry.md), and [open decisions](docs/open-decisions.md).
4. Explore [the content index](content/README.md) and [provenance](docs/content-provenance.md).
5. Use [HANDOFF.md](HANDOFF.md) as the implementation starting brief.

## Inventory

- 30 psychological tools: P01–P30, full authored scripts.
- 10 body tools: B01–B10, full authored scripts and physical teaching notes.
- 40 focused practice cards.
- 90 activities: reading, spontaneous/description and prepared roleplay.

Content remains review-draft material; availability does not imply commercial or clinical validation. Authored wording has been preserved during content-only extraction. Existing app UI, navigation, infrastructure, prompts, pricing policies and code have not been imported.

## Current decision

Integrate the existing Gemini speech-analysis approach now and test it in the app. Chetan has already tested it and reports good event detection. Do not require a separate pre-build audio-validation study. Exact API model, endpoint and credentials still need to be supplied; do not invent them.

## Build target

First deliver a working assessment → P01 experience → responsive roleplay → saved follow-up. Make it testable by Chetan before expanding the catalogue or adding elaborate dashboards. This handoff contains no app implementation and no production payment configuration.
