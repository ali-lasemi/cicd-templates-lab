# SSH Deployment Workflow

This document describes a reusable SSH-based deployment workflow.

---

## Purpose

The SSH deployment workflow is designed for applications deployed directly to Linux servers.

It can be used for:

- Node.js applications
- Nuxt applications
- Backend services
- Small production environments
- VPS-based deployments

---

## Required Secrets

Configure these secrets in GitHub Actions:

- SSH_HOST
- SSH_USER
- SSH_PRIVATE_KEY
- SSH_PORT
- APP_PATH
- SERVICE_NAME
- HEALTHCHECK_URL

---

## Deployment Flow

```txt
Checkout code
  ↓
Connect over SSH
  ↓
Pull latest code
  ↓
Install dependencies
  ↓
Build application
  ↓
Restart service
  ↓
Run healthcheck