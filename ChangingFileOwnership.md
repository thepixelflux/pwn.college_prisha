# Perceiving Permissions

## Changing file ownership
we will practice changing the owner of the /flag file to the hacker user, and then read the flag. For this challenge only, I made it so that you can use chown to your heart's content as the hacker user (again, typically, this requires you to be root). Use this power wisely and chown away!

### Solve
**Flag:** `pwn.college{kF4ZgJJ0AYZ3sSP7qtJ1gpuqkJN.QXxEjN0wiN5EzNzEzW}`


```bash
hacker@permissions~changing-file-ownership:~$ ls -l /flag
-r-------- 1 root root 60 Sep 29 21:22 /flag
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{kF4ZgJJ0AYZ3sSP7qtJ1gpuqkJN.QXxEjN0wiN5EzNzEzW}
hacker@permissions~changing-file-ownership:~$
```
### New Learnings
ls -l lists the file (/flag) in long format
chown changes the owner of /flag to the user hacker. After this, hacker becomes the file owner.