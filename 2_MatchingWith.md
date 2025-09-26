# File globbing

## Matching with ?
Starting from your home directory, change your directory to /challenge, but use the ? character instead of c and l in the argument to cd! Once you're there, run /challenge/run for the flag!

### Solve
**Flag:** `pwn.college{shMkRNOsQPU9RezThkoPCDQJFku.QXyIDO0wiN5EzNzEzW}`

```bash
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{shMkRNOsQPU9RezThkoPCDQJFku.QXyIDO0wiN5EzNzEzW}
hacker@globbing~matching-with-:/challenge$ 
```

### New Learnings
When terminal encounters a ? character in any argument, the shell will treat it as a single-character wildcard. This works like *, but only matches one character