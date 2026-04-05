# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — facilitated by the **Scrum Master**; focus on progress, blockers, and dependencies
- Weekly delivery sync — Project Manager runs status updates; QA Lead reports quality metrics; DevOps reports pipeline health
- Demo/Review at the end of each sprint or milestone — Product Manager accepts completed work against Definition of Done

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic (owned by **Developers**)
- Integration tests where applicable (Developers + QA Lead)
- End-to-end smoke tests for critical flows before release (owned by **QA Lead**)
- Security scanning and dependency checks in CI (owned by **DevOps Engineer**)
- Manual QA and acceptance testing against the Definition of Done (owned by **QA Lead**)
- QA Lead reports defect status and quality metrics at the weekly delivery sync
- See [Definition of Done template](octoacme-project-kickoff-checklist.md#definition-of-ready--done-template) for quality gates required before a story is considered complete

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup (facilitated by **Scrum Master**)
- Level 2: **Project Manager** escalates to Product Lead and dependent teams; **Scrum Master** escalates persistent impediments to PM
- Level 3: Sponsor-level escalation for business-impacting issues (Project Manager is Accountable)
- For production incidents, **DevOps Engineer** leads triage; Project Manager handles stakeholder communication

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI pipeline configured by DevOps Engineer (tests, lint, security scans)
- [ ] RACI Ownership Matrix published (see [Project Kickoff Checklist](octoacme-project-kickoff-checklist.md))
- [ ] Definition of Done enforced by QA Lead before stories move to Done
- [ ] Regular demos scheduled (Scrum Master coordinates)
- [ ] Risk register updated weekly (Project Manager)
