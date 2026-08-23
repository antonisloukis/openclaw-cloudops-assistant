# Examples

## Example 1: Kubernetes Incident

### User Input
My Kubernetes pod keeps restarting.
Error:
CrashLoopBackOff


---

### OpenClaw Response

## Incident Summary

The application container is failing during startup and Kubernetes is restarting it.

## Possible Causes

- Application crash
- Missing environment variables
- Dependency unavailable
- Incorrect configuration


## Investigation Steps

Check logs:


kubectl logs <pod-name>

Inspect pod status:
kubectl describe pod <pod-name>

Recommended Fix
Review application startup errors and verify required configuration values.
Prevention
- Add health checks
- Improve logging
- Configure resource limits

Commit:

```text
Add usage examples
