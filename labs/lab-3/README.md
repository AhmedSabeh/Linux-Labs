# Lab 3: Working with File Content

## Objective
Learn how to create files, edit them with a text editor, and view their contents in different ways.

---

## Steps

1. **Navigate to your `documents` folder**
   ```
   cd ~/my_projects/documents
   ```
2. **Create a file called `intro.txt` using touch**
```
touch intro.txt
```
3. **Edit the file using nano and add 3 lines of text about yourself**
```
nano intro.txt
```
-   Output:
```
My name is Ahmed Sabeh.
I am learning Linux for DevOps.
I enjoy building cloud projects.
```

<img width="739" height="483" alt="Screenshot (191)" src="https://github.com/user-attachments/assets/0a62f590-070f-4fd1-aee5-1880e2099203" />

4. **Save and exit nano: Press CTRL + O, then Enter to save, and CTRL + X to exit.**

5. **Display the entire content of the file using cat**
```
cat intro.txt
```
-   Output:
  
<img width="735" height="482" alt="Screenshot (192)" src="https://github.com/user-attachments/assets/7fb174f5-cd08-43f2-b15f-2cd648a8318f" />

6. **Display the content page by page using less**
```
less intro.txt
```

<img width="739" height="475" alt="Screenshot (193)" src="https://github.com/user-attachments/assets/489073ea-815f-494f-bc66-890998a0dcc5" />

-   Use the space bar to go to the next page.

-   Press q to quit.
