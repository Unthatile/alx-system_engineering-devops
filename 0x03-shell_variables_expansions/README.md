0x03. Shell, init files, variables and expansions

Describing What Each Script Is Doing

0. alias ls="rm *" - This will create an alias named ls that will execute the command rm *. Please note that this is a dangerous command as it will delete all files in the current directory. You should be careful when using it.
1. echo "hello $USER" - To print “hello user” where user is the current Linux user in the shell, you can use the following command in the terminal echo "hello $USER". The $USER environment variable contains the name of the current user logged in to the shell.
2. export PATH=$PATH:/action - To add a directory to the PATH in shell, you can use the export command to add a directory to the $PATH variable temporarily or edit the shell configuration files to make the change permanent. In Linux, you can edit the .bashrc file in the Home directory to add a directory to the path permanently.
3. echo $PATH | tr ':' '\n' | wc -l - This command will print the number of directories in your PATH environment variable. The tr ':' '\n' command replaces all colons with newlines so that each directory is on a separate line. The wc -l command counts the number of lines.
4. printenv - To list all environment variables in the shell, you can use the printenv command.
5. To list all shell variables, you can use the set command.
6. BEST="School" - a script that creates a new local variable Name: BEST Value: School.
7. export BEST=School - This will create a new global variable named BEST with the value of School. You can then access this variable from anywhere in your script.
8. echo $((128 + $TRUEKNOWLEDGE)) - The $((...)) syntax is used for arithmetic expansion in Bash. It evaluates the expression inside the parentheses and returns its value. The echo command is used to print the result of the addition to the standard output.
9. echo $(($POWER / $DIVIDE)) - This command will print the result of POWER divided by DIVIDE followed by a new line. Please note that POWER and DIVIDE are environment variables that should be set before running the script. To print all environment variables in a Linux shell script, you can use the env command.
10. echo $(($BREATH ** $LOVE)) - This script uses the echo command to display the result of BREATH to the power LOVE. The $(($BREATH ** $LOVE)) expression calculates the result of BREATH raised to the power of LOVE.
11. echo $((2#$BINARY)) - a script that converts a number from base 2 to base 10. The number in base 2 is stored in the environment variable BINARY. The script should display the number in base 10, followed by a new line.
12. echo {a..z}{a..z} | tr ' ' '\n' | grep -v "oo" - a script that prints all possible combinations of two letters, except oo. Letters are lower cases, from a to z. One combination per line. The output should be alpha ordered, starting with aa. Do not print oo. Your script file should contain maximum 64 characters.
13. printf "%.2f\n" "$NUM" - In this script, the %f format specifier is used to print a floating-point number. The .2 specifies that the number should be printed with two decimal places. The \n at the end of the line is used to print a newline character after the number.
14. printf "%x\n" $DECIMAL - The number in base 10 is stored in the environment variable DECIMAL. The script uses the printf command to convert the decimal number to hexadecimal.
15. tr 'A-Za-z' 'N-ZA-Mn-za-m' - This script uses the tr command to perform the rot13 encryption. The tr command is used to translate or delete characters. In this case, it translates all alphabetic characters by 13 positions in the alphabet
