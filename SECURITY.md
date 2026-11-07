# Security Policy

This policy applies to every repository in the ZIUAI organization unless the repository has its own `SECURITY.md`.

## Reporting a vulnerability

Do not open a public issue or pull request for a security problem.

1. Preferred: use GitHub's private reporting. On the affected repository, open the **Security** tab and choose **Report a vulnerability**.
2. Otherwise, email **admin@ziuai.ai** with the subject `Security report: <repository name>`.

Include what you found, the repository and commit or version, steps to reproduce, and the impact as you understand it. Do not include real customer data in the report; use fake examples.

We acknowledge reports within 2 working days and give an initial assessment within 5 working days. We ask that you give us reasonable time to fix the issue before any public disclosure, and we will credit you in the fix if you want.

## Scope

- Any repository, service, API or application maintained by the ZIUAI organization.
- Out of scope: findings that need physical access to a device, social engineering of staff, denial-of-service testing, and automated scanner output without a confirmed issue.

## If you leaked a secret

A secret pushed to Git is a leaked secret, even if you delete it a minute later. Bots scan GitHub constantly.

1. Tell the tech lead immediately. Do not wait to be sure.
2. Rotate the key, token or password first. This is the only step that actually stops the damage.
3. Only then clean the Git history and force-push with the lead's approval.
4. Check logs for use of the leaked secret between the push and the rotation.
5. If customer data may be affected, the lead starts the breach process (CERT-In reporting within 6 hours).

## Supported versions

Security fixes go to the `main` branch and the latest release of each product. Older releases receive fixes only when a customer contract requires it.

## Security practices we follow

The full rules live in the [Developer Handbook](docs/01-developer-handbook.md), the [Before Development Checklist](docs/02-before-development-checklist.md) and the [Before Launch Checklist](docs/03-before-launch-checklist.md). In short:

- Secrets in a vault or CI secrets store, never in code or committed `.env` files; secret scanning and push protection enabled.
- Dependency and container scanning on every pull request; critical findings block the merge.
- OWASP Top 10 and ASVS used as the baseline; threat modeling before code for new systems.
- Least-privilege access, two-factor authentication for every account, and read-only production access by default.
- No real customer data outside production.
