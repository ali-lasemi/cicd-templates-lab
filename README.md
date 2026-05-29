# CI/CD Templates Lab

Reusable CI/CD templates for Node.js, Nuxt, Docker and Android applications using GitHub Actions and GitLab CI.

---

# Overview

This repository contains production-oriented CI/CD templates and deployment workflows designed to accelerate software delivery.

The goal is to provide reusable pipeline patterns that are:

- Automated
- Reliable
- Reproducible
- Production-ready

---

# Supported Technologies

## GitHub Actions

- Node.js
- Nuxt 3
- Docker
- Android

## GitLab CI

- Node.js
- Nuxt 3
- Docker
- Android

---

# Features

- Reusable pipeline templates
- Build automation
- Artifact management
- Deployment workflows
- Rollback patterns
- Environment management
- Release automation

---

# Repository Structure

```txt
docs/
templates/
scripts/
.github/workflows/
```

---

# Pipeline Lifecycle

```txt
Code
  │
  ▼
Build
  │
  ▼
Test
  │
  ▼
Package
  │
  ▼
Deploy
  │
  ▼
Healthcheck
  │
  ▼
Rollback
```

---

# Roadmap

- Multi-environment deployments
- Kubernetes deployment workflows
- Blue/green deployments
- Canary release examples
- Infrastructure pipelines
- Security scanning integration

---

# Philosophy

```txt
Deployments should be boring.
Automation should be reliable.
Failures should be recoverable.
```

---

# License

MIT License