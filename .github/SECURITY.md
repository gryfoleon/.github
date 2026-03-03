# Security Policy (Internal Use Only)

## 1. Purpose
This document defines the process for reporting and handling security issues for this internal repository, including vulnerabilities, misconfigurations, and suspected secret exposure.

## 2. Scope
This policy applies to:
- Source code, configuration, CI/CD workflows, and infrastructure-as-code in this repository
- Build artifacts and dependencies produced by this repository
- Internal documentation stored in this repository

## 3. Reporting a Security Issue
**Do not** open a public issue or Pull Request for suspected security problems.

Report security issues via one of the following internal channels:
- Security email: **security@TUEMPRESA.com**
- Internal ticketing system: **(enlace a Jira/ServiceNow)** using the category **Security Incident / Vulnerability**
- Internal escalation (if urgent): **#security** (do not paste secrets)

### 3.1 Required information
Please include, as available:
- Summary and suspected impact
- Affected component(s) and environment(s) (dev/staging/prod)
- Steps to reproduce (PoC where possible)
- Affected versions/commits and configuration context
- Any immediate mitigations already applied
- Whether customer or personal data may be involved

## 4. Handling of Secrets
If secrets (tokens, passwords, private keys, certificates) may have been exposed:
- Treat the secret as **compromised**
- Coordinate **immediate revocation/rotation**
- Remove the secret from the repository and CI/CD configuration
- Follow internal guidance for history rewrite if required (only by authorized personnel)

## 5. Response Targets (Internal)
Target response times (business days) are:
- Acknowledgement: **within 1 business day**
- Initial triage: **within 2 business days**
- Remediation plan/ETA: **within 5 business days**, subject to severity and operational constraints

## 6. Disclosure
This is an internal repository. External disclosure is **not permitted** without explicit approval from Security and Legal.

## 7. Ownership
- Security contact: **security@TUEMPRESA.com**
- Repository owner team: **@TU-ORG/TEAM**