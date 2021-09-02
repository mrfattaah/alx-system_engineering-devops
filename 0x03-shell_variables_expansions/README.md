0.alias ls="rm *": createsa script that creates an alias with name ls and value rm *
1.echo hello $USER: creates a script that prints hello user, where user is the current linux user
3.export PATH=$PATH:/action: adds /action to the PATH. /action should be the last directory the shell looks into when looking for a program
4.printenv: lists environment variables
5.set: lists all local variables and environment variables, and functions
6.BETTY="Holberton": creates a new local variable
7.export HOLBERTON="Betty": creates a new global variable
8.echo "$((TRUEKNOWLEDGE+=128))":  prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line
9.echo $((POWER/DIVIDE)):  prints the result of POWER divided by DIVIDE, followed by a new line
10.echo $((BREATH**LOVE)): displays the result of BREATH to the power LOVE
11.echo "$((2#$BINARY))":  converts a number from base 2 to base 10
12.printf "%s\n" {a..z}{a..z} | grep -v "oo": prints all possible combinations of two letters, except oo
13.printf "%.2f\n" $NUM: prints a number with two decimal places, followed by a new line
14.printf "%x\n" $DECIMAL: converts a number from base 10 to base 16
15.tr 'a-zA-Z' 'n-za-mN-ZA-M': encodes and decodes text using the rot13 encryption. Assume ASCII
16.cat -n | grep [13579][[:space:]] | tr -s ' ' | cut -f2: prints every other line from the input, starting with the first line
17.printf "%o\n" $((5#`echo $WATER | tr 'water' '01234'` + 5#`echo $STIR | tr 'stir.' '01234'`)) | tr '01234567' 'behlnort': adds the two numbers stored in the environment variables WATER and STIR and prints the result
