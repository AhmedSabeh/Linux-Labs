# Lab 4: File Permissions Practice

## Objective
Learn how to view, change, and verify file permissions in Linux.

---

## Steps

1. **Create a file called `secret.txt` in your home directory**
   ```
   cd ~
   touch secret.txt
   ```
2. **Check the current permissions of the file**
```
ls -l secret.txt
```
-   Output:

<img width="734" height="480" alt="Screenshot (194)" src="https://github.com/user-attachments/assets/de2a2f3c-4239-43ba-b33e-b9071204c55f" />

      *   rw- → owner can read and write

      *   r-- → group can only read

      *   r-- → others can only read

3. **Change the permissions so only you can read and write the file**
```
chmod 600 secret.txt
ls -l secret.txt
```
- Output:

<img width="736" height="135" alt="Screenshot (198)" src="https://github.com/user-attachments/assets/734b8e40-771d-487b-a0e0-eeddee001669" />

4. **Create a script file called `hello.sh`**
```
touch hello.sh
echo "echo Hello, World!" > hello.sh
```
5. **Make the script executable for everyone**
```
chmod a+x hello.sh
ls -l hello.sh
```
6. **Run the script**
```
./hello.sh
```
-   Output:
```
Hello, World!
```

<img width="734" height="480" alt="Screenshot (196)" src="https://github.com/user-attachments/assets/5f22e449-308d-4560-ad97-b6c7a0f85845" />
