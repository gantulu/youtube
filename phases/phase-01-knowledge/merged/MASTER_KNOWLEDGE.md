# Phase 1 — Master Knowledge

## Purpose
Canonical merged knowledge for the YouTube Shorts AI system. This document reconciles normalized product facts with explicit project decisions without conflating them.

## Authority model
- P0-A: Official Google AI / Gemini documentation.
- P0-B: Official Google Workspace / Google Vids documentation.
- P1: Explicit project decisions.
- P2: Validated project examples.
- R: Unverified/reference material.

Higher authority controls product capability claims. P1 controls how this project chooses to use those capabilities.

## 1. Video understanding
Gemini Video Understanding can accept public YouTube URLs and analyze visual and audio streams. Static processing defaults to 1 FPS; custom sampling is available. Rapid motion or quick cuts can be missed at 1 FPS. Agentic processing is model-dependent. Timestamps are represented as MM:SS.

### Project rule
The analyzer must complete internal multimodal analysis before emitting scenes, cover the complete timeline, verify rapid events when needed, and distinguish observed, inferred, and unknown information.

## 2. Video generation
Gemini Omni and Veo are generation layers separate from video understanding. Current official documentation describes Omni capabilities including image-to-video, interpolation, editing, and extension. Current Veo documentation describes Veo 3.1 with 8-second generation, native audio, 9:16/16:9, image-based generation, interpolation, references, and extension.

### Project rule
Generation stages remain explicit: image anchor/reference → image-to-image where needed → image-to-video animation → extension/continuation. Exact model IDs and limits are versioned and must be rechecked against current official documentation.

## 3. NotebookLM / Gemini Notebook
Official Gemini Notebook documentation supports textual and multimodal source types including Docs, Slides, Sheets, images, audio, Markdown, text, PDF, CSV, DOCX, PPTX, web URLs, and public YouTube URLs with captions. For YouTube sources, the imported source is the transcript text rather than frame-level video evidence.

### Project rule
NotebookLM is the knowledge/reference layer. It is not the primary frame-level visual analyzer. GitHub is the canonical versioned project-of-record; NotebookLM is the knowledge workspace.

## 4. Global reference and continuity
The project maintains stable references for characters, objects, environment, visual style, camera, composition, lighting, and relevant audio. Persistent IDs and scene start/end states are used to enforce continuity.

These are project controls, not guarantees of native model identity persistence.

## 5. Scene generation contract
Scene 1 establishes the visual anchor. Later scenes can use image-to-image references for continuity. Image-to-video and extension are separate operations. Scene output is emitted only after analysis completion and validation gates.

## 6. Validation contract
Validate timeline coverage, scene boundaries, prompt alignment, visual continuity, animation continuity, audio/narration continuity, and cross-scene identity.

## 7. Non-negotiable distinctions
- Understanding ≠ generation.
- Image-to-image ≠ image-to-video.
- Extension ≠ restarting a scene.
- Official capability ≠ project workflow decision.
- 1 FPS default ≠ guarantee of complete temporal capture.
- NotebookLM transcript source ≠ frame-level video analysis.

## 8. Volatility
Model identifiers, availability, limits, pricing, and UI behavior can change. Treat current official documentation as the source of truth whenever these values are used operationally.
