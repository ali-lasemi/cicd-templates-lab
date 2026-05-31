# Environment Promotion Workflow

This document describes a reusable environment promotion workflow.

---

## Purpose

Environment promotion workflows help move tested releases between environments.

Example flow:

Development → Staging → Production

---

## Inputs

- source_environment
- target_environment
- version

---

## Promotion Flow

Validate promotion request  
Select target environment  
Apply environment protection rules  
Deploy selected version  
Verify deployment health

---

## Production Notes

- Use protected environments
- Require approvals for production
- Promote immutable artifacts
- Avoid rebuilding between environments
- Track promoted versions