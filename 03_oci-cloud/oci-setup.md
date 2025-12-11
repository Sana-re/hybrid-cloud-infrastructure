# Oracle Cloud Infrastructure (OCI) Setup

This folder documents the public cloud portion of the hybrid architecture.

---

## VCN & Subnet
- VCN CIDR: 10.0.20.0/24
- Public subnet with internet gateway
- Route tables allowing outbound traffic

---

## Compute Instance (OCI Web Server)
- Ubuntu 22.04 LTS
- SSH key authentication
- Fail2ban and UFW enabled
- nginx installed for testing

---

## Security Lists
Inbound:
- SSH (22)
- HTTP (80)
- HTTPS (443)

Outbound:
- All traffic allowed

---

## Backup Policy
- Daily automatic backups
- Manual backups before deployments
