

# PII Compliance & GRC Audit Lab

## 📸 Sample Evidence

![Splunk Logs](screenshots/splunk-ingestion-success.png)
![Login Page](screenshots/login-page.png)
# PII Compliance & GRC Audit Lab

## Overview
This project simulates a compliance assessment of a web application processing Personally Identifiable Information (PII). The focus is on evidence collection, control validation, audit defensibility, and remediation tracking aligned to NIST SP 800-53.

## Objectives
- Collect and validate technical evidence
- Map controls to authentication, logging, and encryption requirements
- Identify compliance gaps and assign risk
- Track remediation actions
- Align data handling to PII/CCPA concepts

## Environment
- Web App: OWASP Juice Shop (Docker)
- SIEM: Splunk Enterprise (local)
- Platform: Windows

## Controls Assessed
- IA-2: Identification and Authentication
- AU-2: Audit Events
- AU-6: Audit Review
- SC-8: Transmission Confidentiality
- AC-2: Account Management

## Evidence Collected
- Splunk log ingestion and search results
- Web application login and account behavior
- HTTP (no TLS) observation
- System password policy (net accounts)
- Architecture diagram

## Key Findings
- No TLS encryption (SC-8) → High Risk
- No MFA implemented (IA-2) → Medium Risk
- No log review process (AU-6) → Medium Risk
- Logging present and validated (AU-2) → Low Risk

## Remediation Actions
- Implement HTTPS/TLS
- Enable MFA
- Establish log monitoring procedures

## Project Structure
