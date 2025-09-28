# Practicing Piping

## Grepping stored results
Redirect the output of /challenge/run to /tmp/data.txt.
This will result in a hundred thousand lines of text, with one of them being the flag, in /tmp/data.txt.
grep that for the flag!

### Solve
**Flag:** `pwn.college{Qxu4P4n1RZVfnxsxOyjTLXPh6dy.QX4EDO0wiN5EzNzEzW}`

```bash
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep "pwn.college" /tmp/data.txt
pwn.college{Qxu4P4n1RZVfnxsxOyjTLXPh6dy.QX4EDO0wiN5EzNzEzW}
```

### New Learnings
grep command is used to search for specific text patterns inside files or outputs of other commands. 
***
Output Redirection (>): /challenge/run > /tmp/data.txt
Runs the program /challenge/run.
Takes stdout (standard output) of that program.
Redirects it into the file /tmp/data.txt.

***
Input Redirection (<): /challenge/run < /tmp/data.txt
Runs the program /challenge/run.
Instead of waiting for you to type input (from keyboard), it takes input from the file /tmp/data.txt.
That file’s content is fed to the program as its stdin (standard input).