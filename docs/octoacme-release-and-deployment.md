# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (verified by **DevOps Engineer**)
- **QA Lead** sign-off: all planned test cases executed, no open P0/P1 defects
- Release notes drafted and reviewed by **Product Manager**
- Rollback / mitigation plan documented by **DevOps Engineer**
- Smoke tests prepared and approved by **QA Lead**
- Go/no-go decision recorded by **Project Manager** (see [QA → Release Handoff checklist](octoacme-project-kickoff-checklist.md#qa--release-handoff-qa-lead--devops-engineer--project-manager))

## Deployment Checklist
- [ ] Go/no-go decision recorded — **Project Manager** is Accountable
- [ ] Deployment window scheduled and communicated by **Project Manager** (if needed)
- [ ] Backup or snapshot completed by **DevOps Engineer** (if applicable)
- [ ] **DevOps Engineer** deploys to staging; **QA Lead** runs smoke tests
- [ ] **DevOps Engineer** deploys to production (automated pipeline preferred)
- [ ] **QA Lead** runs post-deploy verifications
- [ ] **Project Manager** announces release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **DevOps Engineer** triggers incident response and notifies on-call
  - **Project Manager** handles stakeholder communication (see [Incident Communication template](octoacme-risks-and-communication.md#communication-templates))
  - Rollback to last known-good release executed by **DevOps Engineer** if necessary
  - **QA Lead** verifies system stability after rollback
  - Triage root cause and capture action items; schedule blameless post-mortem

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
