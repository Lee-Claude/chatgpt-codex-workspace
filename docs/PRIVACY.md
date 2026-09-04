# Privacy and Public-Repository Safety

This repository is public. Treat every committed file and every commit in its history as potentially visible to anyone.

## Never commit directly

Do not commit any of the following unless the user has deliberately approved that exact material for public release:

- passwords, API keys, access tokens, private keys, certificates, recovery codes, or credentials
- customer names linked to addresses, phone numbers, email addresses, IDs, signatures, banking data, meter numbers, account numbers, or other personal data
- customer contracts, quotations, invoices, applications, forms, correspondence, photos, scans, or project files that identify a customer
- confidential company documents, unpublished financial data, internal pricing logic, private supplier terms, or confidential third-party information

## Safer alternatives

When sensitive material is needed for a task, prefer one of these approaches:

1. redact or anonymize identifying information before committing
2. keep the source file outside Git and commit only a sanitized summary
3. move the sensitive work to a private repository
4. store secrets in the appropriate secret-management mechanism rather than source control

## Important Git fact

Deleting a sensitive file in a later commit does not automatically remove it from Git history. If a secret or private document is accidentally committed, treat it as exposed and take remediation steps immediately, including rotating credentials where applicable and removing the data from repository history when necessary.

## Pre-commit review checklist

Before committing, check changed files for:

- names, addresses, telephone numbers, email addresses, signatures, IDs, IBAN/account data
- `.env` values, tokens, passwords, certificates, private keys, credential JSON files
- customer-specific PDFs, images, spreadsheets, contracts, offers, or invoices
- internal financial or commercial information that was not intended for publication

If uncertain, stop and ask the user before publishing the material.
