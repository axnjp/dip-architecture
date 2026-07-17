# Publication Build

Reserved for publication tooling, public-source allowlists, render configuration, and verification outputs permitted under P5.

Generated files are never authoritative over canonical Markdown and structured metadata.

P0-B27 adds controlled public and restricted ADR staging tools:

- `public-staging-policy.json` defines the explicit public projection and disclosure controls;
- `tools/build_public_staging.py` generates the public-only staging tree without reading restricted ADR bodies;
- `tools/build_restricted_adr_staging.py` assembles the complete ADR working corpus for the separately authenticated restricted repository;
- `templates/public-repository-README.md` supplies the controlled public repository front matter.

Staging outputs remain working artifacts until repository readback and evidence binding are complete. They are not Architecture v1.0 release pins.

P0-B28 adds the closed structured-register projection layer:

- `public-structured-register-projection-policy.md` defines projection classes, allowed and prohibited content, review gates, and failure behavior;
- `../schemas/public-projections/` contains the common schema, twelve register-specific schemas, the schema registry, and controlled fixtures;
- `tools/generate_public_projection_schema_fixtures.py` produces deterministic validation fixtures;
- `tools/create_public_projection_schema_integrity.py` inventories the schema set and verifies prohibited properties, local references, and closed top-level shapes.

P0-B30 promotes the explicitly approved P0-B29 candidate set into twelve canonical public structured-register projections. The public builder consumes only those installed projections and rejects any projection that is not marked approved or whose disclosure review is incomplete. It still has no fallback path that sanitizes complete canonical records.
