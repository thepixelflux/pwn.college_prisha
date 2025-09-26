# File Globbing

## Multiple Globs
We put a few happy, but diversely-named files in /challenge/files. Go cd there and run /challenge/run, providing a single argument: a short (3 characters or less) globbed word with two * globs in it that covers every word that contains the letter p.

### Solve
**Flag:** `pwn.college{4oGpH-x9h-6WluuTDEADzL5_xP8.0lM3kjNxwiN5EzNzEzW}`

```bash
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{4oGpH-x9h-6WluuTDEADzL5_xP8.0lM3kjNxwiN5EzNzEzW}
hacker@globbing~multiple-globs:/challenge/files$ ^
```

### New Learnings
* → in shell globs, matches zero or more characters.
p → is the literal letter p.
*p* → matches any filename that has the letter p somewhere in it.

You pass *p* (literally) to /challenge/run.The program then uses it to find all files in /challenge/files whose names contain p
