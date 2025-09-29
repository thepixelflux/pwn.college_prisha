# Untangling Users

## Other users with su
 In this level, you must switch to the zardus user and then run /challenge/run. Zardus' password is dont-hack-me

### Solve
**Flag:** `pwn.college{oYT6KF9hig8k8fKykhNMdRlPGtb.QX2UDN1wiN5EzNzEzW}`


```bash
hacker@users~other-users-with-su:~$ su zardus
Password: 
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{oYT6KF9hig8k8fKykhNMdRlPGtb.QX2UDN1wiN5EzNzEzW}
zardus@users~other-users-with-su:/home/hacker$ 
```
### New Learnings
using the su command to switch to other user