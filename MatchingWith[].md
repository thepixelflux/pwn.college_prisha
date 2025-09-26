# File globbing

## Matching with []
We've placed a bunch of files in /challenge/files. Change your working directory to /challenge/files and run /challenge/run with a single argument that bracket-globs into file_b, file_a, file_s, and file_h!

### Solve
**Flag:** `pwn.college{ANbEIu7dvHOfeVKjN9tG23RLpOa.QXzIDO0wiN5EzNzEzW}`

```bash
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ ls
file_a  file_c  file_e  file_g  file_i  file_k  file_m  file_o  file_q  file_s  file_u  file_w  file_y
file_b  file_d  file_f  file_h  file_j  file_l  file_n  file_p  file_r  file_t  file_v  file_x  file_z
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{ANbEIu7dvHOfeVKjN9tG23RLpOa.QXzIDO0wiN5EzNzEzW}
```

### New Learnings
[] syntax, also called a character class.
[bash] means “match one character that is either b, a, s, or h.So the shell looked at all filenames in the directory and picked the ones where the last letter matches one of these.
[] matches one character at that position.
Characters can be listed individually ([abc]) or as a range ([a-c]).
