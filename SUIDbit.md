# Percieving permissions

## SUID bit
we are going to let you add the SUID bit to the /challenge/getroot program in order to spawn a root shell for you to cat the flag yourself!

### Solve
**Flag:** `pwn.college{86eOcpKyQNvLs5CEUstLzhQf9RP.QXzEjN0wiN5EzNzEzW}`

```bash
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root! 
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{86eOcpKyQNvLs5CEUstLzhQf9RP.QXzEjN0wiN5EzNzEzW}
root@permissions~the-suid-bit:~# 
 
```
### New Learnings
chmod: This is the command used to change the file mode (permissions) of a file.

u+s: This is the specific permission change being applied:
u stands for the user (the file owner).
+s adds the Set User ID (SUID) bit to the file's permissions.

/challenge/getroot: This is the path to the program whose permissions are being changed.
This line sets the SUID bit on the /challenge/getroot program. This means that no matter which user runs this program, it will execute with the permissions of the owner of the file (which, in this context, is implied to be the powerful root user).

This line simply executes the program located at /challenge/getroot.
then we read the flag suing cat /flag