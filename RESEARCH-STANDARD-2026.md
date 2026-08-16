# Cybersecurity Research & Experiment Standard — 2026

## Purpose

A reproducible standard for technical studies, security experiments, labs, and research notes published through this portfolio.

## Required structure

1. **Question** — What security question is being investigated?
2. **Hypothesis** — What result is expected and why?
3. **Scope** — Assets, environment, assumptions, exclusions.
4. **Threat model** — Attacker capabilities, trust boundaries, relevant assets.
5. **Method** — Exact experimental procedure at an appropriate level of detail.
6. **Environment** — OS, versions, hardware/VM, network topology, tool versions.
7. **Dataset / Inputs** — Source, size, preparation, labeling, limitations.
8. **Variables** — Independent, dependent, controlled variables.
9. **Measurements** — Metrics and collection method.
10. **Results** — Observed outcomes, including failures.
11. **Analysis** — Interpretation and uncertainty.
12. **Limitations** — What the experiment cannot establish.
13. **Reproducibility** — What another researcher needs to repeat it.
14. **Security / Ethics** — Authorization and responsible-use boundaries.
15. **References** — Standards, papers, documentation, advisories.
16. **Next experiment** — The most valuable follow-up.

## Evidence grading

- **A — Direct evidence:** measured result, test artifact, or verified implementation.
- **B — Strong evidence:** repeated controlled observation or validated architecture evidence.
- **C — Supporting evidence:** documented design or limited experiment.
- **D — Hypothesis:** proposed or unvalidated claim.

Never present grade D as a measured finding.

## Metrics guidance

Prefer metrics that answer the security question. Examples:

### Detection
- Precision
- Recall
- F1
- False-positive rate
- False-negative rate
- Detection latency
- Coverage

### Network systems
- Packets/sec
- Packet loss
- CPU usage
- Memory usage
- Parse accuracy
- Throughput

### Application security
- Findings by category
- Validation rate
- Deduplication rate
- Time to triage
- Remediation verification rate

### Mobile
- API-level compatibility
- Permission-test pass rate
- Crash-free rate
- Memory usage
- Startup time
- Security-control pass rate

### AI security
- Attack success rate
- Defense success rate
- Refusal/acceptance error rate
- False-positive rate
- Evaluation coverage
- Robustness across prompts/inputs
- Human-review agreement

## Publication rules

- Do not fabricate results, benchmarks, CVEs, affiliations, or publications.
- Clearly label prototype, academic, private, lab, experimental, and production status.
- Sanitize screenshots and logs.
- Never commit secrets or private data.
- Avoid publishing operational details that would enable misuse outside an authorized lab.
- Keep source-code ownership and canonical repositories explicit.

## Reviewer checklist

A reviewer should be able to determine what was asked, what was tested, what was observed, how it was measured, what failed, what remains uncertain, and how the result can be reproduced.
