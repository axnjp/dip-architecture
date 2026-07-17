# Public Structured-Register Projection Policy

Status: `approved model implemented as P0 working policy`  
Batch: `P0-B28`  
Classification: Public Reference Architecture

## Purpose

This policy turns the P0-B27 minimum-necessary-disclosure model into enforceable schemas for public machine-readable registers. A structurally valid document is only a candidate projection; semantic approval is still required.

## Projection classes

1. **Deterministic field projection** copies only schema-allowlisted public fields from records already classified as Public Reference Architecture.
2. **Field projection with semantic review** applies the allowlist and then requires record-by-record review because otherwise public-looking prose may carry restricted context.
3. **Authored public projection** creates a separate public-safe summary from controlled public evidence. It does not transform or redact restricted source text.

## Allowed content

Public projections may contain stable identifiers, approved public titles, normalized public statements, lifecycle status, public Blueprint destinations, public relationships, abstract gate criteria, and public scope or phase summaries.

## Prohibited content

Public projections must not contain:

- approved source quotations or approval-message text;
- source identifiers, conversation locators, evidence-package locations, verification evidence, or evidence hashes;
- restricted repository identity, location, authentication, access-control, or revision metadata;
- real Workspace or Private Strategy instance data, memberships, bindings, identifiers, or active private configuration;
- provider-specific protected topology, authority roots, configuration paths, or secret-resolution details;
- secret values, secret-shaped tokens, emails, account identifiers, attachment identifiers, or complete export material;
- inferred values reconstructed from restricted evidence.

## Release conditions

A projection can move from `draft_projection` to `approved_public_projection` only after:

1. schema validation passes;
2. prohibited-field scanning passes;
3. secret scanning passes;
4. private-instance non-disclosure review passes;
5. semantic disclosure review passes;
6. every relationship resolves only to public-safe records;
7. the public staging build reads only public projection files;
8. repository readback at an immutable working revision matches the approved projection hashes.

## Failure behavior

Validation or review failure blocks the affected projection. The build omits the register and records a publication gap; it never falls back to loading the complete canonical or restricted record and attempting redaction.
