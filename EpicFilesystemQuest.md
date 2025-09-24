# Comprehending Commands

## An epic filesystem quest
In this challenge, I have hidden the flag! Here, you will use ls and cat to follow my breadcrumbs and find it! Here's how it'll work:

Your first clue is in /. Head on over there.
Look around with ls. There'll be a file named HINT or CLUE or something along those lines!
cat that file to read the clue!
Depending on what the clue says, head on over to the next directory (or don't!).
Follow the clues to the flag!

### Solve
**Flag:** `pwn.college{4MRAO9Ch-wxHwS4Ylnh5mlG8n-h.QX5IDO0wiN5EzNzEzW}`


```bash
hacker@commands~an-epic-filesystem-quest:~$ ls /
WHISPER  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin      challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:~$ cat /WHISPER
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/include/config/associative

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:~$ ^C
hacker@commands~an-epic-filesystem-quest:~$ ls -a
.  ..  .bash_history  .config  a  college
hacker@commands~an-epic-filesystem-quest:~$ ls -a /opt/linux/linux-5.4/include/config/associative
.  ..  .INFO  array.h
hacker@commands~an-epic-filesystem-quest:~$ cat /opt/linux/linux-5.4/include/config/associative/.INFO
Lucky listing!
The next clue is in: /usr/lib/python3/dist-packages/urllib3/contrib

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:~$ ls -a /usr/lib/python3/dist-packages/urllib3/contrib
.   .NOTE        __pycache__            _securetransport  ntlmpool.py   securetransport.py
..  __init__.py  _appengine_environ.py  appengine.py      pyopenssl.py  socks.py
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/lib/python3/dist-packages/urllib3/contrib/.NOTE
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/lib/lz4
hacker@commands~an-epic-filesystem-quest:~$ ls -a /opt/linux/linux-5.4/lib/lz4
.   .built-in.a.cmd        Makefile  built-in.a      lz4_decompress.c  lz4defs.h
..  .lz4_decompress.o.cmd  SNIPPET   lz4_compress.c  lz4_decompress.o  lz4hc_compress.c
hacker@commands~an-epic-filesystem-quest:~$ cat /opt/linux/linux-5.4/lib/lz4/SNIPPET
Tubular find!
The next clue is in: /opt/linux/linux-5.4/tools/perf/lib/tests

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:~$ ls -a /opt/linux/linux-5.4/tools/perf/lib/tests
.  ..  .DOSSIER  Makefile  test-cpumap.c  test-evlist.c  test-evsel.c  test-threadmap.c
hacker@commands~an-epic-filesystem-quest:~$ cat /opt/linux/linux-5.4/tools/perf/lib/tests/.DOSSIER
Great sleuthing!
The next clue is in: /usr/share/icons/hicolor/scalable/stock/object

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:~$ ls -a /usr/share/icons/hicolor/scalable/stock/object
.  ..  .MESSAGE
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/share/icons/hicolor/scalable/stock/object/.MESSAGE
Tubular find!
The next clue is in: /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX/SizeThreeSym/Bold
hacker@commands~an-epic-filesystem-quest:~$ ls -a /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX/SizeThreeSym/Bold
.  ..  Main.js  REVELATION
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX/SizeThreeSym/Bold/REVELATION
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/include/config/compat/binfmt

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:~$ cd /opt/linux/linux-5.4/include/config/compat/binfmt
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/compat/binfmt$ ls -a
.  ..  POINTER  elf.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/compat/binfmt$ cat POINTER
Congratulations, you found the clue!
The next clue is in: /usr/lib/debug/.build-id/2e

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/compat/binfmt$ ls -a /usr/lib/debug/.build-id/2e
.  ..  22fecbf93060418578684bd152e0004e0d27b9.debug  834668d12a2606600e4f13dd2fba2c6cb8fbc6.debug  SECRET-TRAPPED
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/compat/binfmt$ cat /usr/lib/debug/.build-id/2e/SECRET-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{4MRAO9Ch-wxHwS4Ylnh5mlG8n-h.QX5IDO0wiN5EzNzEzW}
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/compat/binfmt$ ^C
```

### New Learnings
Understanding how to traverse through files and directories using absolute path and cd whenever required and as per per asked
using ls and ls -a to read files and hidden files
using cat to derive the hidden files
