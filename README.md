# Compliance Automation Toolkit (STIG + Nessus Workflow)

![Compliance](https://img.shields.io/badge/focus-Compliance%20Automation-blue)
![Security](https://img.shields.io/badge/controls-STIG%20%2F%20Vuln%20Remediation-success)
![Docs](https://img.shields.io/badge/deliverable-Runbooks%20%26%20Evidence-informational)

A toolkit-style repo demonstrating how to run compliance like an engineer:
- Execute vulnerability scanning workflows (Nessus/Tenable style)
- Track findings and remediation status
- Validate configuration hardening (STIG-aligned approach)
- Generate evidence artifacts and audit-ready documentation
- Automate recurring checks with scripts and checklists

This is designed to show real-world readiness for regulated environments and security engineering roles.

---

## Table of Contents
- [What You’ll Build](#what-youll-build)
- [Scope & Assumptions](#scope--assumptions)
- [Repo Structure](#repo-structure)
- [Workflow Overview](#workflow-overview)
- [Step 1 — Build the Findings Register](#step-1--build-the-findings-register)
- [Step 2 — Remediation Workflow](#step-2--remediation-workflow)
- [Step 3 — Validation Scripts](#step-3--validation-scripts)
- [Step 4 — Evidence Pack Generation](#step-4--evidence-pack-generation)
- [Step 5 — Recurring Operations](#step-5--recurring-operations)
- [Examples](#examples)
- [Hiring Manager Notes](#hiring-manager-notes)
- [Resources](#resources)
- [License](#license)

---

## What You’ll Build
- Findings register (CSV/Markdown) with status workflow
- Remediation runbooks (Windows + Linux)
- Validation scripts (PowerShell/Bash/Python)
- Evidence pack template (audit-ready)
- Recurring schedule checklist (weekly/monthly)

---

## Scope & Assumptions
This repo is vendor-neutral, but aligns with common environments:
- Windows endpoints and servers
- Linux servers (Ubuntu/Alpine-style)
- Nessus/Tenable-like scanning outputs
- DISA STIG hardening mindset (control-driven remediation)

---

## Repo Structure
Compliance-Automation-Toolkit/
README.md
docs/
workflow.md
evidence-pack-template.md
remediation-runbooks/
windows-remediation.md
linux-remediation.md
control-mapping/
stig-to-finding-mapping.md
scripts/
validate_windows.ps1
validate_linux.sh
parse_scan_report.py
generate_evidence_pack.py
templates/
findings_register.csv
findings_register.md
change_log.md
examples/
sample_scan_report.json
sample_evidence_pack/
