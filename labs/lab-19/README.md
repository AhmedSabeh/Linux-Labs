# Lab 19: Environment Customization:

### Task 19.1: Check your current environment variables

-  Environment variables define how your shell and programs behave.
```
printenv
```
-  or
```
env
```
<img width="1084" height="99" alt="Screenshot (260)" src="https://github.com/user-attachments/assets/2bb33f5c-96ba-43b9-bbb6-b5b5c995cfd4" />

### Task 19.2: Display your PATH variable

-  The PATH variable tells Linux where to look for executables when you type a command.
```
echo $PATH
```
-  You should see directories separated by : (like /usr/local/bin:/usr/bin:/bin).

<img width="1081" height="78" alt="Screenshot (261)" src="https://github.com/user-attachments/assets/04a0fd27-47c4-4ba6-b1cf-f13478cfe4a5" />

### Task 19.3: Add an alias to your .bashrc file

-  Aliases save time by shortening long commands.

-  Open .bashrc in nano (or your preferred editor):
```
nano ~/.bashrc
```
-  Add a line at the bottom. Example:
```
alias ll='ls -lah'
```

-  Save & exit (CTRL+O, ENTER, CTRL+X).

-  Reload .bashrc:
```
source ~/.bashrc
```

-  Test your alias:
```
ll
```

### Task 19.4: Create a custom prompt 

-  The shell prompt is controlled by the PS1 variable. 
```
export PS1="student@devops:~$ "
```
<img width="905" height="79" alt="Screenshot (263)" src="https://github.com/user-attachments/assets/7fd58699-8fbd-4049-b77f-20f0936480d2" />

-  To make it permanent, add it to your ~/.bashrc.

### Task 19.5: Test your customizations

-  Run ll to test your alias.

-  Open a new terminal → see if your prompt and alias persist.
