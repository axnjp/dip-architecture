# Public Structured-Register Projection Schemas

Status: `active / twelve approved projections installed`  
Batch: `P0-B30`  
Classification: Public Reference Architecture

These JSON Schemas define the only permitted machine-readable shapes for structured registers entering the public publication corpus. They do not authorize a projection merely because it validates structurally.

## Governing controls

- Every projection is deny-by-default and uses a register-specific schema.
- Schemas expose normalized public statements and public-safe relationships, not source evidence.
- Record objects reject undeclared fields.
- Approval quotations, source identifiers, evidence locators, verification evidence, restricted repository metadata, Private Authority data, and secrets are not projection fields.
- Semantic review, private-instance non-disclosure review, prohibited-field scanning, and secret scanning are mandatory before public approval.
- Restricted sources are never loaded by the public build.
- Missing public evidence produces omission or a publication gap, never reconstruction from assumption.

The schema registry maps each canonical register to its schema, projection class, eligibility rule, and intended public output path. `build/public-structured-register-projection-policy.md` defines the operating policy.

P0-B30 installs all twelve approved projections after schema validation, semantic/security review, explicit approval, immutable public working-revision binding, and byte-for-byte repository readback. `PUB-GAP-0012` is closed; final Architecture v1.0 source and release pinning remains separate.
