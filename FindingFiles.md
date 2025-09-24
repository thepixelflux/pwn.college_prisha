# Compreh3ending Commands

## Finding files
First, there are other files named flag on the filesystem. Don't panic if the first one you try doesn't have the actual flag in it. Second, there're plenty of places in the filesystem that are not accessible to a normal user. These will cause find to generate errors, but you can ignore those; we won't hide the flag there

### Solve
**Flag:** `pwn.college{4qdEMNOO6NwrCf2CvNCdsgIlLn3.QXyMDO0wiN5EzNzEzW}`


```bash
hacker@commands~finding-files:~$ find / -name flag
find: ‘/root’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
find: ‘/tmp/tmp.TpSOPGOVKK’: Permission denied
/usr/local/lib/python3.8/dist-packages/pwnlib/flag
/usr/lib/debug/.build-id/89/flag
^C
hacker@commands~finding-files:~$ cat /usr/lib/debug/.build-id/89/flag
pwn.college{4qdEMNOO6NwrCf2CvNCdsgIlLn3.QXyMDO0wiN5EzNzEzW}
```

### New Learnings
using find command to find a certain directory
