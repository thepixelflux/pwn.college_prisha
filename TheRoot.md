# Pondering Paths

## The Root
Invoke the pwn program using its absolute path, and Capture that Flag

### Solve
**Flag:** `pwn.college{MZAzBnNVTw-kksoZFCUa_i6RA0U.QX4cTO0wiN5EzNzEzW}`

Invoke a program by providing its path on the command line. In this case, you'll be giving the exact path, starting from /, so the path would be /pwn. This style of path, one that starts with the root directory, is referred to as an "absolute path".

```bash
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{MZAzBnNVTw-kksoZFCUa_i6RA0U.QX4cTO0wiN5EzNzEzW}
hacker@paths~the-root:~$ ^C
```

### New Learnings
from this i understood that the filesystem starts at /. Under that, there are a whole mess of other directories, configuration files, programs, and, most importantly, flags can be present.

