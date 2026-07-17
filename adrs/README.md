# Architecture Decision Records

Canonical ADR working destination for P0 normalization and later P3 publication. Existing identifiers are preserved; missing evidence is logged rather than reconstructed.

Status: all 29 implementation ADR titles and normalized bodies are complete. `PG3` has not passed because publication production and approved PG3 verification criteria remain pending.

P0-B27 establishes a two-tier publication model. The public repository carries abstract public ADR projections; the separately authenticated restricted repository carries the complete normalized bodies. Both forms preserve the same identifier and accepted decision. The public build does not load restricted bodies, and neither repository may contain Private Authority instance data or secrets.
