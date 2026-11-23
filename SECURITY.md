# Security Policy

## Reporting

Configure a company-controlled security contact before public production release. Do not send secrets or customer data in public issue reports.

## Production controls

- Enforce TLS for all service traffic.
- Use a vetted identity provider, MFA for administrators, short-lived tokens, revocation, and rate limits.
- Encrypt data at rest and backups; apply least-privilege access and audit administrative actions.
- Design and independently review message encryption and key management before representing messages as end-to-end encrypted.
- Use secure media access controls, abuse reporting, retention policies, and tested backup recovery.
- Run dependency scanning, security testing, and incident-response exercises.

## Never commit

API secrets, private keys, signing certificates, passwords, credential-bearing database URLs, push certificates, session cookies, or user data.
