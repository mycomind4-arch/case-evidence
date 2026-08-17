# Case Evidence

**Status: Platform/infrastructure concept — not a consumer vertical.**

## Purpose

Provide reusable document, evidence, provenance, timeline, and case-analysis primitives for specialized MailMyPDF verticals.

## Core model

**Case → Documents → Extracted Facts → Evidence → Relationships → Events → Findings → Actions**

Every important derived fact should retain provenance to its source document/page where possible, with confidence and review state where applicable.

## Intended consumers

- Code Enforcement
- Tenant Reply
- Insurance Claims
- Benefits Appeal
- GovReply
- Appeal Mail
- Records Requests
- future case-oriented verticals

## Core capabilities

- document ingestion/extraction
- page-level provenance
- evidence records and relationships
- timeline/event reconstruction
- deadline primitives
- contradiction/gap detection
- human review state
- auditable findings
- export/API interfaces

## Architecture guidance

This should eventually live as shared platform infrastructure or a reusable package, not become another consumer-facing product. FairProcess and FairProcessMaps are reference implementations and sources of technology to evaluate, not systems to blindly copy wholesale.

## Non-goals

- consumer legal advice
- jurisdiction rules without authoritative sources
- opaque AI conclusions
- duplicated vertical-specific workflows
- premature microservices or agent orchestration

## Success criterion

A vertical should be able to ingest real documents and produce a source-linked, reviewable case record without rebuilding extraction, provenance, evidence, or timeline logic from scratch.
