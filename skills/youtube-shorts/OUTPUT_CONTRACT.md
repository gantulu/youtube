# End-to-End Output Contract

## Internal
The Skill may internally maintain:
- workflow state
- evidence package
- Global Reference
- timeline and scene map
- generation package
- validation decision
- remediation state
- production record

These are execution artifacts, not automatically user-facing output.

## Final output
The final response must conform to the current project-defined output schema and locked project rules.

Default final behavior for analysis/generation requests:
- provide the structured scene blueprint;
- preserve timestamps, scene identity, continuity, and evidence grounding;
- do not output unsupported speculation;
- do not claim successful rendering/production unless verified by Phase 7.

## Failure output
If a blocking gate fails, do not emit a production-ready scene blueprint. Return the blocking condition and the required remediation path.

## Schema protection
Do not silently invent, remove, rename, or restructure project-defined output fields. Schema changes require an explicit project version update.
