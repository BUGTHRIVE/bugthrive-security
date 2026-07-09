# Authorized Scope

This document defines the assets authorized for security testing under the BugThrive Vulnerability Disclosure Policy. Read this carefully before beginning any security research.

---

## In Scope

The following BugThrive-owned assets are authorized for security testing:

| Asset | Details |
|---|---|
| Production web applications | Officially deployed BugThrive web apps |
| Domains and subdomains | `*.bugthrive.com` (actively operated only) |
| Official APIs | Publicly accessible BugThrive APIs |
| GitHub repositories | Public repos officially owned or maintained by BugThrive |

An asset is considered in scope **only** when it is officially deployed, actively operated, and controlled by BugThrive.

---

## Out of Scope

The following assets are **not** authorized for security testing:

- Unofficial, deprecated, unsupported, or unauthorized deployments
- Domains, subdomains, or services not owned or controlled by BugThrive
- Subdomains or pages displaying a "Coming Soon" notice
- Third-party applications, integrations, vendors, or platforms
- Customer-owned systems or environments
- Assets that BugThrive does not have authorization to permit testing against

> The presence of a third-party service on a BugThrive domain does not make it eligible for testing. Researchers are responsible for reviewing and complying with third-party policies independently.

---

## Not Sure?

If you are uncertain whether an asset is in scope, contact us at `compliance@bugthrive.com` **before** conducting any testing.

Do not assume an asset is authorized — when in doubt, ask first.

---

*For full researcher guidelines, see the [Security Policy](SECURITY.md).*
