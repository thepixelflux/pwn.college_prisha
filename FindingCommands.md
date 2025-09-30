# Pondering PATH

## Finding commands
In this challenge, we added a win command somewhere in your $PATH, but it won't give you the flag. Instead, it's in the same directory as a flag file that we made readable by you! You must find win (with the which command), and cat the flag out of that directory!

### Solve
**Flag:** `pwn.college{0xtukcyrcf-95osp5urIMjrbclr.01NzEzNxwiN5EzNzEzW}`

```bash
 hacker@path~finding-commands:~$ which win
/challenge/paths/4394/win
hacker@path~finding-commands:~$ ls /challenge/paths/4394
flag  win
hacker@path~finding-commands:~$ cat /challenge/paths/4394/flag
pwn.college{0xtukcyrcf-95osp5urIMjrbclr.01NzEzNxwiN5EzNzEzW}
hacker@path~finding-commands:~$ 
```
### New Learnings
to find where the win is we use the which command
the directory given by running it contains the flag and then we print the flag by using cat command