# ZIUAI Engineering Documentation

This folder holds the engineering standards every developer at ZIUAI follows. Read the documents in the order below. Each one builds on the one before it, and together they cover a project from the first planning meeting to the weeks after launch.

## Reading order

| # | Document | Who reads it | When | Formats |
| --- | --- | --- | --- | --- |
| 1 | [Developer Handbook](01-developer-handbook.md) | Every developer | On joining, before writing any code | [DOCX](downloads/Developer%20Handbook.docx) · [PDF](downloads/Developer%20Handbook.pdf) |
| 2 | [Before Development Checklist](02-before-development-checklist.md) | Tech lead, product owner, whole team | At the start of every project, before coding | [DOCX](downloads/Before%20Development%20Checklist.docx) · [PDF](downloads/Before%20Development%20Checklist.pdf) |
| 3 | [Before Launch Checklist](03-before-launch-checklist.md) (Engineering Production Playbook) | Tech lead, DevOps, product, whole team | One week before go-live, and after launch | [DOCX](downloads/Engineering%20Production%20Playbook.docx) · [PDF](downloads/Engineering%20Production%20Playbook.pdf) |

## Learning path: beginner to advanced

The handbook defines three levels. Use this path to know what to read first and what to come back to later.

### Level 1: Basics (0–2 years, and every new joiner)

Read the [Developer Handbook](01-developer-handbook.md) end to end and sign it. Focus on:

- Daily workflow: pull every morning, small branches, Conventional Commits, pull requests under 400 lines
- Code quality rules: the 400-line file limit, the 40-line function limit, no hard-coding
- Config, `.env`, `.gitignore` and secrets: a secret pushed to Git is a leaked secret
- Unit testing and the test report attached to every PR
- SonarQube quality gate: fix issues before pushing
- Using Claude Code well: plan mode, review every line, never paste secrets or customer data

### Level 2: Intermediate (2–5 years)

Everything in Level 1, plus the [Before Development Checklist](02-before-development-checklist.md). Focus on:

- Folder structure and architecture: routes, controllers, services, repositories
- API and database design: OpenAPI first, versioning, indexes, UTC, money as integers
- Security by design: threat modeling, OWASP Top 10, authorization on every endpoint
- Data and privacy by design: DPDP and GDPR, delete-my-data and export-my-data flows
- Reviewing other people's PRs and setting up the team's `CLAUDE.md`, hooks and skills

### Level 3: Advanced (5+ years, seniors and leads)

Everything above, plus you own the [Before Launch Checklist](03-before-launch-checklist.md). Focus on:

- Running the Production Readiness Review and the go / no-go meeting
- SLOs, observability, backups, rollback and canary releases
- Incident response and blameless postmortems
- The team training plan (four weekly sessions) and the launch sign-off
- Writing design docs and ADRs, and mentoring Level 1 and Level 2 developers

## How the three documents fit together

```text
Project start                 During development              One week before go-live        After launch
     |                               |                                |                           |
     v                               v                                v                           v
Before Development Checklist   Developer Handbook (daily)      Before Launch Checklist      Day 1 and ongoing habits
(signed off by tech lead)      (every developer, every PR)     (Production Readiness Review) (weekly, monthly, per incident)
```

## Folder layout

```text
docs/
  README.md                              This index and learning path
  01-developer-handbook.md               Rules every developer follows
  02-before-development-checklist.md     Planning sign-off before coding
  03-before-launch-checklist.md          Production readiness and launch sign-off
  downloads/                             The same documents as DOCX and PDF
```

## Keeping these documents up to date

- Changes go through a pull request, like code. Describe what changed and why.
- Update the Markdown, DOCX and PDF together so all three formats say the same thing.
- When the Developer Handbook changes, every developer signs it again (see its sign-off table).
