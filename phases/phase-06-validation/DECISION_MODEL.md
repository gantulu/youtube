# Validation Decision Model

## PASS
All blocking checks pass. Warnings may remain only when they do not violate a locked rule or required contract.

## FAIL
At least one blocking error exists. Final production-ready output is prohibited.

## WARNING
A non-blocking uncertainty or quality concern is recorded without being converted into a false fact.

## Decision record
The validator should identify:
- status: PASS or FAIL;
- errors;
- warnings;
- affected scenes;
- responsible upstream stage;
- required remediation.

## Validator boundary
The validator diagnoses and routes defects. It does not silently regenerate scenes or alter locked project rules.
