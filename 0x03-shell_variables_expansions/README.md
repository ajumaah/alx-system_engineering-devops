#Create a script that creates an alias.
we use alias as a command to shorten or bind a single letter in order to original command. 
alias ls = "rm *"

#Create a script that prints hello user, where user is the current Linux user.
echo hello "$(USER)"

2. The path to success is to take massive, determined action
#Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.
export PATH  ="$HOME/action:$PATH"

3. If the path be beautiful, let us not ask where it leads
#Create a script that counts the number of directories in the PATH.
find . -path -c dir |wc -l

4. Global variables
#Create a script that lists environment variables.
printenv

5. Local variables
#Create a script that lists all local variables and environment variables, and functions.
set
6. Local variable
#Create a script that creates a new local variable.
#Name: BEST
#Value: School
BEST="School"

7. Global variable
#Create a script that creates a new global variable.
#Name: BEST
#Value: School
export BEST="School"

8. Every addition to true knowledge is an addition to human power
#Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.
echo '$((128 + TRUEKWOLEDGE))'

9. Divide and rule
#Write a script that prints the result of POWER divided by DIVIDE, followed by a new line.
#POWER and DIVIDE are environment variables
echo $((POWER/DIVID))

10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath
#Write a script that displays the result of BREATH to the power LOVE
#BREATH and LOVE are environment variables
#The script should display the result, followed by a new line

echo '$((BREATH**LOVE))

11. There are 10 types of people in the world -- Those who understand binary, and those who don't
#Write a script that converts a number from base 2 to base 10.
#The number in base 2 is stored in the environment variable BINARY
#The script should display the number in base 10, followed by a new line



