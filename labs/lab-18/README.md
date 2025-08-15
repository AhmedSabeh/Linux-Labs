Lab 18: Log Analysis:

1. View the last 20 lines of system logs

Most Linux systems store logs in /var/log/ — for system logs, it’s often syslog (Debian/Ubuntu) or messages (RHEL/Amazon Linux).

sudo tail -n 20 /var/log/syslog      # Debian/Ubuntu  
sudo tail -n 20 /var/log/messages    # RHEL/CentOS/Amazon Linux  

2. Search for specific error messages

Use grep to find keywords like "error" in the logs:

sudo grep -i "error" /var/log/syslog


-i makes the search case-insensitive.

3. Display logs from today only

We can filter by date — for example, if today is Aug 14:

sudo grep "$(date '+%b %e')" /var/log/syslog


This dynamically matches month and day.

4. Follow logs in real-time for 30 seconds

You can use tail -f and stop it after 30 seconds:

sudo timeout 30 tail -f /var/log/syslog


or manually stop with Ctrl + C.
