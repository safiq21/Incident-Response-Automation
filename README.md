# ISP Incident Response Automation

This project is an **Ansible playbook** that automatically:

- Checks Nginx service status
- Restarts Nginx if down
- Captures CPU, memory, disk, and interface metrics
- Saves a timestamped incident report
- Sends the report via Gmail automatically

## Features

- Automated email notifications via Gmail App Password
- Works with multiple hosts (simulated or real)
- Logs saved in `reports/` folder
- Can be scheduled with cron or systemd timers

## Usage

1. Clone the repo
2. Configure `inventory.ini` with your hosts
3. Set your Gmail App Password in `incident.yml`
4. Run playbook manually:

```bash
ansible-playbook -i inventory.ini incident.yml --ask-become-pass




- Save + exit  

---

## **Step 5: Commit Your Files**

```bash
git add .
git commit -m "Initial commit: Incident Response Automation playbook with Gmail notifications"
