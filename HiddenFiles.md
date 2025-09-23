# Comprehending Commands

## Hidden files
Go find the flag, hidden as a dot-prepended file in /.

### Solve
**Flag:** `pwn.college{MRbhN67-_Bg_tA0iDhV_EM7oHNK.QXwUDO0wiN5EzNzEzW}`

```bash
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls
bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-16340791214423  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-16340791214423
pwn.college{MRbhN67-_Bg_tA0iDhV_EM7oHNK.QXwUDO0wiN5EzNzEzW}
hacker@commands~hidden-files:/$ 
```

### New Learnings
first we go to / by using cd. then using ls -a to find the hidden files. then show the content of this hidden file by cat(as we wanted to read)