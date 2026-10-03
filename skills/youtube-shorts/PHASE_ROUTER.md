# Phase Router

## Routing table

| Condition | Route |
|---|---|
| Knowledge/product fact required | /knowledge + current official documentation |
| Skill behavior required | phases/phase-02-skill |
| Input normalization/access | phases/phase-03-workflow |
| Video evidence, temporal, visual, audio analysis | phases/phase-04-video-analysis |
| Scene specification, anchor, I2I, I2V, extension | phases/phase-05-scene-generation |
| Structural/evidence/timeline/continuity/prompt/audio validation | phases/phase-06-validation |
| Generation execution, asset verification, assembly, audio, QA, export | phases/phase-07-production |

## Failure routing
- Input failure → Phase 3
- Video unavailable or incomplete evidence → Phase 4
- Global Reference or continuity-generation defect → Phase 5
- Validation defect → Phase 6, then responsible upstream phase
- Production execution/asset/assembly/audio/QA/export defect → Phase 7
- Material change to validated scene plan → Phase 6 revalidation before production continues

## Routing principle
Route the defect, not the whole workflow, when safe. Never bypass the failing contract.
