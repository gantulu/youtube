# Normalized Knowledge — Gemini Video Generation

## Authority
P0-A — Official Google AI for Developers documentation.

## Canonical sources
- Gemini Omni Flash: https://ai.google.dev/gemini-api/docs/omni
- Veo: https://ai.google.dev/gemini-api/docs/veo

## Gemini Omni Flash facts

The current Omni documentation describes:
- image-to-video generation;
- first/last-frame interpolation;
- video editing;
- video extension;
- task modes including text_to_video, image_to_video, reference_to_video, edit, and extend.

The documented model identifier is `gemini-omni-1.1-flash`. Model identifiers must be revalidated against the current model catalog before production use.

Image-to-video quality benefits from high-resolution reference images and specific descriptions of subject motion, camera movement, and environmental effects.

Video extension appends a continuation to the end of a clip. The current documentation describes generated continuations of 3–10 seconds.

## Veo 3.1 facts

The current Veo documentation describes Veo 3.1 as an 8-second video generation model with native audio.

Documented capabilities include:
- portrait 9:16;
- landscape 16:9;
- image-based generation;
- first/last-frame interpolation;
- reference images;
- extension of previously generated Veo videos.

## Project interpretation

1. Generation and understanding are separate stages.
2. Image-to-video prompts should explicitly describe subject motion, camera motion, and relevant environmental/lighting motion.
3. Extension prompts must describe continuation from the current end state, not restart the scene.
4. A project may use scene 1 as an image-generation anchor and later scenes as image-to-image or continuation stages, but this is a project workflow decision rather than a model guarantee.
5. Exact model IDs and duration limits must remain version-controlled and be checked against current official documentation.

## Important distinction

Do not merge:
- Gemini Video Understanding
- Gemini Omni generation
- Veo generation
- Google Vids UI workflows

They are separate capability layers.
