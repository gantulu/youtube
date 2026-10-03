# YouTube Shorts AI — Project Rules

## Authority
P1 — Explicit project decisions. These are project-level controls, not native Gemini guarantees.

## Input
Accept and normalize a public YouTube Shorts URL or video ID.

## Analysis gate
Analyze the actual video before output. Cover the complete timeline, inspect visual and audio evidence, preserve timestamps, distinguish observed/inferred/unknown, and avoid hallucination.

## Global Reference
Maintain stable references for characters, objects, environment, visual style, camera, composition, lighting, and relevant audio characteristics.

## Continuity
Use persistent character/object IDs where applicable. Preserve start/end state, identity, spatial/environment continuity, and action continuity.

## Generation pipeline
1. Scene 1 establishes the visual anchor.
2. Later scenes may use image-to-image references for continuity.
3. Image-to-video is a separate animation stage.
4. Extension is a separate continuation stage.

## Output gate
Emit the structured scene blueprint only after analysis completion and validation.

## Validation
Check timeline coverage, boundaries, prompt alignment, visual continuity, animation continuity, audio/narration continuity, and cross-scene identity.

## Change control
These rules are locked. Change only through an explicit project version update.
