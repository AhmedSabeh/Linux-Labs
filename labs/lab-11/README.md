# Lab 11: Service Management

## Objective
Learn how to check the status of services, view logs, and see which services start automatically at boot.

---

## Steps

1. **Check the status of a system service**  
   Example: SSH service  
   ```bash
   sudo systemctl status ssh
Example output (shortened):

lua
Copy
Edit
● ssh.service - OpenBSD Secure Shell server
     Loaded: loaded (/lib/systemd/system/ssh.service; enabled)
     Active: active (running) since Tue 2025-08-12 14:03:20 EET; 3h 15min ago
View recent system logs

bash
Copy
Edit
sudo journalctl -n 20
(Shows the last 20 log entries.)

Look for any error messages in the logs

bash
Copy
Edit
sudo journalctl -p err -n 20
(Shows the last 20 log entries with error priority.)

Check which services are enabled to start at boot

bash
Copy
Edit
systemctl list-unit-files --type=service --state=enabled
Example output:

Copy
Edit
ssh.service                           enabled
cron.service                          enabled
network-manager.service               enabled
