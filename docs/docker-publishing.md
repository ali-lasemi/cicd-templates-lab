# Docker Registry Publishing Workflow

This document describes a reusable workflow for building and publishing Docker images.

---

## Purpose

The workflow automates:

- Docker image build
- Image tagging
- Registry authentication
- Image publishing

---

## Supported Registries

Examples:

- Docker Hub
- GitHub Container Registry (GHCR)
- GitLab Registry
- Private Registries

---

## Required Secrets

- REGISTRY_HOST
- REGISTRY_USERNAME
- REGISTRY_PASSWORD
- IMAGE_NAME

---

## Publishing Flow

Checkout Source Code
↓
Build Docker Image
↓
Tag Image
↓
Authenticate Registry
↓
Push Image
↓
Publish Version

---

## Generated Tags

Examples:

latest

and

github sha

Example:

my-app:latest

my-app:a4d9e12

---

## Production Notes

- Never store credentials in repository files
- Use immutable image tags
- Keep latest for convenience only
- Scan images before deployment
- Apply image retention policies