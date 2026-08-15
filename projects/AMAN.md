# AMAN / Amntak — Cybersecurity Learning & Labs Platform

**Private project — public portfolio documentation**

## Overview

AMAN is a private software project whose verified implementation combines a .NET backend with a web client for a cybersecurity-oriented learning and practice platform. The backend exposes authentication, courses, hands-on labs, profiles/dashboard, social posts, notifications, and subscription/billing capabilities.

## Product Model

The available implementation indicates a platform designed around three connected experiences:

1. **Learning** — courses, course discovery, enrollment, and progress.
2. **Hands-on security practice** — labs that can be started/stopped and can accept flag submissions.
3. **Community and progression** — profiles, posts/feed, notifications, points, experience level, rank, achievements, and subscription plans.

## Verified Backend Capabilities

- User registration and password login
- Google external authentication flow
- JWT-based authentication support
- Course listing, search/category filtering, details, enrollment and enrolled-course queries
- Lab listing, lab instances, start/stop lifecycle and flag submission
- User dashboard and profile endpoints
- Social feed and post creation
- Real-time notifications using SignalR
- Subscription plan listing and subscription workflow
- OpenAPI/Scalar API documentation support

## Architecture

The backend is structured into separate API, Application, Core, and Infrastructure projects, consistent with a layered/Clean Architecture direction.

- **API:** ASP.NET Core controllers, authentication, SignalR hub and HTTP surface
- **Application:** MediatR commands/queries, FluentValidation and mapping
- **Core:** domain layer
- **Infrastructure:** Entity Framework Core with SQL Server and Docker integration

## Verified Technology Stack

- .NET 10 / ASP.NET Core 10
- C#
- Entity Framework Core 10
- SQL Server
- MediatR
- FluentValidation
- AutoMapper
- JWT Bearer Authentication
- Google Authentication
- SignalR
- OpenAPI
- Scalar
- Docker.DotNet

## Web Client

The companion `amntak-web` repository provides the browser-facing experience and uses Next.js 16, React 19, TypeScript, TanStack React Query, tRPC, Zod, Tailwind CSS and Framer Motion.

## Product Experience Observed

The dashboard is designed around cybersecurity progression: active labs, recent courses and progress, points, experience level, rank, completed challenges, streaks and achievements.

## Security & Engineering Notes

The project demonstrates practical security engineering concerns including authentication, authorization boundaries, current-user services, protected lab actions, external identity integration and real-time authenticated notifications.

The current private implementation also contains development-stage placeholders in some flows; this portfolio description therefore distinguishes the implemented architecture from production-readiness claims.

## Source & Privacy

The canonical source remains private:

[AMAN](https://github.com/mukhtarprov1-hue/AMAN)

No source code is copied into this public portfolio repository.

## Related

- [AMNTAK Web Client](./Amntak-Web.md)
- [Mukhtar Alawady Portfolio](https://github.com/mukhtarprov1-hue/Mukhtar-Alawady)
- [GitHub Profile](https://github.com/mukhtarprov1-hue)
- [LinkedIn](https://www.linkedin.com/in/mukhtar-alawady-078697382/)
