# Processes and Jobs

## Suspending processes
This level's run wants to see another copy of itself running and using the same terminal. How? Use the terminal to launch it, then suspend it, then launch another copy while the first is suspended!

### Solve
**Flag:** `pwn.college{MfhgebVqTcNA1Q7PLm8iPLOJF4-.QX1QDO0wiN5EzNzEzW}`

```bash
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in 
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         146     136  0 06:08 pts/0    00:00:00 bash /challenge/run
root         148     146  0 06:08 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can 
background me with Ctrl-Z or, if you're not ready to do that for whatever 
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in 
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         146     136  0 06:08 pts/0    00:00:00 bash /challenge/run
root         153     136  0 06:08 pts/0    00:00:00 bash /challenge/run
root         155     153  0 06:08 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{MfhgebVqTcNA1Q7PLm8iPLOJF4-.QX1QDO0wiN5EzNzEzW}
hacker@processes~suspending-processes:~$ 
```
### New Learnings
we can suspend processes to the background with Ctrl-Z
