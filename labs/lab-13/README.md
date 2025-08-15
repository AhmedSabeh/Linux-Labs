# Lab 13: User and Group Management.

**1. Display information about your user account**
```
id
```
This shows:

<img width="1268" height="115" alt="Screenshot (231)" src="https://github.com/user-attachments/assets/8d70ed87-a570-492b-bf46-e86bd3afa3a0" />

-  UID (user ID)

-  GID (group ID)

-  Groups you belong to
---
**2. List all users on the system**
```
cut -d: -f1 /etc/passwd
```
-  ``` cut -d: -f1 ``` extracts only the username from /etc/passwd.

<img width="1268" height="146" alt="Screenshot (226)" src="https://github.com/user-attachments/assets/d8e47da8-d357-4d76-9fd2-5b296c57de13" />

---

**3. Show which groups you belong to**
```
groups
```
or
```
id -nG
```
Both will list the group names.

<img width="1262" height="111" alt="Screenshot (228)" src="https://github.com/user-attachments/assets/7ac51896-4131-4086-b80d-2fa2fb55a467" />

---
**4. Check the contents of the /etc/passwd file (first 10 lines)**
```
head -n 10 /etc/passwd

```
The /etc/passwd file contains user account information in this format:

<img width="1263" height="232" alt="Screenshot (229)" src="https://github.com/user-attachments/assets/d2a36c86-bf95-4ed5-a804-986e4e3fa1df" />

(Note: The password field usually contains an x and is stored in /etc/shadow)
---
**5. Display your shell history**
```
history
```
This shows a numbered list of the commands you’ve run.

<img width="1265" height="498" alt="Screenshot (230)" src="https://github.com/user-attachments/assets/2285a31c-a1bb-44cf-8536-1c5dc5fde5e5" />

