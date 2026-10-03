# Production Failure Handling

## Validation not passed
Do not start production. Return to Phase 6.

## Generation failure
Retry only with the validated specification or route the defect for correction.

## Asset verification failure
Block assembly for the affected asset until corrected and reverified.

## Assembly failure
Repair assembly without silently changing the validated scene plan; revalidate if the material timing/order changes.

## Audio failure
Correct and reverify synchronization; return to Phase 6 if the validated audio plan must change.

## Final QA failure
Block export and route the defect to production or the responsible upstream phase.

## Export failure
Do not mark production complete. Retry export or correct the technical issue, then verify the resulting artifact.
