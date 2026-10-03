# Gemini Skill — Output Contract

## Default behavior
The Skill performs internal analysis first and emits only the requested structured scene blueprint after the analysis completion and validation gates.

## Principles
- Do not expose speculative analysis as fact.
- Preserve observed/inferred/unknown distinctions.
- Use canonical project terminology.
- Preserve timeline precision.
- Keep product facts separate from project decisions.
- Do not silently change locked project rules.

## Scene-generation contract
- Scene 1 is the visual anchor and receives the image-generation prompt.
- Later scenes may receive image-to-image prompts referencing the established visual anchor/reference.
- Image-to-video animation is a separate prompt stage.
- Extension is a separate continuation prompt stage.

The exact final scene schema remains governed by the project schema version. This contract defines behavior, not a replacement schema.
