# Pondering Paths

## Position Elsewhere
Navigate around directories by using the cd (change directory) command and passing a path to it as an argument

### Solve
**Flag:** `pwn.college{ojYwBw-MeEqzYRscQln37CMY6zq.QX3QTN0wiN5EzNzEzW}`


```bash
hacker@paths~position-elsewhere:~$ ~
bash: /home/hacker: Is a directory
hacker@paths~position-elsewhere:~$ cd
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /usr/share/doc
hacker@paths~position-elsewhere:/usr/share/doc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{ojYwBw-MeEqzYRscQln37CMY6zq.QX3QTN0wiN5EzNzEzW}
hacker@paths~position-elsewhere:/usr/share/doc$ 
```

### New Learnings
It is similar to the previous challenge where we used ~ to show the current directory location and then using cd to redirect it to the required path in this case was /challenge/run


