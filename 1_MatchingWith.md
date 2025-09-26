# File Globbing

## Matching with *
Starting from your home directory, change your directory to /challenge, but use globbing to keep the argument you pass to cd to at most four characters! Once you're there, run /challenge/run for the flag!

### Solve
**Flag:** `pwn.college{8G_UuljIfYw-1Uen9TsYsH95HmZ.QXxIDO0wiN5EzNzEzW}`

```bash
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{8G_UuljIfYw-1Uen9TsYsH95HmZ.QXxIDO0wiN5EzNzEzW}
hacker@globbing~matching-with-:/challenge$
```

### New Learnings
* is a wildcard that matches any number of characters in filenames (except / and a leading .).
When you type a command with a *, the shell expands it to all matching files or directories before running the command.
If there are no matches, the glob usually stays unchanged.
Globs can make it easier to work with long or unknown names as in our case /ch* expanded into /challenge, letting us use only 4 characters as the command argument.