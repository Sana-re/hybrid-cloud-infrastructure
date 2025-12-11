# K3s Kubernetes Cluster Overview

A lightweight Kubernetes environment deployed inside the Proxmox internal network.

---

## Architecture
- 1 K3s control node
- 1–2 worker nodes
- Internal-only cluster

---

## Deployment Workflow
1. Provision VMs via Proxmox
2. Install K3s via Ansible
3. Retrieve kubeconfig
4. Join worker nodes

---

## Verification Commands
- kubectl get nodes
- kubectl get pods -A

---

## Use Cases
- Microservices
- Internal services
- Automation testing
