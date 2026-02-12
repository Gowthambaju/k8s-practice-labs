# 🚀 Kubernetes Practice Labs

This repository contains my structured Kubernetes learning journey.

I am building production-level Kubernetes knowledge with hands-on labs, focusing on SRE-level understanding rather than surface-level theory.

---

## 📅 Learning Plan

### ✅ Day 1 – Pod Basics
- Created first Pod YAML
- Deployed nginx pod
- Used `kubectl get`, `describe`, `delete`
- Understood:
  - Pod structure
  - YAML anatomy
  - Scheduler basics

File:
- `pod-nginx.yaml`

---

### ✅ Day 2 – Pod Lifecycle & Status (Deep Dive)

Covered:

- Pod Phases:
  - Pending
  - Running
  - Succeeded
  - Failed
  - Unknown

- Container States:
  - Waiting
  - Running
  - Terminated

- CrashLoopBackOff
- ImagePullBackOff
- RestartPolicy
- Exit Codes (0, 1, 137, 143)
- OOMKilled
- Requests vs Limits
- CPU Throttling vs Memory Kill
- Graceful Termination (SIGTERM → SIGKILL)
- ContainerCreating & Terminating states
- Reading Events using:
  ```
  kubectl describe pod <pod>
  ```

Key Learning:
- Scheduler uses requests
- Kubelet enforces limits
- Linux handles OOM
- CPU is throttled, Memory is killed

---

## 🛠 Commands Practiced

```bash
kubectl get pods
kubectl get pods -A
kubectl describe pod <pod>
kubectl delete pod <pod>
kubectl get pods -w
```

---

## 🎯 Goal

Become production-ready Kubernetes Engineer / SRE by:
- Understanding internals
- Debugging real scenarios
- Practicing daily
- Documenting progress publicly

---

More labs coming soon.
