0x02-shell_redirections in this lesson we will learn on how to redirect outputs and inputs of files. This is the third lesson on devops working with shell.
Requirements General
Allowed editors: vi, vim, emacs
All your scripts will be tested on Ubuntu 20.04 LTS
All your scripts should be exactly two lines long ($ wc -l file should print 2)
All your files should end with a new line (why?)
The first line of all your files should be exactly #!/bin/bash
A README.md file, at the root of the folder of the project, describing what each script is doing
You are not allowed to use backticks, &&, || or ;
All your files must be executable
You are not allowed to use sed or awk

The tasks are as below
0. Hello World
Write a script that prints “Hello, World”, followed by a new line to the standard output. This is the first task and 0-hello_world is the file that contains our script.
 echo "Hello, World"

1. Confused smiley
Write a script that displays a confused smiley "(Ôo)'.
echo "\"(Ôo)'"

2. Let's display a file
Display the content of the /etc/passwd file
cat /etc/passwd

3. What about 2?
Display the content of /etc/passwd and /etc/hosts
less  /etc/passwd /etc/host

4. Last lines of a file
Display the last 10 lines of /etc/passwd
ls -lt | tail /etc/passwd

5. I'd prefer the first ones actually
Display the first 10 lines of /etc/passwd
ls -lt | head /etc/passwd

6. Line #2
Write a script that displays the third line of the file iactaThe file iacta will be in the working directory
You’re not allowed to use sed
cat iacta |head -3 |tail -1 or
head -n 3 iacta|tail -1 
will give the same output.

7. It is a good file that cuts iron without making a noise
Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.
echo "Best School">  \\\*\\\\"'\"Best School\"\\'"\\\\\*

\$\\\?\\\*\\\*\\\*\\\*\\\*\:\)

Save current state of directory
Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.
ls -la >ls_cwd_content
9. Duplicate last line
Write a script that duplicates the last line of the file iacta
tail -n 1 iacta  >>iacta
10. No more javascript
Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.
find . -type f -name "*.js" -rm

11. Don't just count your directories, make your directories count
Write a script that counts the number of directories and sub-directories in the current directory.
find . -type d -not -name '.' |wc -l
12. What’s new
Create a script that displays the 10 newest files in the current directory.
Requirements:
One file per line
Sorted from the newest to the oldest
ls -t1|head -n 10

12-newest_files
Create a script that takes a list of words as input and prints only words that appear exactly once.
Input format: One line, one word
Output format: One line, one word
Words should be sorted

ls -la|sort|uniq -u

14. It must be in that file
Display lines containing the pattern “root” from the file /etc/passwd
grep -i 'root' /etc/passwd #we use grep to match root with option -i to ignore-case
