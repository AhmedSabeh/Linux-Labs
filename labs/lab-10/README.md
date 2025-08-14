# Lab 10: Disk Usage Analysis

## Objective
Learn how to check disk space usage, identify large directories, and inspect file sizes.

---

## Steps

1. **Check the disk space usage of all mounted filesystems**
   ```bash
   df -h
Example output:

bash
Copy
Edit
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        50G   20G   28G  42% /
tmpfs           1.9G  2.0M  1.9G   1% /run
Find the size of your home directory

bash
Copy
Edit
du -sh ~
Example output:

arduino
Copy
Edit
3.2G    /home/ahmed
Identify the largest directories in your home folder

bash
Copy
Edit
du -sh ~/* | sort -hr | head -n 10
Example output:

arduino
Copy
Edit
1.5G    /home/ahmed/Videos
1.0G    /home/ahmed/Documents
500M    /home/ahmed/Downloads
Check how much space specific files are using

bash
Copy
Edit
ls -lh ~/my_projects/documents/readme.txt
Example output:

css
Copy
Edit
-rw-r--r-- 1 ahmed ahmed 1.2K Aug 14 20:30 readme.txt
Display information about your storage devices

bash
Copy
Edit
lsblk
Example output:

pgsql
Copy
Edit
NAME   MAJ:MIN RM  SIZE RO TYPE MOUNTPOINTS
sda      8:0    0   50G  0 disk
└─sda1   8:1    0   50G  0 part /
sr0     11:0    1 1024M  0 rom
Notes
df -h → Disk Free in human-readable format.

du -sh → Disk Usage summary for a directory.

lsblk → Lists block devices like HDDs, SSDs, and USB drives.

Sorting with sort -hr shows the largest directories first.
