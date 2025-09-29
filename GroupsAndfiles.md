# Perceiving Permissions

## Groups and files
I  have made the flag readable by whatever group owns it, but this group is currently root. Luckily, I have also made it possible for you to invoke chgrp as the hacker user! Change the group ownership of the flag file, and read the flag!

### Solve
**Flag:** `pwn.college{gPkqpHqZVLHQv_OZrYoqVovoOZ-.QXxcjM1wiN5EzNzEzW}`

```bash
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{gPkqpHqZVLHQv_OZrYoqVovoOZ-.QXxcjM1wiN5EzNzEzW}
hacker@permissions~groups-and-files:~$ 
```
### New Learnings
changes the group owner of /flag to the group named hacker.
General syntax: chgrp <groupname> <file-or-dir>