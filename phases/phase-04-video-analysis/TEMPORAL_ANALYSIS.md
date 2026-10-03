# Temporal Analysis

## Sampling principle
Gemini Video Understanding documents static processing at 1 FPS by default and supports custom sampling. Low sampling can miss rapid motion and quick scene changes.

## Required procedure
1. Establish full timeline coverage.
2. Identify cuts, transitions, rapid actions, and ambiguous moments.
3. Determine whether the active sampling strategy could have missed an event.
4. Perform additional temporal verification when risk exists.
5. Preserve the verified event timestamp.

## Rule
Do not infer that an event did not occur merely because it was absent from a low-rate sample.
