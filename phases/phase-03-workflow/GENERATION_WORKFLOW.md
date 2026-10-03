# Generation Workflow

## Order
1. Establish Scene 1 image anchor.
2. Generate or plan Scene 1 animation separately.
3. For later scenes, use image-to-image references when needed to preserve identity/style continuity.
4. Generate or plan image-to-video motion separately.
5. Use extension only when the desired result is continuation from an existing clip end state.

## Prompt separation
Image prompts describe visual state. Image-to-image prompts describe the target transformation while preserving the reference identity. Image-to-video prompts describe motion/camera/environment/lighting/audio behavior. Extension prompts describe the next action and continuation from the current end state.

## Model volatility
Specific model IDs, limits, and UI behavior are not hard-coded here; consult current official documentation when operational execution requires them.
