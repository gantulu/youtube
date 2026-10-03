# Operational Workflow

## Stage 0 — Input
Receive a public YouTube Shorts URL or video ID.

Output: normalized video identifier.

## Stage 1 — Access Check
Confirm that the actual target video can be inspected. Metadata-only evidence is insufficient.

Output: video evidence available / blocked.

## Stage 2 — Full Video Analysis
Inspect the complete timeline using the available video-understanding capability. Analyze visual and audio evidence, timestamps, scene changes, dialogue/narration/music/SFX, and relevant text overlays internally.

If sampling may miss rapid events, perform additional verification using an appropriate supported processing strategy.

Output: evidence set + timeline observations.

## Stage 3 — Global Reference
Create stable references for characters, objects, environment, visual style, camera, composition, lighting, and relevant audio characteristics. Assign persistent IDs where useful.

Output: Global Reference.

## Stage 4 — Scene Decomposition
Segment the video into coherent scenes. Every scene must have a start/end timestamp and a supported description of its state/action. Check for gaps and overlaps.

Output: scene map.

## Stage 5 — Prompt Planning
Only after analysis and scene decomposition. Scene 1 establishes the visual anchor. Later scenes may use image-to-image references. Animation and extension prompts remain separate.

Output: generation prompt plan.

## Stage 6 — Validation
Validate timeline, boundaries, evidence alignment, continuity, identity, animation, and audio/narration.

Output: validation result.

## Stage 7 — Final Output
Emit only the project-defined structured scene blueprint when required gates pass.
