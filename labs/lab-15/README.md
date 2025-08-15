# Lab 15: Creating a Simple Script.

1️⃣ Create the script file
```
nano system_info.sh
```
2️⃣ Add the script content
```
#!/bin/bash
# system_info.sh - Display system information

echo "===== System Information ====="
echo "Date and Time: $(date)"
echo "Username: $USER"
echo "Current Directory: $(pwd)"
echo "Available Disk Space:"
df -h --total | grep total
```
3️⃣ Save and exit

-  Press CTRL+O → Enter → CTRL+X.

4️⃣ Make the script executable
```
chmod +x system_info.sh
```
5️⃣ Run the script
```
./system_info.sh
```
You should see something like:
```
===== System Information =====
Date and Time: Thu Aug 14 19:12:45 EET 2025
Username: student
Current Directory: /home/student
Available Disk Space:
total      100G   45G   55G  45% -
```
