# Normalized Knowledge — Project Rules

## Authority
P1 — Explicit project design decisions.

These rules are not claims about native Gemini behavior.

## Input
- Accept a public YouTube Shorts URL or video ID.
- Normalize the input before analysis.

## Analysis
- Analyze the actual video rather than relying only on title or metadata.
- Complete internal analysis before producing scene output.
- Cover the complete timeline.
- Track visual and audio information.
- Preserve timestamp precision.
- Separate observed, inferred, and unknown information.
- Do not hallucinate missing details.

## Global reference
Create a global reference describing stable:
- characters;
- objects;
- environment;
- visual style;
- camera language;
- composition;
- lighting;
- relevant audio characteristics.

## Continuity
Use persistent IDs for important characters and objects.
Scene boundaries must preserve:
- start state;
- end state;
- identity;
- spatial/environmental continuity;
- action continuity.

## Generation workflow
- Scene 1 establishes the visual anchor.
- Later scenes may use image-to-image references to improve visual continuity.
- Image-to-video is a distinct animation stage.
- Extension is a distinct continuation stage.

## Output
Produce a structured scene blueprint only after the analysis completion gate passes.

## Validation
Validate:
- timeline coverage;
- scene boundaries;
- prompt alignment;
- visual continuity;
- animation continuity;
- audio/narration continuity;
- cross-scene identity.

## Locked project decisions
These rules should not be silently changed during normalization. Any deliberate change requires an explicit project version update.
