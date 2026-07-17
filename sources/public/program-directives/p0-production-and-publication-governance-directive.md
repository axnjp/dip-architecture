# P0 Production and Publication Governance Directive

Source identifier: `DIP-SRC-0001`  
Source kind: `program_directive`  
Classification: `Public Reference Architecture`  
Approval state: `explicit`  
Lifecycle status: `approved_locked_controlled`  
Captured on: `2026-07-15`

## Control note

This controlled source preserves the exact approved statements from the P0 production handoff that govern publication production, classification, provenance, scope, and authorization. Attachment notices and unrelated first-domain data files are excluded because they are not part of this publication-governance directive.

## Program status

The following are complete, approved, and locked:

- G0 — Conceptual Architecture
- G1 — Operational Design
- First-Domain Viability & Implementation Readiness Review
- AI Operating Profile v1.0
- DIP AI Constitution
- Governed Companion Intelligence Operating System framing
- Implementation Planning Sections 1–12
- ADR-IMP-001 through ADR-IMP-029
- Architecture Publication Planning P0–P6

Do not reopen approved architecture, implementation, or publication decisions unless production reveals a genuine contradiction requiring formal escalation.

The governing rule remains:

> Reduce the initial implementation surface, not the governing architecture.

## Publication status

Architecture Publication planning is complete:

- P0 — Source Inventory and Normalization
- P1 — Architectural Foundations
- P2 — Living Architecture Blueprint
- P3 — ADR and Decision Register
- P4 — Architecture v1.0 and Architect’s Letter
- P5 — Editable Sources, Word/PDF, Rendering, QA, and Archives
- P6 — Implementation Kickoff Package

Publication gates PG0 through PG6 have been defined but have not yet passed. They pass only after their respective artifacts are produced, verified, and approved.

IKG0 — Implementation Authorized has not been granted.

Do not begin DIP product implementation coding. Documentation sources and publication tooling are permitted, but application/runtime implementation is not.

## Approved publication model

The publication system will use:

- canonical Markdown and structured metadata;
- stable identifiers;
- generated DOCX and PDF editions;
- modular documents plus a compiled edition;
- machine-readable manifests and registers;
- page-by-page visual verification;
- checksummed offline ZIP archives;
- exact source-revision and release pinning.

The security classifications are:

1. Public Reference Architecture
2. Restricted Architecture
3. Private Authority
4. Secrets

Public documentation may describe Private Strategy as an abstract platform capability, but it must not reveal whether any real Private Strategy instance exists.

Restricted architectural sources must reside in a separately authenticated location outside the public repository.

Private Authority owns actual Workspace and Private Strategy instances, memberships, bindings, identifiers, and active private configuration.

Secret values must never appear in documentation, repositories, prompts, logs, fixtures, generated files, or archives.

The public build must use an explicit allowlist of public sources rather than loading restricted material and attempting to redact it.

## P0 production authorization

Begin actual publication production with:

P0 — Publication Inventory and Normalization

Do not repeat the already approved P0 planning exercise. Begin producing the canonical artifacts.

Create:

1. Source Catalog
2. Decision Register Seed
3. Requirement Register
4. Principle and Invariant Register
5. Complete ADR Inventory
6. Gate and Research-Spike Register
7. Terminology and Alias Register
8. Scope and Deferral Matrix
9. Gap and Contradiction Log
10. Initial Traceability Map

Use these record families:

- DIP-REQ-####
- DIP-PRN-####
- DIP-INV-####
- DIP-DEC-####
- existing ADR identifiers
- DIP-GATE-####
- DIP-SPIKE-####
- DIP-DEF-####
- DIP-TERM-####
- PUB-GAP-####
- PUB-CON-####

Preserve all existing identifiers, including ADR-IMP-001 through ADR-IMP-029. Preserve identifier gaps. Do not renumber records or retroactively convert every approved decision into an ADR.

For each normalized record, retain:

- approved source statement;
- normalized publication statement;
- approval evidence;
- authority and scope;
- lifecycle status;
- public or restricted classification;
- intended Blueprint destination;
- related decisions, requirements, gates, and verification evidence.

Use prior DIP project conversations and approved handoffs as the evidence corpus.

Do not reconstruct missing decisions from assumption. Record incomplete evidence as a publication gap. Record genuine incompatibilities separately as potential contradictions.

## First production batch authorization

Start with the first controlled P0 production batch:

1. Create the canonical publication-source directory scaffold.
2. Create the publication manifest skeleton.
3. Create the source-catalog schema and initial catalog.
4. Create the terminology and alias register.
5. Inventory all completed DIP phases and approved source families.
6. Inventory the known ADR corpus, beginning with ADR-IMP-001 through ADR-IMP-029.
7. Establish the gap and contradiction logs.
8. Produce an initial traceability map showing how source families feed Foundations, Blueprint modules, ADRs, registers, and the Kickoff Package.

Save the canonical editable artifacts as durable publication working files.

Clearly distinguish:

- what has been created;
- what has been populated;
- what remains to be extracted;
- what evidence is missing;
- whether any blocking contradiction has been found.

Do not declare PG0 passed until the complete source corpus and required inventories satisfy the approved PG0 criteria.
