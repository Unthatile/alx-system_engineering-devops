0x03. Shell, init files, variables and expansions

describing what each script is doing

1. alias ls="rm *" - This will create an alias named ls that will execute the command rm *. Please note that this is a dangerous command as it will delete all files in the current directory. You should be careful when using it.
2. echo "hello $USER" - To print “hello user” where user is the current Linux user in the shell, you can use the following command in the terminal echo "hello $USER". The $USER environment variable contains the name of the current user logged in to the shell.
3. export PATH=$PATH:/action - To add a directory to the PATH in shell, you can use the export command to add a directory to the $PATH variable temporarily or edit the shell configuration files to make the change permanent. In Linux, you can edit the .bashrc file in the Home directory to add a directory to the path permanently.
4. echo $PATH | tr ':' '\n' | wc -l - This command will print the number of directories in your PATH environment variable. The tr ':' '\n' command replaces all colons with newlines so that each directory is on a separate line. The wc -l command counts the number of lines.
5. printenv - To list all environment variables in the shell, you can use the printenv command.
6. To list all shell variables, you can use the set command.
8. export BEST=School - This will create a new global variable named BEST with the value of School. You can then access this variable from anywhere in your script.
