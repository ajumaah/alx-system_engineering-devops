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
