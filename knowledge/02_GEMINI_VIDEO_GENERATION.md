# Gemini Video Generation

## Authority
P0-A — Official Google AI for Developers.

## Sources
https://ai.google.dev/gemini-api/docs/omni
https://ai.google.dev/gemini-api/docs/veo

## Capability layer
Gemini Omni and Veo are video-generation technologies and are separate from Video Understanding.

Current official Omni documentation describes image-to-video, first/last-frame interpolation, editing, reference-to-video, and extension. Current Veo documentation describes Veo 3.1 with 8-second generation, native audio, portrait 9:16 and landscape 16:9, image-based generation, interpolation, references, and extension.

## Project operating rule
Use explicit motion/camera/environment instructions. Treat extension as continuation from the current end state. Keep model identifiers and limits versioned and revalidate them against current official documentation.

## Important boundary
Do not encode current model IDs as permanent prompt rules.
