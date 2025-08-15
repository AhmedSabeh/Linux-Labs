Lab 14: System Monitoring:

1️⃣ Check current memory usage
free -h


-h → human-readable format (MB/GB).

Shows total, used, and free memory (RAM + swap).

2️⃣ Display CPU information
lscpu


Displays detailed CPU architecture, cores, threads, speed, etc.

3️⃣ Monitor system load average
uptime


or

cat /proc/loadavg


Load average shows system load for the last 1, 5, and 15 minutes.

4️⃣ Check available disk space on all mounted filesystems
df -h


-h → human-readable sizes (MB/GB).

Shows usage per mount point.

5️⃣ Display running processes sorted by memory usage
ps aux --sort=-%mem | head -n 15


--sort=-%mem → sorts processes by memory usage (highest first).

head -n 15 → limits output to the top 15 processes.
