# Cybersecurity Portfolio Evidence Matrix — 2026

This matrix separates **verified evidence** from architecture, planned work, and future validation. It is the control document for the public portfolio.

## Status vocabulary

- ✅ **Documented** — publicly documented and supported by project material.
- 🧪 **Needs measured evidence** — capability exists or is described, but quantitative proof should be added.
- 🔒 **Private evidence** — implementation/evidence exists in a private project and is intentionally not published.
- 🗺️ **Planned** — roadmap only; must not be presented as completed.

## Priority projects

| Project | Security identity | Current evidence | Highest-value next evidence | Priority |
|---|---|---|---|---|
| CyberShield | Mobile Security / Security Engineering | Architecture, security principles, technology direction, private canonical repository | Android version matrix, permission tests, storage/security tests, screenshots, performance and reliability measurements | P0 |
| AI-Assisted Website Security Assessment | AppSec / AI Security | Assessment workflow, tooling, finding model, ML approaches, evaluation criteria | Controlled benchmark targets, finding precision/recall, FP/FN analysis, deduplication results, sample sanitized report | P0 |
| CyberVision | Network Security / Detection | Capture architecture, telemetry model, monitoring workflow, Python/Scapy/SQLite direction | PCAP benchmark, protocol parsing accuracy, CPU/RAM measurements, detection scenarios, alert precision, screenshots | P0 |
| Network Security & IDS Labs | Network Defense / Detection Engineering | Lab architecture, tooling, detection lifecycle, representative scenarios | Reproducible lab cases, alert evidence, rule tuning, MITRE ATT&CK mapping, incident timelines | P0 |
| CoreProvenance | Security Intelligence / AI | Security-intelligence architecture and feature model | Data-flow diagram, event schema, model-evaluation plan, provenance/attestation evidence, threat model | P1 |
| Yemen Cyber Security | Cybersecurity initiative / knowledge | Initiative documentation | Public outputs, research/resources index, contribution model, measurable reach | P1 |
| AMAN / Amntak | Cybersecurity education | Platform/product documentation | Lab catalog, learner workflow evidence, security architecture, auth/access-control testing | P1 |

## Evidence pack standard

Each P0 project should eventually have:

1. Executive summary
2. Scope and threat context
3. Architecture diagram
4. Trust boundaries / attack surface
5. Security requirements
6. Security controls
7. Test methodology
8. Test environment
9. Test cases
10. Results and metrics
11. Findings
12. Remediation / engineering decisions
13. Limitations
14. Reproducibility notes
15. Screenshots or sanitized evidence
16. Responsible-use statement
17. Roadmap
18. Canonical repository link

## Metrics library

Use only metrics that are actually measured.

### AppSec / AI assessment

- Precision
- Recall
- F1
- False-positive rate
- False-negative rate
- Finding deduplication rate
- Mean analysis time
- Coverage by OWASP category
- Human-validation agreement

### Network monitoring / IDS

- Packets processed/sec
- Dropped-packet rate
- CPU utilization
- Memory utilization
- Protocol parsing accuracy
- Alert precision
- Alert recall
- False-positive rate
- Detection latency
- Rule coverage

### Mobile security

- Permission coverage
- Android API-level compatibility
- Security-test pass rate
- Crash-free test rate
- Startup time
- Memory usage
- Storage protection test results
- Network-control test results

## Evidence rules

1. Never invent a metric.
2. Never call a roadmap item a feature.
3. Distinguish prototype, academic project, private product, lab, and production deployment.
4. Do not publish credentials, secrets, private datasets, or sensitive implementation details.
5. Screenshots must be sanitized.
6. Security claims should be tied to a test, design decision, source evidence, or clearly labeled hypothesis.
7. A failed test is valid evidence when the failure and remediation are documented honestly.

## Reviewer test

A senior reviewer should be able to answer from the portfolio:

- What problem was solved?
- What assets and threats were considered?
- What was actually built?
- What was tested?
- How was it measured?
- What failed?
- What was improved?
- What remains incomplete?
- Where is the canonical implementation?

If these questions cannot be answered, the case study is not yet complete.
