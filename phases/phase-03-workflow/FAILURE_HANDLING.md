# Failure Handling

## Input failure
Stop. Return the input problem and required correction.

## Video unavailable
Stop scene generation. Do not substitute metadata, thumbnail, or unsupported assumptions for missing video evidence.

## Incomplete analysis
Return to the missing analysis pass. Do not emit final scenes.

## Ambiguous evidence
Mark the detail as unknown or inferred according to evidence strength. Do not fabricate certainty.

## Sampling risk
Perform additional temporal verification when rapid motion or quick cuts may have been missed.

## Continuity failure
Return to Global Reference and Scene Workflow; repair the reference/state mapping before prompt generation.

## Validation failure
Do not emit production-ready output. Identify the failing contract and route back to the responsible workflow stage.
