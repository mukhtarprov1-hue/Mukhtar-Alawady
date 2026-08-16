# CoreProvenance™ — Security Intelligence & Provenance Platform

> **Private product · Public technical case study · Evidence-backed status**

## 1. Executive Summary

CoreProvenance is a security-focused web application concept designed as a command center for security telemetry, investigation, policy management, AI-assisted analysis, model lifecycle, device trust, provenance, and security APIs.

The public portfolio distinguishes the **currently verifiable web application implementation** from the broader product architecture and future security capabilities.

## 2. Verified Implementation Snapshot

The canonical repository is a Vite + React + TypeScript application. Its verified package configuration includes Vite, React 18, TypeScript 5, React Router, TanStack React Query, Vitest, Zod, Recharts, Supabase client libraries, and a broad Radix/shadcn UI component layer. The repository also contains `src/pages`, `src/components`, `src/hooks`, `src/integrations`, `src/lib`, and `src/test` directories. fileciteturn34file0 fileciteturn35file0

The application routing currently exposes concrete page surfaces for:

- Main dashboard
- Causal Explorer
- Policies
- AI Analyst
- Attestation
- Model Registry
- API Documentation
- Architecture
- Authentication

These routes are implemented in `src/App.tsx`. fileciteturn36file0

## 3. Product Concept

The intended security workflow is:

```text
Telemetry → Detection → Verdict → Investigation → Policy → Evidence → Response
```

The product architecture additionally explores device trust, attestation, model integrity, feature controls, and security provenance.

## 4. Primary Product Surfaces

### Security Dashboard

Designed for event, alert, status, and security-operation visibility.

### Causal / Forensic Explorer

Designed to support relationships between processes, files, network activity, user actions, and security events.

### Alert / Policy Workflows

Designed for security findings, severity/context filtering, policy management, and controlled changes.

### AI Analyst

Designed as an analyst-assistance surface for explaining events and producing human-readable security context.

### Attestation / Model Registry

Implemented as navigable application surfaces representing the broader trust and model-lifecycle architecture.

### Architecture / API Documentation

Dedicated product surfaces exist for architectural communication and API documentation.

## 5. Security Architecture Direction

The intended authorization hierarchy is:

```text
System
  ↓
Module
  ↓
Feature
  ↓
Permission
  ↓
Business Rules
  ↓
Database RLS
```

This is a **security architecture direction** and should not be interpreted as proof that every control is production-complete.

## 6. Security Model

The broader design considers:

- Role-based access control
- Server-side authorization
- Database Row Level Security (RLS)
- Append-oriented audit logging
- Device attestation
- Artifact/model integrity
- Evidence provenance
- Controlled feature activation

Where a capability has not been verified in the repository, it remains explicitly categorized as architecture or roadmap.

## 7. AI-Assisted Security

The AI Analyst surface exists in the current application structure. The security-analysis concept includes alert explanation, causal-chain explanation, policy assistance, and human-readable summaries.

Evaluation evidence is still required before claiming production-grade AI accuracy or reliability.

## 8. Verified Technology Direction

- React 18
- TypeScript 5
- Vite 5
- React Router
- TanStack React Query
- Vitest
- Zod
- Recharts
- Supabase client
- Radix UI / shadcn-style components
- Tailwind CSS

The package configuration is the source of truth for this technology list. fileciteturn34file0

## 9. Evidence Boundary

### Verified

- Vite/React/TypeScript application structure
- Existing source directories
- Concrete application routes/pages
- Dependency and test tooling declarations

### Architectural direction

- Full SOC telemetry pipeline
- Provenance-backed forensic workflow
- Device attestation
- Model signing/integrity lifecycle
- Production authorization enforcement
- Full audit/evidence backend

### Not claimed

- Production-ready security operations platform
- Complete backend telemetry ingestion
- Validated AI detection performance
- Independently audited security controls

## 10. Required Next Validation

The strongest next evidence should establish:

1. Build success and reproducibility.
2. Unit/component test results.
3. Route/page functional validation.
4. Authentication and authorization tests.
5. Data-isolation/RLS tests if backend controls are enabled.
6. Dependency and secret scanning.
7. Sanitized screenshots of implemented surfaces.
8. Threat model and trust-boundary diagram.

## 11. Canonical Source

[core-provenance-ai](https://github.com/mukhtarprov1-hue/core-provenance-ai)

The implementation repository remains private and is the source of truth for code.

## 12. Related Portfolio Evidence

- [CoreProvenance Evidence Pack](./CoreProvenance-EVIDENCE.md)
- [Portfolio Evidence Matrix](../EVIDENCE-MATRIX-2026.md)
- [Global Benchmark 2026](../GLOBAL-BENCHMARK-2026.md)

## 13. Responsible Security

Security operations, telemetry analysis, attestation workflows, and any potentially abusable security functionality should be used only in authorized defensive environments and controlled research settings.
