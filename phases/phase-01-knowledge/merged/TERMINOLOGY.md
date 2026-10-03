# Phase 1 — Canonical Terminology

| Term | Canonical meaning |
|---|---|
| Video Understanding | Multimodal analysis of video content, including visual/audio evidence. |
| Static processing | Video processing using a configured sampling rate; official default is 1 FPS. |
| Agentic processing | Model-dependent processing that can dynamically navigate video evidence. |
| Global Reference | Project-level stable description used to preserve identity/style/continuity across scenes. |
| Image-to-Image | Image generation/editing conditioned on a reference image. |
| Image-to-Video | Video generation conditioned on an image/reference and motion instructions. |
| Extension | Generation that continues an existing clip from its end state. |
| Scene Anchor | The first visual reference established for downstream scene continuity. |
| Identity Lock | Project validation rule requiring stable character/object identity. |
| Analysis Gate | Requirement that internal video analysis is complete before scene output. |
| Validation Gate | Requirement that generated scene structure and continuity checks pass before production. |
| NotebookLM | Knowledge/reference workspace for imported sources. |
| GitHub | Canonical versioned repository for project artifacts. |
