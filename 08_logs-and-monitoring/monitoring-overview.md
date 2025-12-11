# Logs & Monitoring Strategy

---

## Ansible Logs
Stored after each playbook run:
- Success/failure
- Unreachable hosts
- Task changes

---

## System Logs
Linux:
- syslog
- journalctl
- dmesg

Windows:
- Event Viewer
- WinRM logs

---

## Health Monitoring
- Uptime checks
- Service health checks
- Kubernetes pod monitoring
