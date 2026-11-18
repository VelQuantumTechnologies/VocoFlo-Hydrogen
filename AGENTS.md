# Instructions for Hydrogen and other implementers

## Ownership and boundaries

Build VocoFlo freshly in this repository. Do not import implementation, design, infrastructure, prompts, execution contracts or commercial policies from VocoFlo-TheApp or another earlier VocoFlo repository. Only the authored tool/practice material in content/ was brought forward with Chetan's authorization.

Use your judgment for framework, backend, database, visual design and code structure. Do not interpret example data entities as a mandated database or screen routes as a mandated framework. Aim for a polished, finishable app, and implement rather than repeatedly redesigning the blueprint.

## Required reading and precedence

Read SPEC.md and docs/phase-1.md before coding. Read content/README.md before consuming the curriculum. New product specifications govern delivery; source content preserves teaching meaning. Old authored references to fixed prompts do not turn those prompts into adaptive conversation. Never silently rewrite the curriculum to resolve an implementation conflict: preserve the source and document a small delivery adaptation separately.

Current user instructions take precedence over this handoff. Open commercial decisions are not authorization to sell an invented package.

## Working rules

- Preserve the curriculum's meaning and complete source text. Do not replace it with generic AI advice.
- Keep the experience audio-first with accessible reading controls and explicit microphone actions.
- Make lesson progression deterministic; Coco can answer naturally without inventing course completion or changing the curriculum.
- Implement speech analysis now. No separate pre-build accuracy gate. Use in-app testing and corrections.
- Keep API keys server-side. Do not copy secrets or user recordings into git.
- Distinguish real integrations, test fixtures and unavailable services. Never show invented analysis or fabricated remembered facts.
- No acoustic inference of shame, anxiety, avoidance, tension, attention or motivation. Ask the learner.
- No live coaching banners, grading or event alerts while the learner speaks.
- One salient primary action per state. Error recovery must leave a usable continuation.
- Optional self-report must stay optional; don't turn every attempt into a questionnaire.
- Responsive roleplay must react to the answer. Prepared rehearsal must be described accurately.
- Keep repeated static practice available without a paid analysis call.
- Test meaningful user paths and recovery states. Report what was actually run and what still requires a device or real credentials.

## First milestone

Follow docs/phase-1.md. Do not make full catalogue animation, a dashboard suite, a provider migration or production payments prerequisites for the first usable build.
