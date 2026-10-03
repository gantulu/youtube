# Phase 3 — Workflow

## Objective
Convert the Phase 2 Gemini Skill into a deterministic operational workflow that can be executed consistently in Gemini Native and supported knowledge workflows.

## Design
The Skill defines behavior; this phase defines execution order, checkpoints, inputs/outputs, failure handling, and handoff artifacts.

## Workflow
INPUT → NORMALIZE → ACCESS CHECK → ANALYZE → BUILD REFERENCE → BUILD TIMELINE → DECOMPOSE → PLAN PROMPTS → VALIDATE → OUTPUT

## Deliverables
- WORKFLOW.md
- INPUT_CONTRACT.md
- ANALYSIS_WORKFLOW.md
- SCENE_WORKFLOW.md
- GENERATION_WORKFLOW.md
- FAILURE_HANDLING.md
- HANDOFFS.md
- CHANGELOG.md
