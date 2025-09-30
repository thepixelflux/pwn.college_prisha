# Pondering PATH

## the PATH variable
In this level, you will disrupt the operation of the /challenge/run program. This program will DELETE the flag file using the rm command. However, if it can't find the rm command, the flag will not be deleted, and the challenge will give it to you! Thus, you must make it so that /challenge/run also can't find the rm command!

### Solve
**Flag:** `pwn.college{sGc8sGeNT86Ja5T52LOmNdrzklm.QX2cDM1wiN5EzNzEzW}`

```bash
hacker@path~the-path-variable:~$ PATH="" /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{sGc8sGeNT86Ja5T52LOmNdrzklm.QX2cDM1wiN5EzNzEzW}
hacker@path~the-path-variable:~$ 
```
### New Learnings
PATH="" — this sets the PATH environment variable to an empty string. With an empty PATH, the shell will not search any directories for commands referenced by name.

/challenge/run — runs the challenge program by absolute path.

