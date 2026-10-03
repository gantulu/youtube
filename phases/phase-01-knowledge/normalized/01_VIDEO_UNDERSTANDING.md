# Normalized Knowledge — Gemini Video Understanding

## Authority
P0-A — Official Google AI for Developers documentation.

## Canonical source
https://ai.google.dev/gemini-api/docs/video-understanding

## Product facts

### Inputs
- Gemini can process video from File API, Cloud Storage registration, inline data, and public YouTube URLs.
- YouTube URL input is specifically documented for public YouTube videos.
- Video understanding uses both visual and audio streams.

### Temporal processing
- Static processing is the default and samples video at 1 FPS.
- Custom FPS can be configured.
- Static 1 FPS can miss rapid motion or quick scene changes.
- Current supported models may also provide agentic processing, where the model dynamically navigates the timeline and loads transcript, frames, and/or audio as needed.
- Agentic processing is model-dependent and must not be treated as a universal Gemini capability.

### Timestamps
- Timestamp references use MM:SS.
- Video-understanding prompts can request salient moments with timestamps.

### Media resolution
- Media resolution is independent of processing mode.
- Higher resolution can improve recognition of fine details but increases token usage and latency.

## Project interpretation

These are project decisions, not product guarantees:

1. A Shorts analyzer should inspect the complete timeline before producing scene output.
2. Fast-motion or rapid-cut content requires verification beyond assuming 1 FPS is sufficient.
3. Timeline coverage, scene boundaries, and continuity must be represented explicitly.
4. Audio and visual evidence must be analyzed together.
5. Observed facts, inference, and unknowns must remain distinguishable.
6. The analyzer should not claim details that are not supported by the video evidence.

## Non-goals
- This document does not define the Gemini Skill output schema.
- This document does not define image/video generation behavior.
- This document does not guarantee character consistency.

## Normalization rule
When product behavior changes, update this document from the official source first, then update dependent project rules.
