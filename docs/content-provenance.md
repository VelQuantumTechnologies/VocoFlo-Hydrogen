# Content provenance

Source: VelQuantumTechnologies/VocoFlo-TheApp, main snapshot commit aefd245e4d049a83f3ff7bc82d1ffbff959e11aa. Source was read only. Destination is a new implementation repository.

Transfer scope was explicitly limited by Chetan to authored tools and content. Source code, system prompts, old specifications, screen contracts, design assets/renderer plans, infrastructure, pricing configuration and runtime schemas were not copied.

## Transformation

- Psychological session JSON: preserved teaching metadata, all narration/segments, learning goals, conceptual visuals, exercises and deeper explanations; renamed blocks to sections and interaction to exercise.
- Full body session JSON: same content-only extraction, supplemented with authored physical teaching notes from body blueprints.
- Practice cards: preserved authored purpose/instructions/reflection and stable content references; removed API/timing/execution policies.
- Activities: preserved passages/scenarios/prompts/steps/reflection; removed runtime mode, timing, turn/audio limits and analysis policy.
- Practice index: retained IDs/titles/content paths.

Source UI, next pointers, transition contracts, target durations, presentation contracts, visual renderer plans and asset routing were omitted. There is no inherited framework requirement. Conceptual visual descriptions are educational material, not mandatory old screen layouts.

No substantive teaching prose was intentionally changed. Existing source text about a fixed rehearsal stays in source; a live-mode delivery adapter must not narrate a fixed-mode disclosure. Approval flags remain source status only.

content-source-map.json identifies every imported source path and original Git blob SHA, including supplementary body notes. Narration and segment preservation were checked by exact string/object comparison before commit; the result is in content-transfer-check.json.

The attached PDF came from a different snapshot and was not substituted for this user-specified repository source. No media asset binaries were included. Body-tool demonstration notes describe intended material; they do not establish that approved demonstration audio/video exists.
