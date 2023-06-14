0x03. Shell, init files, variables and expansions

describing what each script is doing

1. alias ls="rm *" - This will create an alias named ls that will execute the command rm *. Please note that this is a dangerous command as it will delete all files in the current directory. You should be careful when using it.
2. echo "hello $USER" - To print “hello user” where user is the current Linux user in the shell, you can use the following command in the terminal echo "hello $USER". The $USER environment variable contains the name of the current user logged in to the shell.
