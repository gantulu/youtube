# Extension Planning

## Purpose
Extension is used when the next generated segment should continue from an existing clip.

## Continuation contract
Describe the next action, motion, camera continuation, environment continuation, lighting/audio continuity, and intended end state as supported by the scene plan.

## Critical rule
Extension starts from the current clip end state. It must not restart the scene or silently reset character/object/environment state.

## Model/version rule
Current model identifiers, duration limits, and UI capabilities must be checked against official documentation at execution time.
