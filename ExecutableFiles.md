# Perceiving Permissions

## Executable files
In this challenge, the /challenge/run program will give you the flag, but you must first make it executable! Remember your chmod, and get /challenge/run to tell you the flag!

### Solve
**Flag:** `pwn.college{UEPR1U6asApCB-IfPKE66iWRNUJ.QXyEjN0wiN5EzNzEzW}`

```bash
hacker@permissions~executable-files:~$ chmod u+x /challenge/run && /challenge/run
Successful execution! Here is your flag:
pwn.college{UEPR1U6asApCB-IfPKE66iWRNUJ.QXyEjN0wiN5EzNzEzW}
hacker@permissions~executable-files:~$ 
```
### New Learnings
chmod u+x /challenge/run
u+x = you (owner) can run it → this is what you need.

u+x = add execute permission for the owner only
You, as the owner, can now execute the file.