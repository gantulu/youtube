# Prompt Contract

## Prompt layers
1. **Image prompt** — defines the target visual state.
2. **Image-to-image prompt** — defines target transformation from a reference state.
3. **Image-to-video prompt** — defines temporal motion and audiovisual behavior.
4. **Extension prompt** — defines continuation from the current end state.

## Common controls
Prompts should preserve evidence-grounded subject identity, environment, composition, camera, lighting, action, and relevant audio requirements.

## Separation of concerns
Do not mix a static visual specification with temporal motion instructions when the downstream generation stage expects them separately.

## Volatile parameters
Do not hard-code current model IDs, limits, or product UI behavior into permanent project rules.
