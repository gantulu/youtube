# Structural Validation

Check that each required scene contains the expected identifiers, timestamps, timing information, source linkage, generation-stage specification, continuity requirements, and applicable audio requirements.

## Checks
- required scene identity present;
- start/end timestamps present and ordered;
- duration is coherent with timestamps;
- generation stage is explicitly identified;
- required prompt/reference fields are present;
- no malformed or contradictory scene structure.

## Schema protection
The exact final schema remains governed by the project schema version. Do not silently introduce or remove required fields.
