# Ansible Automation Overview

Ansible automates provisioning, patching, deployment, and K3s setup across Linux and Windows nodes.

---

## Included Playbooks
- update_systems.yml – OS updates + reboots  
- deploy_web.yml – nginx deployment  
- setup_k3s.yml – K3s installation  
- hardening.yml – system hardening  

---

## Execution Steps
1. Update inventory file  
2. Run playbook  
3. Validate output  
4. Logs stored in 08_logs-and-monitoring  

---

## Transport Methods
- SSH (Linux)
- WinRM (Windows Server)

---

## Verification
- Curl/HTTP checks  
- kubeconfig checks  
- Service status validation
