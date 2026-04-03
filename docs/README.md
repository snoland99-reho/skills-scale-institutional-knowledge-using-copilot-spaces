# OctoAcme Project Management Docs

This README provides an overview of project management processes at OctoAcme and links to detailed documentation for each area. Centralizing these docs makes them searchable and version-controlled, improving onboarding, consistency, and discoverability for all team members.

## Overview of Project Management Processes

OctoAcme's project management approach follows a lightweight, repeatable lifecycle designed for cross-functional delivery: **Initiation → Planning → Execution → Release → Retrospective/Improvement**. Work begins in **Project Initiation** with a clear problem statement, SMART objectives, success metrics, stakeholder alignment, a high-level timeline, and an initial risk list—captured in a concise **Project One-pager/Charter**. Once there is a go/no-go decision, the team moves into **Project Planning**, where scope is decomposed into shippable increments, a prioritized backlog is created with explicit acceptance criteria, estimates are produced, dependencies are identified, and a Definition of Done and release/milestone map are agreed upon.

Roles are clearly defined to support clear ownership and fast execution. The **Project Manager (PM)** coordinates delivery mechanics (schedule, risks, communications, ceremonies, and documentation consistency). The **Product Manager (PdM)** owns outcomes—defining success metrics, prioritizing the backlog, and guiding trade-offs with stakeholders. **Developers** implement features with an emphasis on testability and maintainability, while **QA/Testing** validates acceptance and quality. **Stakeholders/Sponsors** provide inputs and approvals and participate in escalations when business impact warrants it. These personas are used throughout the process docs to set expectations for who owns decisions, execution, and communication at each stage.

Execution emphasizes visible work tracking and disciplined collaboration. OctoAcme uses a project board (e.g., GitHub Projects) with a standard flow—**Backlog → Ready → In Progress → In Review → QA → Done**—supported by a regular team rhythm (daily standups, weekly delivery syncs, and sprint/milestone demos). Communication is structured with weekly PM+PdM alignment, regular team standups, monthly stakeholder updates, and standardized templates for weekly status and incident updates. Risks are managed via a **Risk Register** (impact/likelihood/owner/mitigation/status) reviewed regularly, and blockers follow a defined escalation path from team triage up through PM/Product Lead to sponsor-level escalation when needed.

Quality assurance and release practices are embedded throughout delivery. PRs are kept small, include linked issues and acceptance criteria, and require CI (tests/lint/security scanning) and at least one approval before merge. Testing expectations include unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, and manual QA when needed for feature acceptance. Releases are standardized with explicit pre-release requirements (acceptance criteria met, CI/scans passing, release notes, rollback plan, smoke tests) and a deployment checklist spanning staging validation, production deployment, post-deploy verification, and stakeholder announcements. After sprints, releases, or incidents, OctoAcme runs retrospectives to capture learnings, assign owners to a small set of improvements, and track those actions in the backlog to continuously refine how the team delivers.

## Documents

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles and Personas](octoacme-roles-and-personas.md)

---

Add or update documents in the `docs/` folder as needed.
