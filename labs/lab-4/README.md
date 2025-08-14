# Lab 4: File Permissions Practice

## Objective
Learn how to view, change, and verify file permissions in Linux.

---

## Steps

1. **Create a file called `secret.txt` in your home directory**
   ```bash
   cd ~
   touch secret.txt
Check the current permissions of the file

bash
Copy
Edit
ls -l secret.txt
Example output:

css
Copy
Edit
-rw-r--r-- 1 ahmed ahmed 0 Aug 14 19:20 secret.txt
rw- → owner can read and write

r-- → group can only read

r-- → others can only read

Change the permissions so only you can read and write the file

bash
Copy
Edit
chmod 600 secret.txt
ls -l secret.txt
Example output:

diff
Copy
Edit
-rw------- 1 ahmed ahmed 0 Aug 14 19:20 secret.txt
Create a script file called hello.sh

bash
Copy
Edit
touch hello.sh
echo "echo Hello, World!" > hello.sh
Make the script executable for everyone

bash
Copy
Edit
chmod a+x hello.sh
ls -l hello.sh
Example output:

diff
Copy
Edit
-rwxr-xr-x 1 ahmed ahmed 24 Aug 14 19:25 hello.sh
Run the script

bash
Copy
Edit
./hello.sh
Output:

Copy
Edit
Hello, World!
