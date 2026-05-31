# Blue-Green Deployment

This document describes a reusable blue-green deployment pattern.

---

## Purpose

Blue-green deployments reduce deployment risk by maintaining two production-like environments.

One environment serves live traffic while the other receives the new release.

---

## Environments

- Blue
- Green

At any time, only one color should receive production traffic.

---

## Deployment Flow

Deploy to inactive color  
Run healthcheck  
Validate application behavior  
Switch traffic  
Keep previous color available for rollback

---

## Benefits

- Reduced downtime
- Safer production releases
- Faster rollback
- Better release confidence

---

## Production Notes

- Use reverse proxy routing for traffic switching
- Keep blue and green environments isolated
- Validate health before switching traffic
- Automate rollback when healthcheck fails