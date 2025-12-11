# Network Topology Overview

This project uses a segmented private network aligned with enterprise networking practices.

---

## Bridges
### vmbr0
External NAT network

### vmbr1
Internal network 10.0.10.0/24 for all virtual machines

---

## VM IP Layout
- Ansible Control Node  
- Windows Server  
- Linux Web Server  
- K3s Nodes  

---

## Routing
- NAT via vmbr0
- Internal routing through Proxmox host
- Firewall rules enforce segmentation
