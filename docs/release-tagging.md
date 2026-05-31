# Release Tagging Workflow

This document describes an automated release tagging workflow.

---

## Purpose

Release tagging helps teams create consistent and traceable software releases.

The workflow supports:

- Manual version input
- Git tag creation
- GitHub Release creation
- Generated release notes

---

## Input

Example version:

v1.0.0

---

## Release Flow

Checkout repository  
Create Git tag  
Push tag  
Create GitHub Release  
Generate release notes

---

## Production Notes

- Use semantic versioning
- Protect release branches
- Avoid overwriting existing tags
- Attach build artifacts when needed
- Review release notes before publishing