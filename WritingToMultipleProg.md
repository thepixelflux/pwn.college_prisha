# Practicing Piping

## WritingToMultipleProg
Now it's your turn! In this challenge, we have /challenge/hack, /challenge/the, and /challenge/planet. Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands! Scroll back through the previous challenges "Duplicating piped data with tee" and "Process substitution for input" if you need a refresher on this method.

### Solve
**Flag:** `pwn.college{kEtXCHh2lMsfytpsS7xavAE6B_u.QXwgDN1wiN5EzNzEzW}`

```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >( /challenge/the ) | /challenge/planet
Congratulations, you have duplicated data into the input of two programs! Here 
is your flag:
pwn.college{kEtXCHh2lMsfytpsS7xavAE6B_u.QXwgDN1wiN5EzNzEzW}
```

### New Learnings
-> as we have to run /challenge/hack first...we write /challenge/hack and the duplicate its output into two files using the |  and tee > command.

-> Because the last program (/challenge/planet) is receiving data via a pipe from tee, not as an argument to tee. You only use >(...) when you want to give tee (or any command) a filename-like argument that actually feeds into a process. The pipe (|) already connects stdout→stdin for the last process, so there’s no need for >(...)

-> in the usual usage of tee command, only the arguments you want to be treated as “processes” get >(...)
 
