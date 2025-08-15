# Lab 5: Finding Your System Information

## Objective
Learn how to find information about your current user, groups, and system environment.

---

## Steps

1. **Find out who you are currently logged in as**
   ```
   whoami
   ```
-   Output:

<img width="736" height="129" alt="Screenshot (199)" src="https://github.com/user-attachments/assets/a4cb4c9a-8bd3-4cae-8155-6c1cc131600a" />

2. **Display your user ID and group memberships**
```
id
```
-   Output:

<img width="738" height="163" alt="Screenshot (200)" src="https://github.com/user-attachments/assets/f7b35167-54fd-4692-b0ed-7d44b9b7519c" />

3. **Show your current working directory**
```
pwd
```
-   Output:

<img width="740" height="110" alt="Screenshot (201)" src="https://github.com/user-attachments/assets/d6b64c03-210a-486d-b0c8-94e9d47b56a5" />

4- **Display the contents of your .bashrc file (if it exists)**
```
cat ~/.bashrc
```
(This file contains shell configuration and aliases.)

5- **List all hidden files in your home directory**
```
ls -la ~
```
-   Output:

<img width="736" height="319" alt="Screenshot (202)" src="https://github.com/user-attachments/assets/d8cab985-9a9e-490b-a6cd-7fa3ea06884c" />
