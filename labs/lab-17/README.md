# Lab 17: Network File Transfer.

## Task 17.1: Use wget to download a sample file
-  Navigate to your home directory
```
cd ~
```
-  Download a sample text file
```
wget https://www.w3.org/TR/PNG/iso_8859-1.txt
```

## Task 17.2: Use curl to fetch only headers of a website
```
curl -I https://www.google.com
```
-  -I means fetch headers only.

-  You’ll see details like HTTP status, server type, and date.

## Task 17.3: Create a text file and move it between directories
-  Create a file
```
echo "This is my test file" > myfile.txt
```
-  Create a directory to move it to
```
mkdir myfolder
```
-  Move the file into the folder
```
mv myfile.txt myfolder/
```
-  Verify
```
ls myfolder
```

## Task 17.4: Check file size before and after operations
-  Before moving (original file size)
```
ls -lh myfile.txt   # (Run this before moving in step above)
```
-  After moving (inside folder)
```
ls -lh myfolder/myfile.txt
```
```
ls -lh shows human-readable file sizes (KB, MB).
```
