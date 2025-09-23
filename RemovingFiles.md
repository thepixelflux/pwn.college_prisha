# Comprehending commands

## Removing files
 This challenge will create a delete_me file in your home directory! Delete it, then run /challenge/check,

### Solve
**Flag:** `pwn.college{8ZowuLeUS-3xFtqrijG5N05JkyF.QX2kDM1wiN5EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for any bash commands and output you type on the terminal.

```bash
hacker@commands~removing-files:/$ cd /home/hacker
hacker@commands~removing-files:~$ touch delete_me
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{8ZowuLeUS-3xFtqrijG5N05JkyF.QX2kDM1wiN5EzNzEzW}
hacker@commands~removing-files:~$ 
```

### New Learnings
we go in the home directory which is /home/hacker here..then create a file by touch command used for creating files and after that use rm command to delete tht created file present in /challenge/check

