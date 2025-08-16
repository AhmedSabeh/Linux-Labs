# Lab 17: Network File Transfer
### Task 17.1: Use wget to download a sample file from the internet

-  Move into your lab directory:
```
cd ~/linux-labs/labs/lab-17
mkdir network-transfer && cd network-transfer
```
-  Download a sample file (example: small text file from GNU project):
```
wget http://ftp.gnu.org/gnu/wget/wget-1.21.1.tar.gz
```
-  Verify the download:
```
ls -lh
```
<img width="1074" height="335" alt="Screenshot (256)" src="https://github.com/user-attachments/assets/2d232813-17a1-41db-81fb-5ae8d14350e0" />

### Task 17.2: Use curl to fetch just the headers of a website
```
curl -I https://www.example.com
```
✅ This shows only the HTTP headers (status, server, content type, etc.).

<img width="1074" height="198" alt="Screenshot (256) 2" src="https://github.com/user-attachments/assets/350663b0-117c-41a9-9d7e-cee2cf82f47d" />

### Task 17.3: Create a simple text file and practice moving it between directories

-  Create a text file:
```
echo "This is a test file for Lab 17" > myfile.txt
```
-  Check it exists:
```
ls -l
```
-  Make a new folder and move the file:
```
mkdir moved-files
mv myfile.txt moved-files/
```
-  Verify:
```
ls moved-files/
```

<img width="1090" height="200" alt="Screenshot (257)" src="https://github.com/user-attachments/assets/e898ddaa-3034-4baa-b2e8-cd74414e6959" />

### Task 17.4: Check the file size before and after operations

```
ls -lh moved-files/myfile.txt
```

-  Or use du:
```
du -sh moved-files/myfile.txt
```

<img width="1071" height="142" alt="Screenshot (259)" src="https://github.com/user-attachments/assets/21afd2d9-4d54-470f-9239-da7ac097f222" />
