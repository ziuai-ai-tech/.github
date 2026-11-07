# Contributing to ZIUAI repositories

This file applies to every repository in the ZIUAI organization unless the repository has its own `CONTRIBUTING.md`. It is the short version of the [Developer Handbook](docs/01-developer-handbook.md); the handbook is the full set of rules and every developer signs it before writing code.

## Before you start

1. Read the [Developer Handbook](docs/01-developer-handbook.md) and sign it.
2. For a new project or a large feature, the [Before Development Checklist](docs/02-before-development-checklist.md) must be signed off by the tech lead before any code is written.
3. Make sure the repository runs locally by following its README. If it takes more than 15 minutes, open an issue about the README.

## Branches

- Never commit directly to `main`, `staging` or `production`.
- Branch from `main` and keep the branch short-lived.
- Name branches `feature/TICKET-123-short-name`, `fix/TICKET-456-login-error` or `hotfix/TICKET-789-short-name`.
- Every morning: `git checkout main && git pull`, then `git pull --rebase origin main` on your branch. Fix conflicts locally and re-run tests before pushing.

## Commits

- Follow [Conventional Commits](https://www.conventionalcommits.org/): `feat:`, `fix:`, `refactor:`, `test:`, `docs:`, `chore:`.
- One commit does one thing. No "final changes", "update" or "wip" messages on `main`.
- Run `git status` and `git diff` before every commit. Never `git add .` blindly.
- Never commit `.env`, keys, certificates, dumps or customer data. Only `.env.example` with placeholder values is committed.

## Before every push

```bash
npm run lint        # or: ruff check .
npm run test        # all tests green
npm run build       # it must build
```

## Pull requests

- Keep a PR under about 400 changed lines. Split larger work into several PRs.
- Fill in the PR template: what changed, why, how to test, screenshots for UI, linked ticket and the test report.
- CI must be green and the SonarQube quality gate must pass before you request review.
- At least 1 approval. Auth, payment, encryption, permission and infrastructure changes need 2, one from a senior.
- Review your own diff first. Reply to every review comment; never resolve someone else's comment without a fix or an answer.
- Squash or rebase so `main` stays readable, and delete the branch after merge.

## Tests

- Every new function and every bug fix comes with tests. A bug fix starts with a test that reproduces the bug.
- Coverage on new code: 80% or more. Mock external services; never call real third parties in unit tests.
- No skipped tests (`.skip`, `xit`) merged without a ticket.

## Code quality

- Files under 400 lines, functions under 40 lines, at most 4 parameters, nesting at most 3 levels.
- No hard-coded URLs, IPs, ports, keys, IDs or magic numbers. Use config and named constants.
- Handle every error; no empty catch blocks. Timeouts on every external call.
- No `console.log` / `print` debugging, commented-out code or unused imports.

## AI-assisted code

- Use only company-approved AI tools and accounts.
- Never paste secrets, customer data or confidential client code into an AI tool.
- You own every line you merge. Read it, be able to explain it, and verify every package it adds actually exists and is maintained.
- AI-written auth, payment, encryption or permission logic needs senior review.

## Reporting problems

- Bugs and feature requests: use the issue templates.
- Security vulnerabilities or a leaked secret: follow [SECURITY.md](SECURITY.md). Do not open a public issue.

## Questions

Ask in the team channel after 30 minutes stuck, with what you already tried. Asking early is part of the job.
