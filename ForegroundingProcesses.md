# Processes and Jobs

## Foregrounding processes
Imagine that you have a backgrounded process, and you want to mess with it some more. What do you do? Well, you can foreground a backgrounded process with fg just like you foreground a suspended process! This level will walk you through that!

### Solve
**Flag:** `pwn.college{cS_gRR22mGMEDVRgzIo1NL2Q9gU.QX4QDO0wiN5EzNzEzW}`

```bash
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the 
background, and *then* foreground it without re-suspending it! You can 
background me with Ctrl-Z (and resume me in the background with 'bg') or, if 
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~foregrounding-processes:~$ 


Yay, I'm now running the background! Because of that, this text will probably 
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times 
to scroll this text out. After that, resume me into the foreground with 'fg'; 
I'll wait.

hacker@processes~foregrounding-processes:~$ fg
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{cS_gRR22mGMEDVRgzIo1NL2Q9gU.QX4QDO0wiN5EzNzEzW}
hacker@processes~foregrounding-processes:~$ 
```
### New Learnings
first we run /challenge/run...then we use ctrl+Z command...then bg ..then finally fg to get the flag
