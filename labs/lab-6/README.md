# Lab 6: Process Management

## Objective
Learn how to view running processes, identify them by Process ID (PID), and manage them.

---

## Steps

1. **Display all currently running processes**
   ```
   ps aux
   ```
-   Output 

<img width="732" height="423" alt="Screenshot (203)" src="https://github.com/user-attachments/assets/901112be-8042-46c5-9338-d07af338ca42" />

2. **Open a new terminal OR run a long-running command (sleep for 60 seconds)**
```
sleep 60 &
```
-   Output:
```
[1] 191591
```
-   Here 191591 is the PID.

3. **Find the process ID (PID) of your sleep command**

If you didn’t note it from the previous step:
```
ps aux | grep sleep
```

4. **Kill the sleep process using its PID**
```
kill 191591
```

-   Ouput:

<img width="924" height="211" alt="Screenshot (206)" src="https://github.com/user-attachments/assets/627a072c-879a-4ccf-b4d5-859081ef5bf9" />
  
5. **Monitor system processes in real-time**

Using top:
```
top
```
-   Press q to quit.

-   Or, if htop is installed (more user-friendly):
```
htop
```
