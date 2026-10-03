# Phase 1 — Project Decisions

## Status
Locked unless the project explicitly declares a version update.

## Input
- Public YouTube Shorts URL or video ID.
- Normalize input before analysis.

## Analysis
- Analyze the actual video, not title/metadata alone.
- Complete internal analysis before scene output.
- Cover the complete timeline.
- Analyze visual and audio evidence together.
- Preserve timestamp precision.
- Separate observed, inferred, and unknown.
- Never invent unsupported details.

## Global Reference
Track stable character, object, environment, visual style, camera, composition, lighting, and relevant audio characteristics.

## Continuity
Use persistent IDs where applicable. Preserve scene start/end state, identity, spatial/environmental continuity, and action continuity.

## Generation
- Scene 1: visual anchor/image prompt.
- Later scenes: image-to-image references where continuity benefits.
- Animation: image-to-video stage.
- Continuation: extension stage.

## Output
Structured scene blueprint only after the analysis completion gate.

## Validation
Timeline, boundaries, prompt alignment, visual continuity, animation continuity, audio/narration continuity, and cross-scene identity must be checked.
