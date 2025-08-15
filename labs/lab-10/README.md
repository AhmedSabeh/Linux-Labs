# Lab 10: Disk Usage Analysis

## Objective
Learn how to check disk space usage, identify large directories, and inspect file sizes.

---

## Steps

1. **Check the disk space usage of all mounted filesystems**
   ```
   df -h
   ```
-   Output:

<img width="747" height="205" alt="Screenshot (213)" src="https://github.com/user-attachments/assets/5aeb0911-2e76-4db9-aad6-049c0212f8cc" />

2. **Find the size of your home directory**
```
du -sh ~
```
-   Output:

<img width="907" height="70" alt="Screenshot (214)" src="https://github.com/user-attachments/assets/20b5dcb0-e85c-41c8-98ca-2b771a9151d4" />

3. **Identify the largest directories in your home folder**
```
du -sh ~/* | sort -hr | head -n 10
```
-   Output:

<img width="913" height="250" alt="Screenshot (215)" src="https://github.com/user-attachments/assets/4b2b9b9e-3e7a-42fa-8fa9-489c9973f5da" />

4. **Check how much space specific files are using**
```
ls -lh ~/my_projects/documents/readme.txt
```
-   Output:

<img width="910" height="104" alt="Screenshot (216)" src="https://github.com/user-attachments/assets/81d24fc5-ff08-4ea7-a0bc-208b7c0bab10" />

5. **Display information about your storage devices**
```
lsblK
```
-   Output:

<img width="908" height="474" alt="Screenshot (217)" src="https://github.com/user-attachments/assets/a09f9390-b37d-411a-8dfd-fa276b50e25e" />

-   Notes

      *   df -h → Disk Free in human-readable format.

      *   du -sh → Disk Usage summary for a directory.

      *   lsblk → Lists block devices like HDDs, SSDs, and USB drives.

      *   Sorting with sort -hr shows the largest directories first.
