# Production Protocol

## Preconditions
Production requires a Phase 6 validation decision with status PASS. A WARNING may proceed only when it is explicitly non-blocking and does not violate a locked rule.

## Production order
1. Load the validated generation package.
2. Execute the applicable generation stages.
3. Verify every generated asset.
4. Assemble scenes in validated timeline order.
5. Integrate approved audio requirements.
6. Run final QA against the validated scene plan.
7. Export the final artifact using the required project format.
8. Record production status and artifact references.

## Boundary
Production execution must not silently alter the validated scene plan. Any material change requires revalidation.
