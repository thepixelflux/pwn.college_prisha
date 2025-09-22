# Pondering Paths

## Position yet elsewhere
Similiar to previous 2 challenges.How to navigate around directories by using the cd (change directory) command and passing a path to it as an argument

### Solve
**Flag:** `pwn.college{82bP5JQ2G3iTqZwhbRBl66RV5xT.QX4QTN0wiN5EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for any bash commands and output you type on the terminal.

```bash
hacker@paths~position-yet-elsewhere:~$ ~
bash: /home/hacker: Is a directory
hacker@paths~position-yet-elsewhere:~$ cd
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /etc/apt/sources.list.d directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /etc/apt/sources.list.d
hacker@paths~position-yet-elsewhere:/etc/apt/sources.list.d$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{82bP5JQ2G3iTqZwhbRBl66RV5xT.QX4QTN0wiN5EzNzEzW}
hacker@paths~position-yet-elsewhere:/etc/apt/sources.list.d$ 
```

### New Learnings
using ~ and cd commands to traverse through different directories

