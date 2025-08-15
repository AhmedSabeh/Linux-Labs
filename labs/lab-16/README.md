# Lab 16: File Backup

1️⃣ Create a backup directory in your home folder
```
mkdir ~/backup
```
-  This will create a folder called backup in your home directory.

2️⃣ Copy all files from your projects directory to the backup directory

```
cp -r ~/projects/* ~/backup/
```
-  -r means recursive (needed for folders).

-  This copies everything from ~/projects into ~/backup.

3️⃣ Create a compressed archive of your important files

compress the backup folder into a .tar.gz file:
```
tar -czvf ~/backup_$(date +%F).tar.gz ~/backup
```
-  -c → create

-  -z → compress with gzip

-  -v → verbose (show progress)

-  -f → filename for the archive

-  $(date +%F) → adds today’s date to the filename (e.g., backup_2025-08-14.tar.gz)

4️⃣ Practice restoring files from your backup

-  Restore the archive into a folder called restore_test:
```
mkdir ~/restore_test
tar -xzvf ~/backup_$(date +%F).tar.gz -C ~/restore_test
```
-  -x → extract

-  -z → decompress gzip

-  -C → specify the destination folder
