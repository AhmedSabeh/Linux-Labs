here’s Lab 13: User and Group Management.

1. Display information about your user account
id


This shows:

UID (user ID)

GID (group ID)

Groups you belong to

2. List all users on the system
cut -d: -f1 /etc/passwd


cut -d: -f1 extracts only the username from /etc/passwd.

3. Show which groups you belong to
groups


or

id -nG


Both will list the group names.

4. Check the contents of the /etc/passwd file (first 10 lines)
head -n 10 /etc/passwd


The /etc/passwd file contains user account information in this format:

username:password:UID:GID:comment:home_directory:shell


(Note: The password field usually contains an x and is stored in /etc/shadow)

5. Display your shell history
history


This shows a numbered list of the commands you’ve run.
