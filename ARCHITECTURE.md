# NoMore — Architecture proposal

**Design proposal only. No working application is included in this documentation package.**

## Application boundaries

NoMore is intended to provide three distinct areas:

1. Public presentation and approved support resources.
2. Private personal accounts for journals, goals and progress summaries.
3. An administration area for content, translations, resources and limited account operations.

Administrative access must not imply unrestricted access to personal journals. Roles, exceptional support access and audit requirements must be specified before implementation.

## Technical direction

- Structured PHP application using a maintained PHP version selected at implementation time.
- MySQL or MariaDB, with an explicit supported-version matrix and tested migrations.
- Semantic HTML, modern CSS and lightweight JavaScript with progressive enhancement.
- Small, maintained dependencies where they reduce security or maintenance risk; no unnecessary framework or custom cryptography.
- Deployment documentation suitable for a supported Plesk environment, with preflight checks rather than an assumption that every hosting plan is compatible.

## Proposed separation of files

```text
public/       Public entry point and approved static assets only.
app/          Application logic, access control, templates and services.
config/       Configuration templates; production secrets excluded from Git.
database/     Reviewed schema and migrations; no real user data.
storage/      Private runtime data; excluded from the repository.
tests/        Tests using synthetic data.
```

This tree is a proposal for future code, not a claim that these directories are already implemented. Public web access must be limited to `public/` in the deployed application.

## Data and calculation requirements

Entries must belong to an authenticated individual and remain isolated from other users. No cross-user league table or administrative browsing of journals is planned.

A missing entry is not a zero. Calculations must define their date range, baseline, currency, units and missing-data policy. Financial projections must be labelled as estimates, not guaranteed savings. Descriptive charts must not generate diagnoses or personalised life-expectancy claims.

Alcohol quantities and gambling cash flows require their own specifications. A single generic "addiction score" is not part of the intended design.

## Internationalisation

Interface text must be separated from application logic. French, English and Spanish are initial targets; country selection is separate from language selection.

Translated safety text and local support contacts require a publication workflow with source, review date and reviewer status. Browser translation alone is not the intended localisation system.

## Security and privacy requirements to implement and verify

Server-side authorisation, secure authentication and session management, CSRF protection, contextual output escaping, prepared database queries, rate limiting and protected recovery flows are requirements.

Secrets, personal records and sensitive logs must stay outside the public directory and outside version control. Export and deletion must include appropriate identity checks and a documented backup-retention policy. Encryption decisions require a threat model and managed keys; encryption is not a substitute for access control.

No third-party behavioural tracking or session replay is planned in private account areas. Production records must not be supplied to development assistants; tests and demonstrations must use synthetic data.

Before real-data processing, the project must determine its legal basis, obligations for sensitive data, hosting requirements, operating responsibilities and incident procedures. This document does not certify compliance or security.

## Reuse and integration

Reuse of existing SaaS components remains an architectural option, not an implemented integration. Any reuse requires review of ownership, licences, dependencies, security and isolation from unrelated business records.

No unrelated CRM archive, client dataset or production configuration should be uploaded to this repository as evidence of progress.

## Review gates

Future releases should publish verified test results and known limitations. Security, accessibility and safety-sensitive changes require appropriate review; generated code or a completed checklist alone is not evidence that a release is safe.
