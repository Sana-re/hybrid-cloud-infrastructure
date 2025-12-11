# Proxmox VE Setup Overview

This document describes the Proxmox VE private cloud configuration used in the hybrid cloud environment.

---

## Host Configuration
- Proxmox VE installed on bare metal
- Local storage: ZFS or ext4
- CPU/RAM sized for multiple VMs
- SSH enabled for management

---

## Network Bridges
### vmbr0 (External)
Used for internet access and OS updates.

### vmbr1 (Internal)
Internal lab network (10.0.10.0/24) hosting:
- Windows Server
- Linux servers
- Ansible control node
- K3s Kubernetes nodes

---

## VM Templates
### Windows Server Template
- Sysprep
- Enabled WinRM for Ansible
- Baseline configuration

### Linux Template
- Cloud-init enabled
- SSH keys preloaded
- Hardened baseline

---

## Snapshots & Backups
Snapshots are taken before:
- OS updates  
- Playbook runs  
- K3s deployment  
- Major changes  

OCI backups provide off-site redundancy.
