# Processes and Jobs

## Resuming processes
This challenge's run needs you to suspend it

### Solve
**Flag:** `pwn.college{0_Sy_g35h-jjS1HFHtSoZsCDTot.QX2QDO0wiN5EzNzEzW}`

```bash
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with 
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{0_Sy_g35h-jjS1HFHtSoZsCDTot.QX2QDO0wiN5EzNzEzW}
Don't forget to press Enter to quit me!
^C
hacker@processes~resuming-processes:~$ 
```
### New Learnings
To resume processes, your shell provides the fg command, a builtin that takes the suspended process, resumes it, and puts it back in the foreground of your terminal.
