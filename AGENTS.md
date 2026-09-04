# Pendago Agent Instructions

## Product Phase

Pendago is currently in System Architecture & Technical Specification phase.

Do not begin framework or implementation setup until architecture decisions
have been explicitly approved.

## Source of Truth

The locked product discovery documents under:

docs/product-discovery/

are authoritative product constraints.

Do not silently reinterpret or overwrite locked decisions.
When a technical decision changes an earlier assumption, record it explicitly
through an ADR or superseding document.

## Architecture Principles

- Backend owns authoritative classroom-session state.
- Controller, display, backend, AI engine, and validation boundaries must be contract-first.
- LLM output must conform to versioned structured schemas.
- Never render arbitrary AI-generated HTML.
- Mathematics displayed to learners must pass deterministic validation.
- Curriculum assertions must use controlled and versioned source data.
- AI-generated scenes must be atomic. Never expose partially generated scenes.
- Essential classroom interaction must degrade gracefully during connectivity loss.
- Prepared lessons should remain available locally when connectivity is degraded.
- Minimize student data collection.
- Raw classroom audio must not be persisted by default.

## Current Engineering Constraints

No implementation technology stack has been selected yet.

Do not introduce:
- frontend frameworks
- backend frameworks
- databases
- container platforms
- cloud platforms
- realtime infrastructure

without an explicit architecture decision.

## Required Decision Process

For significant technical decisions:

1. Extract requirements from locked discovery documents.
2. Identify alternatives.
3. Evaluate trade-offs.
4. Recommend one option.
5. Obtain approval.
6. Record the accepted decision as an ADR.
7. Only then implement it.