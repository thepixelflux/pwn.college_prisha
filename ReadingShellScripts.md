# Comprehending Commands

## ReadingShellScripts
In this level, we will learn to read shell scripts. /challenge/run is a shell script that requires you to put in a secret password, but that password is hardcoded into the script iself! Read the script (using, say, cat), figure out the password, and get the flag!

### Solve
**Flag:** `pwn.college{YcjO-54Pej6u0gp2L6EL5JuQajQ.0lMwgDOxwiN5EzNzEzW}`

```bash
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run
^C
hacker@chaining~reading-shell-scripts:~$ /challenge/run
hack the PLANET
CORRECT! Your flag:
pwn.college{YcjO-54Pej6u0gp2L6EL5JuQajQ.0lMwgDOxwiN5EzNzEzW}
hacker@chaining~reading-shell-scripts:~$
```
### New Learnings
reading shell scripts by cat command