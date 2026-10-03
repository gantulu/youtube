# Prompt Validation

## Stage alignment
Verify that each prompt belongs to the correct generation stage:
- image;
- image-to-image;
- image-to-video;
- extension.

## Alignment
Prompt instructions must correspond to the intended scene state and source evidence.

## Separation
Static visual instructions must remain distinct from temporal motion instructions where the downstream stage expects separation.

## Product volatility
Do not treat model IDs, limits, or current UI behavior as valid merely because they appear in a prompt. Operational product facts require current official documentation.
