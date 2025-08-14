# Lab 5: Finding Your System Information

## Objective
Learn how to find information about your current user, groups, and system environment.

---

## Steps

1. **Find out who you are currently logged in as**
   ```bash
   whoami
Example output:

nginx
Copy
Edit
ahmed
Display your user ID and group memberships

bash
Copy
Edit
id
Example output:

ini
Copy
Edit
uid=1000(ahmed) gid=1000(ahmed) groups=1000(ahmed),27(sudo),4(adm)
Show your current working directory

bash
Copy
Edit
pwd
Example output:

arduino
Copy
Edit
/home/ahmed
Display the contents of your .bashrc file (if it exists)

bash
Copy
Edit
cat ~/.bashrc
(This file contains shell configuration and aliases.)

List all hidden files in your home directory

bash
Copy
Edit
ls -la ~
Example output:

yaml
Copy
Edit
drwxr-xr-x 18 ahmed ahmed 4096 Aug 14 19:40 .
drwxr-xr-x  3 root  root  4096 Aug  5 09:12 ..
-rw-------  1 ahmed ahmed  675 Aug  7  .bash_history
-rw-r--r--  1 ahmed ahmed 3771 Aug  5  .bashrc
...

