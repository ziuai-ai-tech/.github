## What changed

<!-- One or two lines. What does this PR do? -->

## Why

<!-- The problem or ticket this solves. Link the ticket below. -->

Ticket:

## How to test

<!-- Steps a reviewer can follow to see it working. -->

1.
2.

## Screenshots

<!-- Required for any UI change. Before / after if useful. Delete this section for backend-only changes. -->

## Test report

- Unit tests: `N passed, 0 failed`
- Coverage on new code: `NN%`
- Integration tests: passed / N/A
- Manual test: steps tried
- SonarQube quality gate: Passed

## Checklist

- [ ] PR is under ~400 changed lines (split it if bigger)
- [ ] Branch name follows `feature/TICKET-123-short-name`, `fix/...` or `hotfix/...`
- [ ] Commits follow Conventional Commits (`feat:`, `fix:`, `refactor:`, `test:`, `docs:`, `chore:`)
- [ ] `lint`, `test` and `build` pass locally
- [ ] CI is green and the SonarQube quality gate passed
- [ ] New code has unit tests; bug fixes start with a test that reproduces the bug
- [ ] No secrets, `.env` files, keys, customer data or hard-coded URLs / IDs / magic numbers
- [ ] No `console.log` / `print` debugging, commented-out code or unused imports
- [ ] Errors are handled (no empty catch blocks) and every external call has a timeout
- [ ] Docs, `.env.example` and `CLAUDE.md` updated if the change needs it
- [ ] I reviewed my own diff before requesting review
- [ ] Auth, payment, encryption, permission or infrastructure change: **2 approvals required**, one from a senior
- [ ] AI-generated code: I read every line and can explain it; every new package exists and is maintained
