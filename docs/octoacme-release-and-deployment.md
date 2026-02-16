# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

### QA Sign-off Checklist
- [ ] Test plan executed and documented
- [ ] All critical and high-priority bugs resolved or accepted
- [ ] Smoke tests pass in staging environment
- [ ] Acceptance criteria validated for all features
- [ ] Performance and security testing completed (if applicable)
- [ ] QA Lead approval obtained

### DevOps Pre-release Checklist
- [ ] CI/CD pipeline green for release candidate
- [ ] Infrastructure and environment capacity verified
- [ ] Monitoring and alerting configured for new features
- [ ] Rollback procedure tested and documented
- [ ] Deployment runbook updated

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) — **Project Manager**
- [ ] Backup or snapshot (if applicable) — **DevOps/Platform Engineer**
- [ ] Deploy to staging and run smoke tests — **DevOps + QA Lead**
- [ ] Deploy to production (automated pipeline preferred) — **DevOps/Platform Engineer**
- [ ] Run post-deploy verifications — **QA Lead**
- [ ] Announce release to stakeholders and support — **Product Manager + Project Manager**

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
