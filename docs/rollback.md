# Rollback Workflow

This document describes a reusable rollback workflow for failed deployments.

---

## Purpose

Rollback workflows help recover quickly from broken deployments.

They are useful when:

- A new deployment fails health checks
- A critical bug reaches production
- Service startup fails
- Configuration breaks runtime behavior

---

## Required Secrets

Configure these secrets in GitHub Actions:

- SSH_HOST
- SSH_USER
- SSH_PRIVATE_KEY
- SSH_PORT
- APP_DIR
- SERVICE_NAME
- HEALTHCHECK_URL

---

## Manual Input

The workflow requires:

- release_path

Example:

/opt/my-app/releases/20260531120000

---

## Rollback Flow

Select previous release  
Update current symlink  
Restart service  
Run healthcheck  
Confirm recovery

---

## Production Notes

- Keep previous releases available
- Validate rollback target before switching
- Always run healthchecks after rollback
- Document rollback events in incident notes