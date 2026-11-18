# VocoFlo product specification

Status: implementation handoff, November 18, 2026. Product decisions below come from the current founder conversation. Technical choices remain Hydrogen's responsibility.

## 1. Product promise and coaching boundaries

Coco is an audio-first AI speaking coach for adults who stammer, including people who speak easily alone and struggle with listeners. It teaches concrete tools, guides speaking practice and supports real conversations. The method combines authored lessons with relevant AI interaction and cross-session memory.

Position the product positively around useful practice, easier participation and meaningful communication. Do not guarantee fluency or imply that fluency is impossible. Do not market this draft curriculum as clinically proven or Coco as a human speech therapist.

Separate audible observations, learner-reported experience and tentative coaching hypotheses. A fluent sample does not cancel a report of difficulty. A pause is not automatically a block. Users can correct Coco. No forced exposure or demand to manufacture discomfort.

## 2. Offer and entitlements

The initial speaking check-in is free and must provide useful feedback before the paid invitation. The intended paid price is approximately US$499; it is a target, not a configured commercial offer.

Separate access to authored content from a defined live-AI service entitlement. Duration, monthly allowances, renewal, taxes, refunds and exact free limits remain undecided. Do not advertise lifetime AI, six/twelve months or numeric allowances as approved.

Repeated local/static practice does not require paid AI analysis. Cache authored narration where appropriate. Selective analysis and dynamic voice/roleplay consume live services. Log actual usage before setting commercial quotas. No speculative margin claims.

## 3. Core flows

### Free speaking check-in

Explain what will be recorded/shared; let the user start each recording. Obtain a little context: situations that matter, the user's goal and optional effort/avoidance experience. Offer short reading, spontaneous speaking and a brief conversational exchange; exact count/durations can be piloted. Do not claim an app exchange reproduces real listener pressure.

Use actual Gemini analysis and a concise Coco debrief. Surface what is known, ask about what is not, and offer one useful tool experiment. If little stammering is detected, respect the learner's reported difficulty. Timeline inspection is optional. Let the learner experience a brief teaching/practice moment before inviting purchase. Do not manufacture severity or fear to sell.

### Experiential tool session

Short welcome and relevant remembered context → early micro-attempt or scenario response → explanation and meaningful visual → one small experiment → rehearsal → brief review and one real-world transfer step.

Retain the 12 authored psychological sections as source material; they are not twelve compulsory screens. Body tools have eight source sections. Reorder delivery through an explicit mapping without discarding the source text or introducing unreviewed physical mechanics. Exact session duration and total course calendar are not fixed.

Coco answers questions and returns to the lesson location. Short specific encouragement is welcome when supported by the user's action. Use deeper explanation when teaching or answering a substantive question, not as a template for every turn.

### Practice

Provide reading, spontaneous speaking and roleplay. Prepared prompts support repeated practice without live coaching costs; live roleplay responds naturally and can use a distinguishable partner voice. Keep character dialogue separate from Coco's debrief. Offer difficulty/context choices; do not force hostile or interrupting personas.

### Review and history

Default review: message → optional effort/experience → at most one focused Coco observation/question → keep, adjust or finish. Invite effort, word substitution/avoidance and attention reports through a light optional input, not three mandatory questions every time.

History prioritizes participation, user observations, active tools and transfer steps. Keep timestamped moments and acoustic trends inside an optional "Inspect Speech Moments" view. No mandatory replay, fluency grades or celebratory event-count reductions.

## 4. Coco intelligence

Use authored teaching as the stable curriculum. Use AI for context-aware openings, grounded debriefs, relevant examples, learner questions and responsive roleplay. Memory spans sessions, with editable user-reported goals, contexts, active tools and plans. A skipped self-report is unknown, not zero effort.

Explain meaning through a concrete experience, a non-shaming explanation and a useful example/experiment when that depth helps. Do not diagnose a nervous-system mechanism from a recording or present a metaphor as physiology.

See docs/coco-behaviour.md for examples and memory rules. OpenAI intelligence is the founder's initial preference; Gemini remains the existing analysis approach. No all-Gemini migration is approved. Select exact current models and voice through practical testing.

## 5. Data and measured operating costs

Keep lesson state, attempts, optional analysis, self-report, corrected events, learner memory and entitlements separately identifiable. Record provider/model, request purpose, actual usage and failures. Separate raw analysis from learner corrections and retain provenance. See docs/data-and-telemetry.md.

Use transparent recording/upload controls and appropriate account isolation. Local/private journal material must not automatically become AI memory. Actual retention and deletion behaviour must be documented.

## 6. First build and in-app analysis testing

Deliver one complete path with real audio analysis, one meaningful teaching visual, responsive roleplay and a remembered follow-up. Integrate now; Chetan will assess the detection inside the app. This supersedes the earlier proposed 15–20-recording pre-build gate.

Validate timestamps and response structure, let users dismiss/correct moments, and keep practice usable through service failures. Test app behaviour and record actual costs. Do not claim detector accuracy from the founder's exploratory test alone.

Phase 1 acceptance checks are in docs/phase-1.md. Full expansion follows a usable first build.
