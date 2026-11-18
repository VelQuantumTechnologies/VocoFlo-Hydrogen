# Data and telemetry

These are logical entities, not a mandated SQL schema or cloud vendor.

| Entity | Minimum useful fields |
| --- | --- |
| Learner | ID, locale, chosen goals, recording/privacy preferences |
| Content | tool/activity ID, source version, delivery version |
| Session progress | learner, lesson, current delivery step, completed/skipped states, checkpoint |
| Attempt | learner, session/activity, context, duration, recording reference/local state, creation time, upload state |
| Analysis | attempt, provider/model/adapter version, status, timestamped observations, error category |
| Event correction | analysis/event, learner decision, amended label/times if provided, original event, timestamp |
| Self-report | attempt/session, optional effort value and scale, optional avoidance/attention/participation note, source |
| Coach memory | fact, source kind/reference, last confirmed time, user edit/delete state |
| Transfer plan | chosen situation, one small action, optional review observation |
| Entitlement | content access, live-AI start/end, allowance configuration version, usage counters |
| Usage ledger | request ID, operation ID, attempt/session, provider/model, purpose, status, actual units, pricing version, calculated cost |

## Measurement rules

Purpose labels should distinguish authored-audio generation, assessment analysis, lesson analysis, requested inspection, conversational understanding, coaching text and dynamic voice.

Log units actually supplied by the provider: input/output/cached tokens, audio seconds, TTS characters or audio tokens as applicable. Missing units/cost are unknown, not zero. Include latency, retries, provider request ID and error outcome. Never log keys or full private audio/transcripts in a general telemetry sink.

Costs must use versioned rates with currency, effective date and source. Distinguish estimated per-call costs from reconciled billed costs. Track infrastructure/storage separately; API spend alone is not gross margin. Track one-time narration generation separately from recurring per-learner costs.

## Reliability and privacy

Use an operation ID/idempotency mechanism to prevent duplicate paid requests and quota charges. Only confirmed usage changes the appropriate ledger/counter under the chosen charging policy. Preserve failed request records even if their cost is unknown.

Isolate users' recordings, notes and memories. Store credentials server-side, use protected access to uploaded audio and avoid audio in git. Provide recording deletion and memory correction/deletion. A private reflection must not be sent to a model or memory store by default. Explain what gets uploaded before the first analysis. Define actual retention, export and deletion behaviour before production use.

## Commercial configuration

Keep $499, service duration, quotas, renewals and free limits configurable. Until approved, development entitlements must be labelled and must not create a real purchase or a lifetime-AI promise. Do not silently downgrade paid features when a quota is reached; clearly distinguish static practice from unavailable live services.
