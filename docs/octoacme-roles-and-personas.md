# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Scrum Master

### Role Summary
The Scrum Master facilitates Agile ceremonies, removes impediments, and coaches the team on Agile best practices. They protect the team's focus and help sustain a culture of continuous improvement.

### Responsibilities
- Facilitate daily standups, sprint planning, sprint reviews, and retrospectives
- Identify and remove blockers that prevent the team from making progress
- Coach team members on Agile principles and practices
- Shield the team from unplanned scope changes during a sprint
- Track sprint health and velocity; surface trends to the Project Manager

### Goals
- Keep ceremonies efficient and outcome-focused
- Reduce cycle time and eliminate waste
- Foster psychological safety and continuous improvement within the team

### Typical Communication
- Daily standup facilitation and blocker triage
- Sprint metrics summaries shared with Project Managers and Product Managers
- Retrospective action items tracked and followed up on

### Interactions with Existing Roles
- **Project Manager**: Shares sprint health data and escalates blockers that require cross-team coordination.
- **Product Manager**: Ensures backlog items are refined and ready before sprint planning; negotiates scope changes.
- **Developers**: Removes impediments, clarifies process, and supports self-organization.

---

## UX Designer

### Role Summary
UX Designers advocate for user needs and translate requirements into clear, validated design solutions. They bridge the gap between business goals and user experience to help the team build the right thing.

### Responsibilities
- Create user flows, wireframes, and interactive prototypes
- Conduct usability studies and synthesize findings into actionable recommendations
- Define and document UX acceptance criteria for features
- Collaborate on feature definition to ensure design feasibility
- Maintain a design system and component library aligned to product standards

### Goals
- Deliver user-centered designs that reduce friction and improve satisfaction
- Reduce rework by validating assumptions early through prototyping and testing
- Ensure design consistency across the product

### Typical Communication
- Design reviews and feedback sessions with Product Managers and Developers
- Usability test reports and research summaries
- Design handoff notes and annotated specifications

### Interactions with Existing Roles
- **Product Manager**: Collaborates closely on problem framing, user research, and feature definition.
- **Developers**: Provides design specs and is available to answer implementation questions during development.
- **Quality Assurance Lead**: Reviews builds for visual and interaction accuracy against approved designs.
- **Project Manager**: Raises design risks or dependencies that may affect the project timeline.

---

## DevOps Engineer

### Role Summary
DevOps Engineers maintain CI/CD pipelines, deployment automation, and system reliability. They enable teams to ship safely and frequently while monitoring production health.

### Responsibilities
- Design, build, and maintain CI/CD pipelines and deployment automation
- Monitor reliability metrics (uptime, latency, error rates) and respond to incidents
- Manage infrastructure provisioning and configuration as code
- Enforce security scanning and dependency checks in the pipeline
- Coordinate and execute production deployments; document rollback procedures

### Goals
- Maximize deployment frequency while minimizing failure rate and recovery time
- Reduce manual toil through automation
- Maintain high reliability and observability in production environments

### Typical Communication
- Release coordination meetings with Project Managers and Product Managers
- Incident status updates and post-mortems shared with the full team
- Pipeline and infrastructure documentation updated in the repo

### Interactions with Existing Roles
- **Developers**: Provides guidance on CI/CD integration; reviews changes that affect pipelines or infrastructure.
- **Quality Assurance Lead**: Coordinates automated test execution in the pipeline; aligns on deployment gates.
- **Project Manager**: Confirms deployment windows, communicates release readiness, and reports on incidents.
- **Product Manager**: Raises reliability risks and infrastructure constraints that could affect the roadmap.

---

## Business Analyst

### Role Summary
Business Analysts gather and clarify requirements, analyze business processes, and bridge communication between business stakeholders and the delivery team. They ensure that what is built aligns with what the business actually needs.

### Responsibilities
- Elicit, document, and validate business and functional requirements
- Translate business needs into clearly scoped, actionable user stories
- Facilitate requirements workshops and stakeholder interviews
- Support user acceptance testing (UAT) and sign-off activities
- Identify process inefficiencies and propose improvements

### Goals
- Ensure requirements are clear, complete, and traceable before development begins
- Minimize rework caused by misunderstood or ambiguous requirements
- Improve cross-functional alignment between business and delivery teams

### Typical Communication
- Requirements documentation and user story write-ups shared with Product Managers and Developers
- UAT session facilitation and sign-off reports
- Regular check-ins with stakeholders to confirm scope and priorities

### Interactions with Existing Roles
- **Product Manager**: Works closely to refine epics and stories; validates that acceptance criteria reflect business intent.
- **Project Manager**: Flags scope changes early; contributes to risk and dependency tracking.
- **Developers**: Clarifies requirements during development; reviews implementations against business needs.
- **Quality Assurance Lead**: Provides acceptance criteria inputs and supports UAT planning.

---

## Quality Assurance Lead

### Role Summary
The Quality Assurance Lead defines the testing strategy and oversees the quality of all deliverables. They ensure that features meet acceptance criteria and that releases are safe to ship.

### Responsibilities
- Define and maintain the overall test strategy and test plans for each release
- Create, review, and triage test cases covering functional, regression, and non-functional areas
- Coordinate testing activities across the team and manage test environments
- Report on quality metrics (defect density, test coverage, pass/fail rates)
- Own the Definition of Done quality gates and enforce them before releases
- Collaborate with DevOps on automated test integration in CI/CD pipelines

### Goals
- Catch defects as early as possible in the development lifecycle
- Maintain high product quality and reduce escape rates to production
- Build confidence in each release through clear, evidence-based quality reporting

### Typical Communication
- Test plans and quality reports shared with Project Managers and Product Managers
- Bug triage sessions and defect reports with Developers and the Scrum Master
- Release readiness sign-offs coordinated with DevOps and Project Managers

### Interactions with Existing Roles
- **Developers**: Reviews implementation against acceptance criteria; collaborates on unit and integration test coverage.
- **Project Manager**: Reports on quality status; raises test-blocking risks that could affect the release timeline.
- **Product Manager**: Validates acceptance criteria completeness; escalates ambiguities that block test planning.
- **DevOps Engineer**: Integrates automated tests into the CI/CD pipeline; aligns on deployment quality gates.
- **Scrum Master**: Raises testing bottlenecks in retrospectives; contributes to sprint health tracking.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [`octoacme-project-kickoff-checklist.md`](octoacme-project-kickoff-checklist.md) for a RACI ownership matrix that maps these roles to key project activities.

