# Processes and Jobs

## Starting background processes
Here, sleep is actively running in the background, not suspended. Now it's your turn to practice! Launch /challenge/run backgrounded for the flag!

### Solve
**Flag:** `pwn.college{IQZgzQelKqg1ps7R0MpAFC_TKhK.QX5QDO0wiN5EzNzEzW}`

```bash
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 156
hacker@processes~starting-backgrounded-processes:~$ 


Yay, you started me in the background! Because of that, this text will probably 
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{IQZgzQelKqg1ps7R0MpAFC_TKhK.QX5QDO0wiN5EzNzEzW}
^C
[1]+  Done                    /challenge/run
hacker@processes~starting-backgrounded-processes:~$ 
```
### New Learnings
you can start them backgrounded right off the bat! It's easy; all you have to do is append a & to the command
