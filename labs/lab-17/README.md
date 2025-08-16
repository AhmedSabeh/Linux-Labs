🔹 Lab 17: Network File Transfer
Task 17.1: Use wget to download a sample file from the internet

Move into your lab directory:

cd ~/linux-labs/labs/lab-17
mkdir network-transfer && cd network-transfer


Download a sample file (example: small text file from GNU project):

wget http://ftp.gnu.org/gnu/wget/wget-1.21.1.tar.gz


Verify the download:

ls -lh

Task 17.2: Use curl to fetch just the headers of a website

Run curl with the -I option (capital i):

curl -I https://www.example.com


✅ This shows only the HTTP headers (status, server, content type, etc.).

Task 17.3: Create a simple text file and practice moving it between directories

Create a text file:

echo "This is a test file for Lab 17" > myfile.txt


Check it exists:

ls -l


Make a new folder and move the file:

mkdir moved-files
mv myfile.txt moved-files/


Verify:

ls moved-files/

Task 17.4: Check the file size before and after operations

Use ls -lh for human-readable file sizes:

ls -lh moved-files/myfile.txt


Or use du:

du -sh moved-files/myfile.txt


Compare before and after moving (file size won’t change when moving, but good practice to check).
