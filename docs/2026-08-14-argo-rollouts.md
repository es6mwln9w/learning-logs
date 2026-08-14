# Argo Rollouts Notes

- Blue-green strategy works well for stateless services.
- Canary with traffic split requires an ingress controller (e.g., nginx or istio).
- `rollout restart` is handy for picking up new secrets.
- Remember to set `strategy.canary.steps` for progressive analysis.
- Dashboard: `kubectl argo rollouts dashboard` (port 3100).