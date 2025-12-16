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
- **QA Lead**: QA sign-off completed with all critical tests passed
- **DevOps Engineer**: Deployment pipeline verified and monitoring configured
- **Product Manager**: Feature acceptance and business validation complete
- **UX Designer**: UI/UX review completed for user-facing changes

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support
- [ ] **DevOps Engineer**: Monitor deployment metrics and system health
- [ ] **QA Lead**: Verify critical flows in production environment
- [ ] **Project Manager**: Update stakeholders on deployment status

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - **DevOps Engineer**: Execute rollback procedure to last known-good release if necessary
  - **QA Lead**: Verify rollback success and validate critical functionality
  - **Project Manager**: Coordinate communication with stakeholders
  - Triage root cause and capture action items
  - Schedule blameless postmortem with all involved roles

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
