# Authored curriculum

Content-only extraction from VelQuantumTechnologies/VocoFlo-TheApp at commit aefd245e4d049a83f3ff7bc82d1ffbff959e11aa, November 18, 2026.

## What is here

40 tool JSON files preserve all 440 source sections, their full narration, 2,791 authored narration segments, learning goals, exercises, reflection questions, deeper explanations where present and conceptual visual descriptions. Body tools also include the original physical teaching notes. There are 40 focused practice cards and 90 activities (30 reading, 30 description/spontaneous, 30 prepared roleplay).

See [tools index](tools-index.json), [practice index](practices/manifest.json), [practice cards](practice-cards.json) and [provenance](../docs/content-provenance.md).

## How to consume it

- tools/P01.json through P30.json: psychological teaching, 12 source sections each.
- tools/B01.json through B10.json: body teaching, eight source sections each, plus physicalToolNotes.
- sections[].narration is preserved authored prose; sections[].segments is also preserved because segment wording can differ. These are source variants, not instructions to play both versions or concatenate them. Map a deliberate delivery version and do not accidentally duplicate teaching.
- sections[].exercise contains authored prompts/questions/choices rather than screen controls.
- sections[].visual contains conceptual metaphors, labels and alternative text, not a renderer or screen design.
- Practice cards tie each tool to an existing activity through stable IDs.
- Prepared roleplay activities are fixed prompt material. A separately implemented responsive roleplay must not pretend those fixed prompts are adaptive.

## Preservation boundary

Source teaching wording was not rewritten. Source drafts and approval flags remain where applicable; these are not claims of clinical validation or production readiness. Narration sometimes describes fixed rehearsal, screens or missing demonstrations. Preserve the source; adapt delivery explicitly and label the actual experience accurately.

Removed material includes old UI/state/navigation contracts, renderer/timing instructions, API modes, screen actions, infrastructure, source execution plans and commercial limits. No implementation or old design manifest was copied. Source section order/IDs are retained for traceability, not enforced navigation. Content JSON is not an executable application schema.

Do not silently abridge the curriculum, replace it with generic AI explanations or invent physical demonstrations. The new SPEC.md governs app delivery.
