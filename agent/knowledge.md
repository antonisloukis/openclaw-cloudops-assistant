# Cloud Operations Knowledge Base

This document defines the operational knowledge areas used by the OpenClaw Cloud Operations Assistant.

---

# AWS Troubleshooting

## EC2

Common problems:

- Instance unreachable
- SSH connection failures
- High CPU usage
- Disk space problems

Investigation:

- Check instance status
- Review CloudWatch metrics
- Verify security groups
- Inspect system logs


## IAM

Common problems:

- Access denied errors
- Missing permissions
- Incorrect policies

Investigation:

- Review IAM policies
- Check attached roles
- Validate least privilege access


## S3

Common problems:

- Access failures
- Public exposure
- Incorrect bucket policies

Investigation:

- Review bucket permissions
- Check Block Public Access settings
- Analyze access logs


---

# Kubernetes Troubleshooting

## CrashLoopBackOff

Possible causes:

- Application crash
- Missing configuration
- Invalid secrets
- Dependency failure


Investigation:

```bash
kubectl logs <pod>
kubectl describe pod <pod>
```

ImagePullBackOff

Possible causes:
- Invalid image name
- Registry authentication failure
- Missing image
Investigation:
```bash
kubectl describe pod <pod>
```
Terraform Troubleshooting

Common problems:
- Failed deployments
- State conflicts
- Infrastructure drift
Investigation:

```bash
terraform plan
terraform validate
```
Linux Operations

Common incidents:
- High memory usage
- Disk full
- Service failure
- Network issues
Investigation:

```bash
systemctl status service-name
df -h
free -m
```
SRE Principles

The assistant follows:
- Reliability first
- Safe investigation
- Observability
- Root cause analysis
- Continuous improvement

```bash
Commit message:
Add cloud operations knowledge bas
```

