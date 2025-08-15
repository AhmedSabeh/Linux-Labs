Lab 19: Environment Customization:

1. Check your current environment variables
printenv


or

env


💡 This lists all environment variables currently set in your shell session.

2. Display your PATH variable
echo $PATH


This shows the directories your system searches when you run a command.

3. Add an alias to your .bashrc file

Let’s say you often run:

ls -lah


You can make it shorter by adding an alias:

nano ~/.bashrc


Add this line at the bottom:

alias ll='ls -lah'


Save and exit (CTRL+O, Enter, CTRL+X).
Then reload your .bashrc:

source ~/.bashrc


Now you can type:

ll


and it will run ls -lah.

4. Create a custom prompt

In .bashrc, you can edit the PS1 variable. For example:

PS1="\u@\h:\w$ "


\u → username

\h → hostname

\w → current directory

Example custom style with colors:

PS1="\[\e[32m\]\u@\h:\[\e[34m\]\w\[\e[0m\]$ "


After editing, reload:

source ~/.bashrc

5. Test your customizations

Run ll to see if alias works

Check prompt appearance

Verify $PATH

Ensure environment variables are accessible
