# Hybrid Cloud Infrastructure Project  
Proxmox VE • Oracle Cloud Infrastructure (OCI) • Ansible • Linux • K3s Kubernetes • Enterprise Networking

This project demonstrates a full hybrid cloud environment built using **Proxmox VE (private cloud)** and **Oracle Cloud Infrastructure (public cloud)**, automated through **Ansible** and extended with **K3s Kubernetes** for lightweight container orchestration.  
It includes full documentation, diagrams, automation scripts, VM configurations, networking layouts, and operational procedures.

---

## 📌 Project Overview

This hybrid cloud solution integrates:

- **Proxmox VE Private Cloud**  
  Virtualization cluster for internal workloads, snapshots, backups, and LXC containers.

- **Oracle Cloud Infrastructure (OCI)**  
  Public cloud compute instance hosting production web applications.

- **Ansible Automation**  
  Automated provisioning, updates, patches, web server deployments, and K3s installation.

- **K3s Kubernetes Cluster**  
  Lightweight container orchestration for internal services and scalable workloads.

- **Enterprise Network Design**  
  Segmented networks using Proxmox bridges (vmbr0 external, vmbr1 internal), VLANs, firewall rules, NAT, and routing.

This architecture supports **high availability**, **low cost**, and **enterprise-grade flexibility** for training and real-world IT operations.

---

## 📁 Repository Structure

