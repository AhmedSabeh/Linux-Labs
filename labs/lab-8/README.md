# Lab 8: Package Management

## Objective
Learn how to update package lists, search for packages, install them, and verify installation.

---

## Steps

1. **Update your package list**  
   *(Debian/Ubuntu-based systems)*  
   ```bash
   sudo apt update
(RHEL/Fedora-based systems)

bash
Copy
Edit
sudo dnf check-update
Search for a package called tree in the package manager

bash
Copy
Edit
apt search tree
or

bash
Copy
Edit
dnf search tree
Install the tree package

bash
Copy
Edit
sudo apt install tree -y
or

bash
Copy
Edit
sudo dnf install tree -y
Use the tree command to display your directory structure

bash
Copy
Edit
tree ~/my_projects
Example output:

nginx
Copy
Edit
my_projects
├── backup
├── documents
│   ├── intro.txt
│   └── readme.txt
└── scripts
Check if the tree package is installed

bash
Copy
Edit
tree --version
Example output:

yaml
Copy
Edit
tree v1.8.0 (c) 1996 - 2018 by Steve Baker
