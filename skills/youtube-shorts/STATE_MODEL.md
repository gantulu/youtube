# Workflow State Model

## State
Each stage uses one of:
- PENDING
- RUNNING
- PASS
- WARNING
- FAIL
- BLOCKED
- REMEDIATE
- COMPLETE

## Required state
Track:
- workflow_status
- current_phase
- input.video_id
- input.youtube_url when supplied
- phase status for Phase 1–7
- blocking_errors
- warnings
- artifacts
- validation_status
- production_status

## Artifact states
Expected handoff artifacts include:
- normalized_input
- analysis_package
- global_reference
- scene_map
- generation_package
- validation_decision
- production_record
- final_artifact_reference

## Transition rules
PENDING → RUNNING → PASS | WARNING | FAIL
FAIL → REMEDIATE → RUNNING
Blocking FAIL prevents downstream execution.
Validation FAIL blocks production.
Production FAIL blocks final completion.
COMPLETE is allowed only after the terminal output requirements are satisfied.

## State integrity
Never mark PASS because a step was attempted. PASS means the relevant contract and gate were actually satisfied.
