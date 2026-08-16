# Network Security & IDS Labs — Evidence Pack

> Network Defense · Detection Engineering · Authorized Security Labs

## 1. Purpose

This lab track demonstrates practical network-security engineering through isolated and authorized environments covering traffic analysis, segmentation, IDS/IPS, monitoring, detection, and incident-oriented investigation.

## 2. Current evidence

| Area | Status | Next evidence |
|---|---|---|
| Lab architecture | ✅ Documented | Topology diagrams per scenario |
| Network engineering | ✅ Documented | Config snapshots + validation outputs |
| Packet analysis | ✅ Documented | Annotated PCAP cases |
| IDS/IPS concepts | ✅ Documented | Rule and alert evidence |
| Detection engineering | 🧪 Needs measured evidence | Detection matrix + tuning results |
| Incident investigation | 🧪 Needs case evidence | Timeline + findings + response |
| MITRE ATT&CK mapping | 🗺️ Planned | Mapping table per detection |

## 3. Lab architecture

```text
Test Hosts / VMs / Simulators
          ↓
     Network Traffic
          ↓
       Wireshark
          ↓
  Suricata / Snort / Zeek
          ↓
      Alerts / Events
          ↓
       Triage & Analysis
          ↓
 Investigation / Containment / Report
```

## 4. Core scenarios

### Scenario A — Segmentation

Build VLANs, routing boundaries and ACLs. Verify expected connectivity and blocked paths.

### Scenario B — Packet analysis

Capture authorized traffic and document DNS, TCP, HTTP and anomalous behavior.

### Scenario C — IDS detection

Generate controlled test traffic, inspect alerts, tune rules, and verify detection behavior.

### Scenario D — VPN security

Validate protected connectivity, routing, access boundaries and traffic visibility.

### Scenario E — Incident investigation

Start from an alert or PCAP, reconstruct the relevant event sequence, identify affected assets and document the response path.

## 5. Detection lifecycle

```text
Telemetry
   ↓
Normalization
   ↓
Detection
   ↓
Alert
   ↓
Triage
   ↓
Enrichment
   ↓
Investigation
   ↓
Response
   ↓
Lessons Learned
```

## 6. Evidence model

Each lab scenario should capture:

- Objective
- Topology
- Assets
- Threat/scenario
- Tool versions
- Configuration summary
- Expected behavior
- Observed behavior
- Alert/evidence artifacts
- Result
- Limitations
- Remediation or tuning

## 7. Detection metrics

Where measurement is possible:

- Detection coverage
- Alert precision
- Alert recall
- False-positive rate
- Detection latency
- Rule-tuning improvement
- Packet-analysis accuracy
- Reproducibility across runs

## 8. MITRE ATT&CK integration

Future mature lab documentation should map each relevant detection or adversary behavior to an ATT&CK technique and explain:

- Why the mapping applies
- What telemetry supports it
- What the detection sees
- What the detection misses
- How validation was performed

## 9. Publishable evidence

Use sanitized public artifacts:

- Network topology diagrams
- Annotated PCAP snippets
- IDS alert screenshots
- Detection rule excerpts where safe
- Test-result tables
- Incident timelines
- ATT&CK mapping tables

## 10. Responsible use

All experiments, scans, attack simulations and detection tests must remain inside isolated laboratories or systems for which explicit authorization has been granted.

## 11. Canonical documentation

See [Network Security & IDS Labs](./Network-Security-IDS-Labs.md) and the [Evidence Matrix](../EVIDENCE-MATRIX-2026.md).
