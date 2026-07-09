# Security Policy

> [!NOTE]
> If you believe you've found a security vulnerability in BugThrive, please report it privately — **not** through public GitHub issues, discussions, or pull requests.

---

## Table of Contents

- [Supported Versions](#supported-versions)
- [Scope](#scope)
- [Reporting a Vulnerability](#reporting-a-vulnerability)
- [Response Timelines](#response-timelines)
- [Research Guidelines](#research-guidelines)
- [Prohibited Activities](#prohibited-activities)
- [Sensitive Data Handling](#sensitive-data-handling)
- [Automated Testing](#automated-testing)
- [Safe Harbor](#safe-harbor)
- [Coordinated Disclosure](#coordinated-disclosure)
- [Recognition](#recognition)
- [Contact](#contact)

---

## Supported Versions

BugThrive is a continuously delivered platform. Security testing is supported only against the current production version.

| Version | Supported |
|---|---|
| Production (latest) | ✅ |
| Deprecated / unofficial / unauthorized | ❌ |

---

## Scope

### In Scope

| Asset | Notes |
|---|---|
| BugThrive production web applications | Officially deployed only |
| `*.bugthrive.com` | Actively operated subdomains |
| Official BugThrive APIs | — |
| Public GitHub repositories | Officially owned or maintained by BugThrive |

An asset is **in scope only** when it is officially deployed, actively operated, and controlled by BugThrive.
If you are uncertain whether an asset qualifies, contact us before testing.

### Out of Scope

- Unofficial, deprecated, unsupported, or unauthorized deployments
- Domains, subdomains, or services not owned or controlled by BugThrive
- Subdomains or services displaying a "Coming Soon" notice
- Third-party applications, integrations, vendors, or platforms
- Customer-owned systems or environments

> The presence of a third-party service on a BugThrive domain does not make it eligible for testing. Researchers are responsible for complying with third-party policies independently.

---

## Reporting a Vulnerability

### Preferred: GitHub Private Vulnerability Reporting

1. Navigate to the **Security** tab of the relevant BugThrive repository
2. Click **Report a vulnerability**
3. Complete and submit the private vulnerability report

This is the recommended channel — it enables faster triage, coordination, and action.

### Alternative: Email

Send reports to **compliance@bugthrive.com** with the subject: Security Vulnerability Report — [Vulnerability Title]

### What to Include

| Field | Status |
|---|---|
| Vulnerability title | Required |
| Short description | Required |
| Affected asset (domain, endpoint, repo, API) | Required |
| Clear steps to reproduce | Required |
| Potential security impact | Required |
| Researcher's full name and email | Required |
| Proof of concept | Recommended |
| Screenshots or video | If applicable |
| Suggested remediation | Optional |

Reports that do not include enough detail to reproduce or assess the issue may require follow-up or may be closed.

---

## Response Timelines

| Stage | Target |
|---|---|
| Acknowledgement and first response | Within 2 business days |
| Initial assessment | Within 4 business days |
| Progress updates (accepted reports) | Every 2 business days |
| Target final resolution | Within 7 business days |

> Business days exclude weekends and public holidays in India.

Critical and high-severity reports may receive accelerated review and prioritization.

Final resolution may include: remediation, mitigation, accepted risk, informational classification, duplicate classification, out-of-scope or intended-behavior determination, or closure.

---

## Research Guidelines

Security research is considered **good faith** when the researcher:

- Tests only authorized, in-scope BugThrive assets
- Uses the minimum level of access necessary to demonstrate the vulnerability
- Avoids accessing, modifying, or retaining other users' data
- Stops testing immediately upon encountering sensitive data
- Reports findings promptly and privately
- Provides accurate and complete information
- Complies with this policy and all applicable laws
- Does not exploit any vulnerability for personal, financial, or competitive gain
- Allows BugThrive reasonable time to investigate and remediate before any disclosure

Researchers acting in good faith are covered under BugThrive's Safe Harbor.

---

## Prohibited Activities

> [!WARNING]
> The following activities are strictly prohibited, regardless of intent or framing.

**Availability attacks**
- Denial-of-service (DoS / DDoS), stress testing, load testing, or resource exhaustion of any kind

**Credential and account attacks**
- Credential stuffing, password spraying, or brute-force attacks
- Using credentials sourced from breaches, dumps, malware, or unauthorized means

**Data access and exposure**
- Accessing, reading, downloading, copying, retaining, or disclosing another user's data
- Accessing additional records beyond what is minimally necessary to confirm a vulnerability

**Deceptive tactics**
- Social engineering, phishing, or impersonation of BugThrive employees, customers, or partners
- Physical attacks against BugThrive offices, infrastructure, or personnel

**Destructive actions**
- Deleting, altering, corrupting, encrypting, or damaging data or systems
- Deploying malware, ransomware, spyware, or persistent malicious payloads

**Unauthorized scope expansion**
- Testing third-party services, infrastructure, or systems without explicit authorization
- Establishing persistence, moving laterally, or accessing systems beyond what demonstrating the vulnerability requires

**Misconduct**
- Using a discovered vulnerability for personal, commercial, financial, or competitive advantage
- Extortion, threats, coercion, or demands connected to disclosure or remediation
- Publicly disclosing vulnerability information without written confirmation from BugThrive
- Submitting raw, unvalidated, or duplicate automated scanner output

---

## Sensitive Data Handling

If you encounter personal information, credentials, API keys, tokens, financial data, or any other sensitive information during testing:

1. **Stop testing immediately**
2. Do not access additional records or explore further
3. Do not copy, download, retain, modify, transfer, or disclose the data
4. **Report the issue to BugThrive immediately**
5. Include only the minimum information required to document the finding
6. Redact all sensitive details from screenshots, videos, and proofs of concept

---

## Automated Testing

Automated security scanning is permitted only when:

- Limited strictly to in-scope assets
- Carefully configured, rate-limited, and non-disruptive
- Conducted in a way that does not affect service availability, performance, or users

**Researchers must manually validate all automated findings before submission.**

Automated testing does not authorize DoS, aggressive scanning, excessive traffic generation, or resource exhaustion. Submitting unverified scanner output may result in the report being closed without further review.

---

## Safe Harbor

BugThrive supports responsible, good-faith security research.

Research conducted in accordance with this policy is considered authorized. BugThrive will not initiate legal action against researchers solely for activity covered by this policy.

If a third party initiates legal action against a researcher for activities conducted in good-faith compliance with this policy, BugThrive may, where appropriate and legally permitted, clarify that the activity was authorized.

> [!WARNING]
> Safe harbor does not apply to activities that are out of scope, prohibited by this policy, involve intentional harm, privacy violations, data theft or retention, service disruption, extortion, unauthorized disclosure, or violations of applicable law.

If you are uncertain whether a proposed activity is permitted, contact BugThrive and obtain written clarification **before proceeding**.

---

## Coordinated Disclosure

All vulnerability information must remain **confidential** until BugThrive provides written confirmation that public disclosure may proceed.

Public disclosure includes, but is not limited to:

- GitHub Issues, Discussions, pull requests, or public commits
- Social media, blogs, forums, or conference talks
- Public advisories, mailing lists, news publications, or videos

Submitting a report does not automatically grant permission for public disclosure.

---

## Recognition

Researchers whose reports are validated may receive a **Letter of Appreciation**.

- BugThrive does **not** currently operate a monetary bug bounty program
- A Security Researcher Hall of Fame may be established in future; validated reporters may be considered for inclusion
- Public recognition requires the researcher's consent
- Recognition depends on report validity, quality, reproducibility, impact, and policy compliance

When multiple researchers report the same vulnerability, BugThrive may recognize the earliest report with sufficient detail to reproduce the issue. Later reports may be classified as duplicates.

---

## Contact

| Channel | Details |
|---|---|
| **GitHub (recommended)** | Private Vulnerability Reporting via the **Security** tab |
| **Email** | compliance@bugthrive.com |

---

## Governing Law

This policy is governed by applicable laws of India. BugThrive operates from Andhra Pradesh, India.

Nothing in this policy authorizes activity that violates applicable law or the rights of third parties.

---

*BugThrive may update this policy periodically. The version published in this repository is the authoritative version. Review it before beginning any security testing.*
