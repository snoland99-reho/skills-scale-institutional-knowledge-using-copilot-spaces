# OctoAcme — Project Kickoff Checklist & RACI Ownership Matrix

## Purpose
Provide a repeatable checklist for project kickoffs and a lightweight RACI matrix that makes role ownership explicit from day one. Use this template alongside the [Project Initiation Guide](octoacme-project-initiation.md) and [Project Planning](octoacme-project-planning.md) docs.

---

## Project Kickoff Checklist

Complete the following before or during the kickoff meeting.

### Pre-Kickoff (Project Manager + Product Manager)
- [ ] One-pager drafted and approved (see [Project Initiation Guide](octoacme-project-initiation.md))
- [ ] Key stakeholders identified and invited to the kickoff
- [ ] RACI matrix below filled in for this project
- [ ] Initial risk register created (see [Risk Management & Communication](octoacme-risks-and-communication.md))
- [ ] Definition of Ready (DoR) and Definition of Done (DoD) drafted (see [Definition of Ready / Done](#definition-of-ready--done-template) below)

### Kickoff Meeting Agenda
1. Project overview and objectives (Product Manager)
2. Scope, constraints, and non-goals (Product Manager + Business Analyst)
3. Role and ownership assignments — walk through the RACI matrix (Project Manager)
4. High-level timeline and milestones (Project Manager)
5. Identified risks and dependencies (Project Manager + Business Analyst)
6. Definition of Ready / Done review (Scrum Master + QA Lead)
7. Communication plan and cadence (Project Manager)
8. Q&A and next steps

### Post-Kickoff (within 48 hours)
- [ ] RACI matrix finalized and shared with all team members
- [ ] DoR / DoD documented in the project repo or board
- [ ] Project board created with initial backlog items
- [ ] Communication cadence scheduled (standups, weekly syncs, demos)
- [ ] Risk register published in the project repo
- [ ] Kickoff notes and decisions captured and distributed

---

## RACI Ownership Matrix Template

**How to read:** For each key activity, assign one of:
- **R** — Responsible (does the work; multiple R entries per row are allowed when work is shared)
- **A** — Accountable (final decision-maker / sign-off; exactly **one** A per row)
- **C** — Consulted (provides input before or during the work)
- **I** — Informed (kept up to date after decisions are made)

> When the same person is both Accountable and Responsible (i.e., they own and do the work), assign **A** in that cell. A separate **R** is only needed when responsibility is shared with other roles.

Replace role names in the header row if your team uses different titles. Add or remove rows as needed for your project.

| Activity | Project Manager | Product Manager | Scrum Master | Business Analyst | UX Designer | Developers | QA Lead | DevOps Engineer |
|---|---|---|---|---|---|---|---|---|
| Define project objectives & success metrics | C | **A** | I | C | I | I | I | I |
| Maintain and prioritize the backlog | I | **A** | C | R | C | C | C | I |
| Backlog refinement & story sizing | C | C | **A** | R | C | R | C | I |
| Sprint planning facilitation | I | C | **A** | I | I | R | C | I |
| UX research & design sign-off | I | C | I | C | **A** | C | C | I |
| Requirements documentation | C | **A** | I | R | C | I | C | I |
| Technical architecture decisions | I | C | I | I | I | **A** | C | R |
| CI/CD pipeline & deployment automation | I | I | I | I | I | C | C | **A** |
| Test strategy & test plan | I | C | C | C | I | C | **A** | C |
| Acceptance criteria review | C | **A** | I | R | C | R | R | I |
| Release coordination & go/no-go | **A** | C | I | I | I | C | R | R |
| Release communications to stakeholders | **A** | C | I | I | I | I | I | C |
| Incident escalation & response | **A** | I | I | I | I | C | C | R |
| Retrospective facilitation | C | I | **A** | I | I | R | R | I |
| Risk register maintenance | **A** | C | C | C | I | I | I | I |
| Stakeholder status reporting | **A** | C | I | I | I | I | I | I |

> **Note:** Each activity has exactly one **A** (Accountable). Multiple **R** entries are allowed when work is shared across roles. An **A** without a separate **R** means the Accountable person is also performing the work.

---

## Cross-Functional Handoff Checklist

Use this checklist when handing off work between key delivery phases.

### Product → Engineering Handoff (PdM + BA → Developers + Scrum Master)
- [ ] User stories written with clear acceptance criteria
- [ ] UX designs finalized and linked in stories
- [ ] Business Analyst has reviewed stories for completeness
- [ ] Stories meet the Definition of Ready (see below)
- [ ] Dependencies and integration points documented

### Engineering → QA Handoff (Developers → QA Lead)
- [ ] Feature branch merged and CI build passing
- [ ] Unit and integration tests written and passing
- [ ] Known edge cases documented for QA
- [ ] Test environment updated and stable
- [ ] DevOps notified if environment changes are needed

### QA → Release Handoff (QA Lead + DevOps Engineer → Project Manager)
- [ ] All test cases executed; results documented
- [ ] No open P0/P1 defects; known issues recorded
- [ ] Release notes reviewed by QA Lead and Product Manager
- [ ] Rollback plan confirmed with DevOps Engineer
- [ ] Go/no-go decision recorded (Project Manager is Accountable)

---

## Definition of Ready / Done Template

### Definition of Ready (DoR)
A backlog item is **Ready** for sprint planning when:
- [ ] User story is written in agreed format (As a… I want… So that…)
- [ ] Acceptance criteria are defined and unambiguous
- [ ] UX designs are attached or linked (for user-facing work)
- [ ] Business Analyst has reviewed and signed off on requirements
- [ ] Dependencies are identified and unblocked (or a mitigation plan exists)
- [ ] Story is estimated by the team
- [ ] Test scenarios are outlined by QA Lead

### Definition of Done (DoD)
A backlog item is **Done** when:
- [ ] All acceptance criteria are met
- [ ] Code reviewed and approved per team policy
- [ ] Automated tests written and passing in CI
- [ ] Manual QA completed and sign-off received from QA Lead
- [ ] Documentation updated (API docs, README, runbook as appropriate)
- [ ] Feature flagged or deployed to staging by DevOps
- [ ] No regression in existing functionality
- [ ] Release notes updated

---

## Related Documents
- [Roles & Personas](octoacme-roles-and-personas.md) — full descriptions of all team roles
- [Project Initiation Guide](octoacme-project-initiation.md) — how to get a project approved
- [Project Planning](octoacme-project-planning.md) — backlog creation and sprint planning
- [Execution & Tracking](octoacme-execution-and-tracking.md) — ceremonies, workflows, and metrics
- [Release & Deployment Guide](octoacme-release-and-deployment.md) — release coordination and deployment
- [Risk Management & Communication](octoacme-risks-and-communication.md) — risk register and escalation paths
