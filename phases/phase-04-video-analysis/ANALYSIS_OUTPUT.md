# Analysis Output Contract

The analysis layer produces an internal evidence package for downstream workflow stages.

## Required contents
- canonical video identifier;
- complete timeline;
- timestamped visual observations;
- timestamped audio observations;
- temporal verification findings;
- persistent character/object references where applicable;
- environment and visual-language references;
- scene start/end states;
- observed/inferred/unknown classification;
- unresolved uncertainties.

## Output boundary
This package is an intermediate artifact. It must not be treated as the final scene blueprint and must not trigger generation before the analysis completion gate passes.
