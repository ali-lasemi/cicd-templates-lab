# GitLab CI Templates

Reusable GitLab CI pipeline templates for Node.js, Nuxt and Android projects.

---

## Included Templates

- Node.js build/test pipeline
- Nuxt build pipeline with artifacts
- Android build pipeline

---

## Usage

Copy a template into your project:

```bash
cp templates/gitlab-ci/nuxt.gitlab-ci.yml .gitlab-ci.yml
```

---

## Notes

- Configure GitLab runners before using pipelines
- Use CI/CD variables for secrets
- Store build artifacts with short expiration times