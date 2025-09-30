# Processes and Jobs

## Listing processes
 In this level, I have once again renamed /challenge/run to a random filename, and this time made it so that you cannot ls the /challenge directory! But I also launched it, so you can find it in the running process list, figure out the filename, and relaunch it directly for the flag

### Solve
**Flag:** `pwn.college{s3Fh8m9nLR71zp-rHUAPixQrDjI.QX4MDO0wiN5EzNzEzW}`

```bash
hacker@processes~listing-processes:~$ ps aux | grep /challenge
root         132  0.0  0.0   4132  2560 ?        S    05:23   0:00 /challenge/3372-run-26345
hacker       166  0.0  0.0 230696  2560 pts/0    S+   05:27   0:00 grep --color=auto /challenge
hacker@processes~listing-processes:~$ ^C
hacker@processes~listing-processes:~$ /challenge/3372-run-26345
Yahaha, you found me! Here is your flag:
pwn.college{s3Fh8m9nLR71zp-rHUAPixQrDjI.QX4MDO0wiN5EzNzEzW}
Now I will sleep for a while (so that you could find me with 'ps'). 
```
### New Learnings
ps -ef
ps = list processes
-e = show every process
-f = show full format

| grep /challenge
| = pipe the output of ps into another command....and grep /challenge = only show lines containing the word /challenge.
A pipe is used to connect two commands.It takes the output of the command on the left and sends it as the input to the command on the right.
using grep....as we have to "find" ....grep searches for text inside files or command output and shows the matching lines