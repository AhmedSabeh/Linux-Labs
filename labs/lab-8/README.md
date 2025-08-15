# Lab 8: Package Management

## Objective
Learn how to update package lists, search for packages, install them, and verify installation.

---

## Steps

1. **Update your package list**  
   *(Debian/Ubuntu-based systems)*  
   ```
   sudo apt update
   ```
-  (RHEL/Fedora-based systems)
```
sudo dnf check-update
```
2. **Search for a package called tree in the package manager**
```
apt search tree
```
or
```
dnf search tree
```
3. **Install the tree package**
```
sudo apt install tree -y
```
or
```
sudo dnf install tree -y
```
4. **Use the tree command to display your directory structure**
```
tree ~/my_projects
```
-  Output:

<img width="924" height="475" alt="Screenshot (210)" src="https://github.com/user-attachments/assets/4a5b87ce-0d47-4799-a4c8-4a80ee90b667" />

5. **Check if the tree package is installed**
```
tree --version
```
-  Output:

<img width="923" height="477" alt="Screenshot (209)" src="https://github.com/user-attachments/assets/71e6fcdf-2df5-4198-a5b3-fc9e41c42c9a" />
