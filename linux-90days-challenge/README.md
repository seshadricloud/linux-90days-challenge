# 🐧 90-Day Linux Challenge

This repository documents my **90-day journey of mastering Linux for DevOps & Cloud**.  
It includes **hands-on projects, scripts, and automation tasks** that cover real-world scenarios.

---

## 📅 Modules & Projects

### ✅ Module 1–3: Basics (OS, Architecture, Filesystem)
- [Linux Basics Guide](Module-1-3_Basics/Linux_Basics_Guide.pdf)
- Explored kernel version, init system, FHS.

### ✅ Module 4–5: Users & Permissions
- [User Management Script](Module-4-5_Users_Permissions/user_mgmt.sh)  
- Automated creation of users, groups, and secure directories.

### ✅ Module 6–7: Processes & Package Management
- [System Health Monitoring Script](Module-6-7_Process_Packages/system_monitor.sh)  
- Runs via cron, logs CPU/memory usage, checks critical services.

### ✅ Module 8–9: Networking & Shell Scripting
- [Network Troubleshooter](Module-8-9_Networking_Scripting/net_troubleshooter.sh)  
- Pings servers, checks open ports, logs connectivity results.

### ✅ Module 10–11: Disks & LVM
- [Automated Disk Setup Script](Module-10-11_Disks_LVM/disk_setup.sh)  
- Creates partitions, mounts them, updates `/etc/fstab`.

### ✅ Module 12–13: Security & Logs
- [Security Hardening Script](Module-12-13_Security_Logs/security_hardening.sh)  
- Configured sudo, firewall, log alerts for failed SSH logins.

### ✅ Module 14–15: Performance & Cloud
- [Deploy Web App on Cloud VM](Module-14-15_Cloud_Containers/deploy_app.sh)  
- Deployed Nginx app on AWS EC2 using Docker, monitored performance.

---

## ⚡ Skills Gained
- Linux administration (users, processes, networking, services).
- Bash scripting & automation.
- System monitoring & troubleshooting.
- Security hardening & firewall setup.
- Cloud (AWS EC2), Docker, Terraform basics.

---

## 🚀 How to Use
Clone the repo and try out individual scripts:

```bash
git clone https://github.com/<your-username>/linux-90days-challenge.git
cd linux-90days-challenge/Module-4-5_Users_Permissions
bash user_mgmt.sh
