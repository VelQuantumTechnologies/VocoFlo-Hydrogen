# Speech analysis integration

## Founder decision

Chetan has already tested the Gemini audio-analysis API and reports good detection. Integrate it now and test in the app. A separate annotated-corpus study is not a prerequisite.

No production model ID, endpoint, prompt, request example or credentials were supplied in this conversation. No old integration code/prompts were copied because the founder authorized content-only transfer. Obtain the working request details securely when wiring the real adapter. Meanwhile scaffold the interface and a clearly labelled development fixture; do not present fixtures as live results.

Audio understanding receives recordings and returns observations. TTS produces voice. Keep these responsibilities separate. Do not switch provider or claim the same exact model without identifying the current configuration.

## Suggested normalized response

Hydrogen may refine the internal contract. Preserve these distinctions:

- attemptId, analysisId, provider, model, adapterVersion, status.
- Recording-relative duration and event start/end in seconds.
- Event ID, type (repetition, prolongation, pause, other/uncertain), optional word/sound and tentative observation.
- source: ai_observed versus user_reported.
- review state: unreviewed, confirmed, dismissed or corrected.
- Optional transcript; retain disfluent wording when available instead of assuming a cleaned transcript preserves events.
- Never fabricate calibrated confidence values. Provider confidence, if present, is not validated detection accuracy.

Silence alone may only yield a pause or gap, never an automatically asserted silent block. A learner may separately report that a moment felt blocked.

## Response handling

Validate finite times: 0 <= start < end <= recording duration. Reject/flag malformed or out-of-range events rather than silently clamping them into plausible markers. Preserve raw provider response only under the chosen privacy/retention policy. Empty events is a valid result. Failed analysis is not zero events.

Use recording-relative times in playback and readable minutes:seconds labels. One tap should seek to the relevant point without forced playback. Let the learner dismiss/correct an event or say that an observation is helpful.

## When analysis runs

Use it in the free check-in and selected high-value lesson comparisons, explicit "Inspect with Coco" requests, and selected roleplay review. Do not re-analyse an unchanged recording on reopening history or re-rendering a screen. Ongoing local/static practice remains usable without analysis.

Coco may use conversational transcription/understanding during live roleplay; that is distinct from running a disfluency-analysis request after every turn. Log both purposes separately.

## In-app testing and failure recovery

Allow Chetan to test repetitions, prolongations, pauses, varied contexts and timestamp seeking during ordinary app use. Capture corrections and timing problems. No public accuracy percentage follows from these tests.

Handle no microphone permission, empty/short audio, interrupted upload, timeout, malformed JSON, quota exhaustion and provider failure. Preserve the attempt when appropriate and offer retry, continue without analysis or finish. Prevent duplicate billing on repeated taps and avoid automatic upload retries after cancellation. Never block authored lesson progression because analysis failed.
