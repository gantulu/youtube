# End-to-End Handoff Contract

## Canonical flow

Phase 3 → Phase 4
Input: normalized video identifier and access result.
Output: video evidence package.

Phase 4 → Phase 5
Input: complete evidence/timeline, temporal verification, evidence classification, persistent references, start/end states.
Output: generation-ready scene specification and Global Reference.

Phase 5 → Phase 6
Input: scene map, anchor/reference decisions, image/I2I/I2V/extension prompts, continuity and audio requirements.
Output: generation package for validation.

Phase 6 → Phase 7
Input: validation decision PASS and validated generation package.
Output: production-ready package.

Phase 7 → Final Output
Input: verified assets, assembly, audio, final QA, export, production record.
Output: final artifact references and project-defined final response.

## Contract rule
The receiving phase must never guess missing required state. Missing state is a failure or unresolved uncertainty and must be routed according to PHASE_ROUTER.md.
