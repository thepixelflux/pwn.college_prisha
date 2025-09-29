# Perceiving Permissions

## Groups and files
In this challenge, you must change the permissions of the /flag file to read it! Typically, you need to have write access to the file in order to change its permissions, but I have made the chmod command all-powerful for this level, and you can chmod anything you want even though you are the hacker user. This is an ultimate power. The /flag file is owned by root, and you can't change that, but you can make it readable. Go and solve this!!

### Solve
**Flag:** `pwn.college{gX2Jsijkfve44TlcjS7Xg1_2bEl.QXzcjM1wiN5EzNzEzW}`

```bash
hacker@permissions~changing-permissions:~$ ls -l /flag
-r-------- 1 root root 60 Sep 29 21:51 /flag
hacker@permissions~changing-permissions:~$ id
uid=1000(hacker) gid=1000(hacker) groups=1000(hacker)
hacker@permissions~changing-permissions:~$ chmod o+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{gX2Jsijkfve44TlcjS7Xg1_2bEl.QXzcjM1wiN5EzNzEzW}
hacker@permissions~changing-permissions:~$ 
```
### New Learnings
chmod o+r /flag: gives the other class the read permission on /flag.

Syntax: chmod WHO±PERM path .... here o = others, + = add, r = read.