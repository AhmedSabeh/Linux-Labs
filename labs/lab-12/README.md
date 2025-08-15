# Lab 12: Advanced File Operations
1️⃣ Create 5 text files in your projects directory 
```
mkdir -p ~/projects

# Create 5 text files
touch ~/projects/file1.txt ~/projects/file2.txt ~/projects/file3.txt ~/projects/file4.txt ~/projects/file5.txt
```
2️⃣ Find all .txt files in your home directory and subdirectories
```
find ~ -type f -name "*.txt"
```
- This will list .txt files under your home directory.

3️⃣ Create a compressed archive of your projects directory
```
tar -czvf projects.tar.gz ~/projects
```
- c → create archive

- z → compress with gzip

- v → verbose (show files)

- f → filename

4️⃣ Extract the archive to a new location
```
mkdir -p ~/projects_copy
tar -xzvf projects.tar.gz -C ~/projects_copy
```
- This creates a copy of the files in ~/projects_copy.

5️⃣ Compare the original and extracted directories
```
diff -r ~/projects ~/projects_copy
```
- If they’re the same, diff will show no output.
