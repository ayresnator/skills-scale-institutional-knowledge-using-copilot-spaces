# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- QA Lead sign-off confirming test coverage and acceptance criteria validation
- Passing CI and security scans (verified by DevOps Engineer and Security Champion)
- Release notes drafted and reviewed by Release Manager
- Rollback / mitigation plan documented and approved by Release Manager
- Smoke tests prepared and reviewed by QA Lead

## Deployment Checklist
- [ ] Deployment window scheduled and confirmed by Release Manager
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (coordinated by DevOps Engineer)
- [ ] QA Lead confirms staging smoke tests pass
- [ ] Release Manager issues go/no-go decision
- [ ] Deploy to production (automated pipeline managed by DevOps Engineer)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (DevOps Engineer leads technical response)
  - Release Manager initiates rollback decision
  - Rollback to last known-good release if necessary (executed by DevOps Engineer)
  - Security Champion notified if incident has security implications
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
