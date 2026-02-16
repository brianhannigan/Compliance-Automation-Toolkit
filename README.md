# Compliance Automation Toolkit (STIG + Nessus Workflow)

![Compliance](https://img.shields.io/badge/focus-Compliance%20Automation-blue)
![Security](https://img.shields.io/badge/controls-STIG%20%2F%20Vuln%20Remediation-success)
![Docs](https://img.shields.io/badge/deliverable-Runbooks%20%26%20Evidence-informational)

STIG Alignment • Vulnerability Workflow • Evidence Generation

This repository demonstrates structured compliance operations including:

- Vulnerability tracking
- Remediation workflow
- Validation scripting
- Audit-ready evidence generation
- Recurring compliance operations

Designed to reflect regulated and government environments.

---

## Table of Contents

- Overview
- Workflow
- Repository Structure
- Step 1 – Findings Register
- Step 2 – Remediation Runbooks
- Step 3 – Validation Scripts
- Step 4 – Evidence Pack Generation
- Step 5 – Recurring Operations
- Deliverables
- Resources
- License

---

## Overview

Compliance should be:

- Measurable
- Repeatable
- Automated
- Documented

This toolkit demonstrates a structured remediation lifecycle.

---

## Workflow

Scan → Findings Register → Remediate → Validate → Evidence Pack → Audit

---

## Repository Structure

```
Compliance-Automation-Toolkit/
│
├── templates/
│   ├── findings_register.csv
│   └── change_log.md
│
├── docs/
│   ├── remediation-runbooks/
│   ├── evidence-pack-template.md
│   └── workflow.md
│
├── scripts/
│   ├── validate_windows.ps1
│   ├── validate_linux.sh
│   ├── parse_scan_report.py
│   └── generate_evidence_pack.py
│
└── examples/
```

---

## Step 1 – Findings Register

Track:

- Finding ID
- Asset
- Severity
- Control Reference
- Description
- Recommendation
- Owner
- Status
- Evidence Link
- Dates

Use template:

```
templates/findings_register.csv
```

---

## Step 2 – Remediation Runbooks

Create documented procedures for:

Windows:
- Service configuration
- Audit policy settings
- Security configuration checks

Linux:
- SSH hardening
- Permissions validation
- Logging configuration
- Package management

Store in:

```
docs/remediation-runbooks/
```

---

## Step 3 – Validation Scripts

Examples:

Linux:

```bash
bash scripts/validate_linux.sh --mode check
```

Windows:

```powershell
powershell -ExecutionPolicy Bypass -File scripts\validate_windows.ps1 -Mode Check
```

Scripts should:

- Validate configuration
- Output report
- Avoid destructive changes by default

---

## Step 4 – Evidence Pack Generation

Generate evidence:

```bash
python scripts/generate_evidence_pack.py --case COMPLIANCE-001 --out outputs/COMPLIANCE-001/
```

Evidence includes:

- Validation reports
- Findings register
- Change log
- Summary report

---

## Step 5 – Recurring Operations

Establish:

Weekly:
- Scan review
- New findings triage

Monthly:
- Retention validation
- Access audit

Quarterly:
- Control mapping review
- Compliance sampling

---

## Deliverables

- Findings register template
- Remediation runbooks
- Validation scripts
- Evidence automation
- Compliance lifecycle documentation

---

## Resources

- DISA STIG Framework Concepts
- Vulnerability Management Lifecycle Guidance
- NIST Hardening & Logging References

---

## License

MIT
