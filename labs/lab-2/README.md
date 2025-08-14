# Lab 2: Creating Files and Directories

## Objective
Learn to create and organize directories and files in a structured way.

---

## Steps

1. **Create a directory called `my_projects`**
   ```bash
   mkdir ~/my_projects
Navigate into the my_projects directory

cd ~/my_projects


Create three subdirectories: documents, scripts, and backup

mkdir documents scripts backup


Create an empty file called readme.txt in the documents folder

touch documents/readme.txt


Show the tree structure you created

If tree is installed:

tree ~/my_projects


Example output:

my_projects
├── backup
├── documents
│   └── readme.txt
└── scripts


If tree is not installed, use:

ls -R ~/my_projects


Example output:

my_projects:
backup  documents  scripts

my_projects/backup:

my_projects/documents:
readme.txt

my_projects/scripts:
