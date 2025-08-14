# Lab 1: Basic Navigation

## Objective
Learn how to navigate the Linux filesystem, check your current location, and move between directories.

---

## Steps

1. **Navigate to your home directory**  
   ```bash
   cd ~
This command moves you to your home directory.

Show your current directory location

pwd


Expected output (example):

/home/username


List all files and directories in your current location

ls -la


This shows both hidden and visible files.

Change to the root directory (/)

cd /


List the contents of the root directory

ls -l


Example output:

drwxr-xr-x   2 root root  4096 Aug  5  bin
drwxr-xr-x   4 root root  4096 Aug  5  boot
...


Return to your home directory

cd ~

