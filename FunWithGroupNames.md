# Perceiving Permissions

## Fun with group names
The point is, you've used hacker for the group before, but in this level, that is not going to work. I'll still allow you to use chgrp, but I have randomized the name of the group that your user is in. You will need to use the id command to figure that name out, then chgrp to victory!

### Solve
**Flag:** `pwn.college{oSPJd4B-PAhYNg06ejgsUTkqfOE.QXycjM1wiN5EzNzEzW}`

```bash
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp28064) groups=1000(grp28064)
hacker@permissions~fun-with-groups-names:~$ chgrp grp28064 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{oSPJd4B-PAhYNg06ejgsUTkqfOE.QXycjM1wiN5EzNzEzW}
hacker@permissions~fun-with-groups-names:~$ 
```
### New Learnings
id := prints your user id and group membership information.

chgrp g42x /flag:= changes the group owner of the file /flag to the group 
chgrp = change group. Syntax: chgrp <groupname> <path>