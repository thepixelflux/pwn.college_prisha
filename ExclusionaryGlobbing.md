# Files Globbing

## Exclusionary Globbing
Armed with this knowledge, go forth to /challenge/files and run /challenge/run with all files that don't start with p, w, or n!

### Solve
**Flag:** `pwn.college{45Bfz6Wth_gyNEBlbyBlqbXaP_W.QX2IDO0wiN5EzNzEzW}`

```bash
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{45Bfz6Wth_gyNEBlbyBlqbXaP_W.QX2IDO0wiN5EzNzEzW}
hacker@globbing~exclusionary-globbing:/challenge/files$ 
```

### New Learnings
[!pwn]* is a bracket-negation glob: [!pwn] matches any single character except p, w, or n; the following * allows any characters after that.
Since the glob is unquoted, the shell expands it into the list of filenames that do not start with p, w, or n, and those filenames are passed to /challenge/run.
Note about !: it must be the first character inside the brackets ([!...]) to mean negation.