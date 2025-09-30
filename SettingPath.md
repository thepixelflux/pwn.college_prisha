# Pondering PATH

## Setting path
This level's /challenge/run will run the win command via its bare name, but this command exists in the /challenge/more_commands/ directory, which is not initially in the PATH. The win command is the only thing that /challenge/run needs, so you can just overwrite PATH with that one directory. 

### Solve
**Flag:** `pwn.college{UfqWA3_mQH5pK-NfX-SKXoDXYJf.QX1cjM1wiN5EzNzEzW}`

```bash
hacker@path~setting-path:~$ PATH=/challenge/more_commands
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{UfqWA3_mQH5pK-NfX-SKXoDXYJf.QX1cjM1wiN5EzNzEzW}
hacker@path~setting-path:~$ 
```
### New Learnings
PATH stores a list of directories to find commands in and, for commands in nonstandard places, we must typically execute them via their path

