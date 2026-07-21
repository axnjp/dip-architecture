# G1 — Operational Design

Status: approved normalized current source under PG0-E001; formal PG0 closure
pending

Provenance: `manual_recovered_provenance_limited`

This is a normalized current source under PG0-E001. It is not the unavailable
original conversation text.

## 1. Governed artifact lifecycle

Every authoritative platform artifact follows a governed lifecycle:

**receive → validate → accept → version → propagate → observe**

Receipt, validation, acceptance, publication, freshness, and propagation are
distinct control states. Artifact versions are immutable, and provenance and
lineage identify the exact version used by downstream reasoning or action.

Evidence: `recovered_continuity`, `normalized_current`.

## 2. Workflow and orchestration model

The durable execution hierarchy is:

**Trigger → Workflow → Stage → Job → Attempt**

The system uses at-least-once execution with idempotent jobs. Domain Events,
Orchestration Signals, Commands, and Outcomes are distinct concepts. Change
Detection and Execution Planning decide when work is required. Transactional
Outbox and Consumer Inbox patterns support reliable publication and
deduplication. Scoped event ordering is used where ordering is required.

Workflow versions are immutable while active. Shadow and limited rollout,
execution policy profiles, freshness policies, domain calendars, circuit
breakers, catch-up planning, reconciliation reports, and generation-based
rebuilds are governed capabilities.

Refresh, replay, backfill, and rebuild are distinct operations.

Evidence: `recovered_continuity`.

## 3. Workspace and Private Strategy operation

The Workspace is the operational boundary for a domain instance. Private
Strategy is private strategic context and intellectual capital governed within
that Workspace. Cross-Workspace sharing is explicit, scoped, and governed; it
does not occur through accidental context leakage. Workspace selection and MCP
write scope are explicit. Review Service authority is preserved for any
governed mutation.

Evidence: `recovered_continuity`, `normalized_current`.

## 4. Interfaces and review

ChatGPT and the minimal DIP Operations Page are peer interfaces to the Review
Service. Every governed action may be initiated from an authorized interface
while preserving the same governance and audit behavior. Conversation is a
first-class workflow trigger. The Operations Page initially provides review
inbox, refresh controls, workflow inspection, and related operational views.

Evidence: `recovered_continuity`.

## 5. Domain and repository boundaries

The repository reflects the architecture but does not define it. Schemas are
first-class reusable assets. DIP Core, Domain Packages, Workspaces, and Private
Strategy assets have distinct ownership and dependency boundaries. Domain
Packages cannot modify DIP Core. Private packages cannot become dependencies of
public packages. Curated Knowledge Assets are distinct from generated
intelligence.

Evidence: `recovered_continuity`.

## 6. Initial operational posture

The initial target is a low-cost private deployment that preserves the long-term
architecture without unnecessary enterprise infrastructure. The initial
implementation may be narrow, but it must preserve the governing boundaries,
provenance, review, and audit model.

Evidence: `recovered_continuity`.

## 7. Canonical scope decision

This packet is sufficient as the current operational source for publication and
implementation planning. It does not claim that every original G1 subsection
or historical explanatory paragraph was recovered verbatim.
