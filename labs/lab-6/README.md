# Lab 6: Process Management

## Objective
Learn how to view running processes, identify them by Process ID (PID), and manage them.

---

## Steps

1. **Display all currently running processes**
   ```bash
   ps aux
Example output (partial):

sql
Copy
Edit
USER       PID  %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root         1  0.0  0.1 225276  1124 ?        Ss   Aug14   0:05 /sbin/init
ahmed     1503  0.0  0.3  95432  3240 pts/0    Ss   19:45   0:00 bash
Open a new terminal OR run a long-running command (example: sleep for 300 seconds)

bash
Copy
Edit
sleep 300 &
Output example:

csharp
Copy
Edit
[1] 2156
Here 2156 is the PID.

Find the process ID (PID) of your sleep command

If you didn’t note it from the previous step:

bash
Copy
Edit
ps aux | grep sleep
Example:

yaml
Copy
Edit
ahmed     2156  0.0  0.0   2604   548 pts/0    S    19:46   0:00 sleep 300
Kill the sleep process using its PID

bash
Copy
Edit
kill 2156
If it doesn’t stop, use:

bash
Copy
Edit
kill -9 2156
Monitor system processes in real-time

Using top:

bash
Copy
Edit
top
Press q to quit.

Or, if htop is installed (more user-friendly):

bash
Copy
Edit
htop
