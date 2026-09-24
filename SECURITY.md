# Security and privacy — development notice

## Current state

This repository is at the documentation and planning stage. It does not currently publish a production-ready NoMore application, a supported security release or an independent security audit.

Security and privacy statements in the project documents describe requirements to be implemented and verified, not guarantees.

## Reporting a sensitive concern

Do not disclose vulnerabilities, credentials, sensitive screenshots or personal records in a public issue or pull request.

If GitHub displays a **Report a vulnerability** option in the repository's security advisory area, use that private reporting channel and share only the minimum technical information needed.

If that option is not available, open an issue containing only a request for a private reporting channel, without the vulnerability details or any personal data. Do not infer that a private channel is configured merely because this file exists.

At this early stage, no response-time commitment or emergency-monitoring service is advertised.

## Publication precautions

Never publish production secrets, environment files, personal journals, CRM exports, database dumps, private attachments or access tokens.

Review changes before publishing. A `.gitignore` file only supports a local Git workflow: it is not a confidentiality barrier, does not remove previously committed content and must not be relied on to protect a manual browser upload.

If a secret is exposed, treat it as compromised and arrange revocation or rotation through the appropriate service. Deleting the visible file alone must not be treated as a complete remedy.

## Future release expectations

Before processing real user records, the project needs verified access isolation, secure authentication, protected administrative functions, appropriate logging and retention, export/deletion tests, backup-restoration tests and incident procedures.

Development tools, public demos, examples and tests must use synthetic data. A project document or an automated check is not a substitute for review of the actual application and hosting environment.

This repository is a software-development space, not a confidential place for personal health disclosures or urgent assistance.

## Reference documentation

- [GitHub: ignoring files](https://docs.github.com/en/get-started/git-basics/ignoring-files).
- [GitHub: removing sensitive data](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository).
- [GitHub: configuring private vulnerability reporting](https://docs.github.com/en/code-security/how-tos/report-and-fix-vulnerabilities/configure-vulnerability-reporting/configure-for-a-repository).
