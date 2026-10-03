# Phase 1 — Source Inventory

## Authority levels

- **P0-A** — Official Google/Gemini developer documentation
- **P0-B** — Official Google Workspace / Google Vids documentation
- **P1** — Explicit project decisions and locked workflow rules
- **P2** — Validated project examples
- **R** — Reference-only material pending verification

## P0-A — Gemini

| Area | Source | Status |
|---|---|---|
| Video Understanding | https://ai.google.dev/gemini-api/docs/video-understanding | VERIFIED |
| Image Understanding | https://ai.google.dev/gemini-api/docs/image-understanding | VERIFIED |
| Image Generation | https://ai.google.dev/gemini-api/docs/image-generation | VERIFIED |
| Text Generation | https://ai.google.dev/gemini-api/docs/text-generation | VERIFIED |
| Gemini Omni Flash | https://ai.google.dev/gemini-api/docs/omni | VERIFIED |
| Veo Video Generation | https://ai.google.dev/gemini-api/docs/veo | VERIFIED |
| Gemini Models | https://ai.google.dev/gemini-api/docs/models | VERIFIED |
| Gemini API Changelog | https://ai.google.dev/gemini-api/docs/changelog | VERIFIED |

## P0-B — Google Vids

| Area | Source | Status |
|---|---|---|
| Google Vids | https://workspace.google.com/products/vids/ | VERIFIED |
| Google Vids + Gemini Omni Flash | https://workspace.google.com/blog/product-announcements/introducing-gemini-omni-flash-in-google-vids | VERIFIED |
| Google Vids Text-to-Video | https://workspace.google.com/resources/text-to-video/ | VERIFIED |

## OPEN official-source audits

| Area | Required audit |
|---|---|
| NotebookLM | Supported source types, YouTube ingestion, limits, updates/refresh |
| Google Docs | Source/document workflow if retained |
| Google Vids help | Exact UI controls and prompt behavior |
| Current Gemini model choice | Capability, availability, cost, latency, and production suitability |

## P1 — Project knowledge to normalize

- YouTube URL/video ID input
- Full-video analysis before scene generation
- Timeline and timestamp precision
- Visual + audio analysis
- Scene decomposition
- Global reference
- Character/object/environment identity locks
- Scene continuity
- Scene 1 image prompt
- Later scenes image-to-image
- Image-to-video animation
- Video continuation/extend
- Structured scene blueprint
- Validation gate
- No hallucinated observations
- Observed/inferred/unknown separation

## P2 — Examples

Validated examples must be imported from prior project artifacts before being promoted to canonical examples.

## Audit rule

A project rule may depend on an official capability, but it must remain labeled as a project decision. Official documentation is the authority for what the product supports; the project decides how to use that capability.
