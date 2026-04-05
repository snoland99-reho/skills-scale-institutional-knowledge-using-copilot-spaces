# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner (see [Roles & Personas](octoacme-roles-and-personas.md) for role definitions)
- Mitigation plan
- Status

**Default risk owners by type:**
- Schedule / scope risks → **Project Manager**
- Requirements ambiguity → **Business Analyst** + **Product Manager**
- Technical / architecture risks → **Developers** + **DevOps Engineer**
- Quality / testing risks → **QA Lead**
- Process / team dynamic risks → **Scrum Master**

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- **Project Manager** owns stakeholder status reporting; **Scrum Master** owns team-facing communication
- **Business Analyst** ensures business stakeholders are kept informed of scope and requirements decisions
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level → **Scrum Master** (impediment removal and team-level triage)
- **Scrum Master** → **Project Manager** (cross-team or resource-level escalation)
- **Project Manager** → Product Lead → Sponsor (business-impacting escalation)
- For security incidents, **DevOps Engineer** leads triage; follow the security incident runbook and notify Security on-call
- For requirements disputes, **Business Analyst** facilitates resolution between stakeholders and the delivery team
