# Processes and Jobs

## Interrupting processes
Try it here! /challenge/run will refuse to give you the flag until you interrupt it

### Solve
**Flag:** `pwn.college{kDGzw50TaWyjuoCC3vozV_cCfDS.QXzQDO0wiN5EzNzEzW}`

```bash
hacker@processes~interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember, 
you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:
pwn.college{kDGzw50TaWyjuoCC3vozV_cCfDS.QXzQDO0wiN5EzNzEzW}
hacker@processes~interrupting-processes:~$ 
```
### New Learnings
 sometimes you just want to get rid of the process that's clogging up your terminal. for that terminals have a hotkey for this: Ctrl-C (e.g., holding down the Ctrl key and pressing C) sends an "interrupt" to whatever application is waiting on input from the terminal and, typically, this causes the application to cleanly exit.
