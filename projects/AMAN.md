# AMAN / Amntak — Cybersecurity Learning & Labs Platform

> **Private product · Public technical case study**

## 1. Product Summary

AMAN / Amntak is a cybersecurity learning and hands-on practice platform built around three connected experiences: structured learning, interactive security laboratories, and community/progression features.

The verified implementation combines a .NET backend with a companion Next.js web client. The public portfolio documents the product and architecture while the source remains private.

## 2. Product Problem

Traditional learning platforms can separate theory from practical security work. AMAN / Amntak is designed to connect:

**Course → Practice Lab → Submission → Progress → Community → Skill Progression**

The product model therefore treats practical security training as an integrated application experience rather than a collection of static lessons.

## 3. Core User Journeys

### Learner

1. Create an account or authenticate externally.
2. Discover and filter courses.
3. Enroll in a course.
4. Track course progress.
5. Browse available security labs.
6. Start a lab instance.
7. Perform the authorized exercise.
8. Submit the challenge flag.
9. Accumulate points, experience and progression signals.
10. Review achievements, rank and activity.

### Community User

- Maintain a profile.
- Publish posts.
- Consume a feed.
- Receive targeted notifications.
- Participate in platform progression.

### Platform Operator

- Manage learning content and labs.
- Manage subscription plans.
- Operate authenticated platform services.
- Observe platform and user progression signals.

## 4. Verified Backend Capabilities

- Registration and password login
- Google external authentication flow
- JWT bearer authentication support
- Course listing and search/category filtering
- Course details and enrollment
- Enrolled-course queries
- Lab listing
- Lab instance start/stop lifecycle
- Flag submission
- User profile and dashboard endpoints
- Social post creation and feed retrieval
- Authenticated real-time notifications via SignalR
- Subscription plan listing and subscription workflow
- OpenAPI and Scalar API documentation

## 5. Architecture

The backend is organized into four major layers:

```text
API
  ↓
Application
  ↓
Core
  ↓
Infrastructure
```

### API

ASP.NET Core HTTP endpoints, authentication surface and SignalR hub.

### Application

MediatR-based commands and queries, validation, mapping and application-level workflows.

### Core

Domain-oriented layer containing core application abstractions and business concepts.

### Infrastructure

Entity Framework Core, SQL Server and infrastructure integrations, including Docker integration.

## 6. Security Architecture

Security-relevant design elements verified in the implementation include:

- JWT bearer authentication
- External identity integration through Google
- Protected current-user operations
- Authorization boundaries for lab actions
- Authenticated real-time notification channel
- Layer separation between API, application, domain and infrastructure concerns

### Engineering Caveat

The private implementation contains development-stage placeholders in some flows. This portfolio therefore distinguishes the **implemented architectural direction** from a claim of production readiness.

## 7. Technology Stack

| Layer | Technology |
|---|---|
| Backend | .NET 10 / ASP.NET Core 10 |
| Language | C# |
| ORM | Entity Framework Core 10 |
| Database | SQL Server |
| Application Pattern | MediatR |
| Validation | FluentValidation |
| Mapping | AutoMapper |
| Authentication | JWT Bearer + Google Authentication |
| Realtime | SignalR |
| API Docs | OpenAPI + Scalar |
| Infrastructure | Docker.DotNet |
| Web Client | Next.js 16 + React 19 + TypeScript |
| Web Data | TanStack React Query + tRPC |
| Validation | Zod |
| UI | Tailwind CSS + Framer Motion |

## 8. Product Experience

The verified dashboard model includes:

- Active labs
- Recent courses and progress
- Points
- Experience level
- Rank
- Completed challenges
- Streaks
- Achievement indicators

This gives the platform a **learning + practice + progression** product loop.

## 9. Security Training Model

The lab lifecycle is particularly relevant to cybersecurity training:

```text
Lab Catalog
   ↓
Start Lab
   ↓
Lab Instance
   ↓
Practical Exercise
   ↓
Flag Submission
   ↓
Validation
   ↓
Progress / Score
```

The design naturally supports isolated, authorized practical security exercises without exposing offensive project source code in the portfolio.

## 10. Engineering Strengths

- Clear separation of backend concerns
- Typed application workflows
- Dedicated security-oriented lab lifecycle
- Authentication and protected-user operations
- Real-time platform notifications
- Structured course and progression model
- Web/backend separation
- API documentation support

## 11. Known Development Considerations

The private repository shows some MVP-stage placeholders and hard-coded development values in individual flows. These should be addressed before any production deployment, especially around authenticated identity propagation, token handling, external login callbacks and billing identity association.

This observation is documented as an engineering limitation, not exposed source code.

## 12. Portfolio Evidence

The public portfolio records only verified product behavior and architecture. Source files, credentials, internal datasets and implementation artifacts remain in the canonical private repository.

## 13. Source

**Canonical repository:** [AMAN](https://github.com/mukhtarprov1-hue/AMAN)

**Companion web client:** [amntak-web](https://github.com/mukhtarprov1-hue/amntak-web)

## 14. Privacy & Source Policy

No source code from the private repositories is copied into this public case study. The original repositories remain the source of truth.

## 15. Responsible Security

Security laboratories and offensive-security exercises must be operated only in systems and environments where the required authorization exists.
