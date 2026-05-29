# Deployment Patterns

Common CI/CD deployment patterns for production systems.

---

## Build → Artifact → Deploy

```txt
Source Code
   │
   ▼
Build
   │
   ▼
Artifact
   │
   ▼
Deploy
   │
   ▼
Healthcheck
```

---

## Recommended Practices

- Build once, deploy many times
- Store artifacts
- Use environment-specific variables
- Add healthchecks
- Add rollback strategy
- Keep production secrets out of repository