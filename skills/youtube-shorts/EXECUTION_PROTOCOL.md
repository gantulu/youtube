# End-to-End Execution Protocol

## Lifecycle
INPUT → NORMALIZE → ACCESS → ANALYZE → REFERENCE → DECOMPOSE → GENERATE → VALIDATE → REMEDIATE IF REQUIRED → PRODUCE → FINAL OUTPUT

## Phase mapping
- Input/normalize/access: Phase 3
- Video analysis: Phase 4
- Global Reference and scene generation: Phase 5
- Validation and defect routing: Phase 6
- Production execution, QA, export, record: Phase 7

## Execution rules
1. Initialize workflow state.
2. Normalize URL or video ID.
3. Run access gate.
4. Execute Phase 4 analysis.
5. Build and verify Global Reference.
6. Decompose the complete timeline into scenes.
7. Execute Phase 5 generation planning.
8. Run Phase 6 validation.
9. If validation fails, route the defect to the responsible upstream stage, repair, and revalidate.
10. Only after validation PASS, execute Phase 7.
11. Verify production assets, assembly, audio, final QA, and export according to Phase 7.
12. Emit the final output only when its output contract is satisfied.

## No-skip rule
A phase may be considered complete only when its required gate is PASS. A warning may continue only when explicitly non-blocking and compliant with locked project rules.

## Remediation loop
VALIDATION FAIL → IDENTIFY DEFECT → ROUTE UPSTREAM → REPAIR → REVALIDATE

Production defects follow Phase 7 failure handling. Material changes to the validated plan require Phase 6 revalidation.
