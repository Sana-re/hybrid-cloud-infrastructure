# Backup & Continuity Workflow

A combined Proxmox + OCI backup strategy ensures availability and quick recovery.

---

## Proxmox
- Local snapshots
- Snapshot before updates
- Versioned rollback

---

## OCI
- Automated daily backups
- On-demand backups before changes

---

## Disaster Recovery Steps
1. Restore Proxmox snapshot  
2. Redeploy services via Ansible  
3. Rebuild K3s workloads  
4. Validate system state  
