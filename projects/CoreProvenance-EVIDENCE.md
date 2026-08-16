# CoreProvenance — Evidence Pack

> Security Intelligence · Provenance · AI-Assisted Analysis · Private Product

## 1. Verified repository evidence

The canonical private repository is currently a Vite/React/TypeScript application. Its package manifest declares Vite, React, TypeScript, React Router, TanStack React Query, Vitest, Zod, Recharts, Supabase client libraries, and UI dependencies. fileciteturn34file0

The `src` tree currently contains application, component, hook, integration, library, page, and test areas. fileciteturn35file0

`src/App.tsx` currently wires concrete application routes for the dashboard, Causal Explorer, Policies, AI Analyst, Attestation, Model Registry, API Docs, Architecture, Authentication, and a not-found route. fileciteturn36file0

## 2. Evidence status

| Area | Status | Evidence |
|---|---|---|
| React/Vite/TypeScript application | ✅ Verified | Repository package manifest and source tree |
| Application routing | ✅ Verified | `src/App.tsx` |
| Security-oriented product surfaces | ✅ Verified as application routes | Causal Explorer, Policies, AI Analyst, Attestation, Model Registry, API Docs, Architecture |
| Automated test tooling | ✅ Declared | Vitest in package scripts/dependencies |
| Full security backend | 🧪 Needs verification | Backend/data-path evidence |
| Authorization/RLS enforcement | 🧪 Needs verification | Security tests and backend evidence |
| AI quality/performance | 🧪 Needs measurement | Evaluation dataset + metrics |
| Device attestation | 🗺️ Architecture/product direction | Integration proof required |
| Model integrity lifecycle | 🗺️ Architecture/product direction | Verification/revocation tests required |
| Production readiness | 🛑 Not claimed | Security review and deployment evidence required |

## 3. Security architecture

```text
Security Events / Data
          ↓
       Analysis
          ↓
    Verdict / Alert
          ↓
 Investigation
          ↓
 Policy / Response
          ↓
 Evidence / Audit
```

Trust controls under evaluation include RBAC, server-side authorization, RLS, auditability, provenance, attestation, and model integrity.

## 4. Threat model focus

Representative assets:

- Security events
- Alerts and verdicts
- Investigation evidence
- Policies
- Model artifacts
- Device trust information
- Authorization metadata
- Audit records

Representative threats:

- Unauthorized access
- Privilege escalation
- Data-isolation failure
- Evidence tampering
- Malicious model/artifact modification
- Policy manipulation
- False or misleading AI-assisted conclusions

## 5. Validation plan

The next validation cycle should cover:

1. `npm run build` reproducibility.
2. `npm test` / Vitest results.
3. Route-level functional tests.
4. Authentication tests.
5. Authorization tests.
6. RLS/data-isolation tests where applicable.
7. Dependency and secret scanning.
8. Error and failure-path testing.
9. Sanitized UI screenshots.
10. Threat-model verification.

## 6. AI-security evaluation

Do not publish accuracy claims until measured. Recommended metrics:

- Analyst agreement
- Explanation correctness
- Hallucination/error rate
- Confidence calibration
- False-positive/false-negative behavior
- Response latency
- Evaluation coverage
- Human-review override rate

## 7. Public evidence

Suitable evidence can include:

- Architecture diagrams
- Route map
- Sanitized screenshots
- Test summaries
- Build/test logs without secrets
- Security-test tables
- Threat model
- Evaluation methodology and results

## 8. Canonical sources

- [CoreProvenance case study](./Core-Provenance-AI.md)
- [Evidence Matrix](../EVIDENCE-MATRIX-2026.md)
- [Global Benchmark 2026](../GLOBAL-BENCHMARK-2026.md)
- [Private canonical repository](https://github.com/mukhtarprov1-hue/core-provenance-ai)

## 9. Responsible security

Security operations and security APIs must be restricted to authorized defensive environments and controlled research settings.
