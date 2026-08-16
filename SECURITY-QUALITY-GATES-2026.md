# Security & Quality Gates — 2026

These gates define the minimum maturity expected before a project is presented as a flagship public cybersecurity project.

## Gate 1 — Identity

- Clear security purpose
- Clear project status
- Canonical repository identified
- Public/private boundary explicit

## Gate 2 — Documentation

- README is complete
- Architecture is documented
- Scope and assumptions are documented
- Security model is documented
- Limitations are explicit

## Gate 3 — Security

- Threat model or threat considerations
- Authentication/authorization review where applicable
- Secret-handling review
- Input/output validation where applicable
- Logging/auditability considerations
- Dependency/supply-chain considerations
- Responsible-use statement

## Gate 4 — Testing

- Functional tests where applicable
- Security tests
- Negative/failure tests
- Reproducible environment
- Measured results where claims depend on performance or accuracy

## Gate 5 — Engineering

- Version control discipline
- Issue/change tracking
- Dependency hygiene
- Automated validation where appropriate
- Security scanning where appropriate
- Release/version notes for meaningful public releases

## Gate 6 — Evidence

A flagship claim should point to at least one of:

- Test result
- Screenshot
- Architecture artifact
- Sanitized log
- Measurement table
- Research result
- Verified source/configuration evidence kept in the canonical repository

## Gate 7 — Publication

Before publishing:

- Remove secrets and private information.
- Sanitize personal/customer/production data.
- Review offensive-security material for safe scope.
- Mark planned features accurately.
- Ensure links resolve to canonical sources.
- Avoid unsupported superlatives such as "world's most advanced" without objective evidence.

## Maturity levels

### Level 0 — Concept

Idea or architecture only.

### Level 1 — Prototype

Working implementation with limited validation.

### Level 2 — Demonstrated

Working implementation with documented tests and evidence.

### Level 3 — Reproducible

Repeatable environment, documented measurements, testing, limitations, and release discipline.

### Level 4 — Production-oriented

Security review, operational controls, deployment/recovery considerations, observability, and sustained maintenance evidence.

The portfolio should use the highest level justified by evidence rather than the highest aspirational level.
