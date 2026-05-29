# GitHub Actions Templates

Reusable GitHub Actions workflows for common application types.

---

## Included Templates

- Node.js CI
- Nuxt CI/CD
- Android CI
- Docker build

---

## Usage

Copy a template into your project:

```bash
mkdir -p .github/workflows
cp templates/github-actions/node.yml .github/workflows/node.yml
```

---

## Notes

- Update Node.js versions based on project needs
- Configure secrets for deployment workflows
- Add environment protection rules for production deployments