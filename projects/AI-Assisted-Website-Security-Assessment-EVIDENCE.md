# AI-Assisted Website Security Assessment — Evidence Pack

> Application Security · AI-assisted Security Analysis · Authorized Assessment

## 1. Purpose

This case study documents a security-assessment workflow that combines conventional web/API security testing, finding normalization, risk classification, and machine-learning-assisted analysis.

## 2. Current evidence

| Area | Status | Next evidence |
|---|---|---|
| Assessment workflow | ✅ Documented | Reproducible test run |
| Toolchain | ✅ Documented | Version-pinned tool inventory |
| Finding model | ✅ Documented | Sanitized sample findings |
| ML approaches | ✅ Documented | Evaluation results |
| Benchmark accuracy | 🧪 Needs measured evidence | Precision / recall / F1 |
| False positives/negatives | 🧪 Needs measured evidence | Confusion matrix |
| Production deployment | 🗺️ Planned | Do not claim as production |

## 3. Threat and assessment scope

Authorized targets may include owned or laboratory web applications and APIs.

Assessment areas:

- Asset discovery
- Endpoint enumeration
- HTTP/HTTPS behavior
- Authentication
- Authorization
- Input validation
- API security
- OWASP-oriented vulnerabilities
- Evidence collection
- Risk prioritization

## 4. Processing pipeline

```text
Authorized Target
      ↓
Discovery / Enumeration
      ↓
Security Testing
      ↓
Raw Findings
      ↓
Normalization / Deduplication
      ↓
Validation
      ↓
AI / ML Analysis
      ↓
Risk Prioritization
      ↓
Human Review
      ↓
Remediation Report
```

## 5. Security controls

- Authorized testing only
- Separation of discovery, testing, validation, and reporting
- Human validation before high-impact conclusions
- Sanitized evidence
- No credential disclosure
- Risk-based prioritization
- Reproducible finding records

## 6. ML evaluation plan

For a controlled labeled dataset, evaluate:

- Precision
- Recall
- F1 score
- False-positive rate
- False-negative rate
- Confusion matrix
- Per-category performance
- Finding deduplication accuracy
- Analysis latency

## 7. Finding schema

Each normalized finding should contain:

| Field | Required purpose |
|---|---|
| Asset | Affected system/endpoint |
| Finding | Security issue |
| Evidence | Supporting observation |
| Severity | Risk level |
| Confidence | Confidence score |
| CWE/OWASP | Weakness/category mapping |
| Impact | Technical/business impact |
| Remediation | Corrective action |
| Validation | Verification method |

## 8. Evidence to publish

Once available, publish only sanitized material:

- Sample assessment report
- Sanitized request/response evidence
- Finding examples
- Model evaluation table
- Confusion matrix
- Architecture diagram
- Benchmark methodology
- Reproducibility notes

## 9. Limitations

Automation and ML do not replace expert validation. Scanner output can contain false positives and false negatives, while models can inherit dataset bias and miss novel weaknesses.

## 10. Canonical documentation

See the main [AI-Assisted Website Security Assessment](./AI-Assisted-Website-Security-Assessment.md) case study and [Evidence Matrix](../EVIDENCE-MATRIX-2026.md).

## 11. Responsible use

Testing must be limited to systems owned by the tester or where explicit authorization has been granted.
