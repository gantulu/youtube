# Scene Workflow

## Scene construction
For each scene establish:
- scene ID;
- start and end timestamp;
- duration;
- visual state;
- action/state transition;
- relevant audio state;
- continuity links to prior/next scenes.

## Boundary rule
A scene boundary must be supported by a meaningful visual, action, temporal, or audio transition. Avoid arbitrary cuts based only on equal durations.

## Continuity rule
Record the scene start state and end state so downstream generation can continue from a known state.
