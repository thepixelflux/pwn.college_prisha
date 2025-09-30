# Processes and Jobs

## Killing misbehaving processes
Check what processes are running.
Find /challenge/decoy in the list and figure out its process ID.
kill it.
Run /challenge/run to get the flag without being overwhelmed by decoys (you don't need to redirect its output; it'll write to the FIFO on its own).

### Solve
**Flag:** `pwn.college{AaHAceICH9kLXmFpmfIKEik2ful.0FNzMDOxwiN5EzNzEzW}`

```bash
hacker@processes~killing-misbehaving-processes:~$ ps aux | grep /challenge/decoy
root         139  0.0  0.0   5204  3520 ?        S    06:02   0:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
hacker       142  0.6  0.0  13516  9280 ?        Ss   06:02   0:00 /usr/bin/python /challenge/decoy
hacker       168  0.0  0.0 230696  2560 pts/0    S+   06:02   0:00 grep --color=auto /challenge/decoy
hacker@processes~killing-misbehaving-processes:~$ kill 142 
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{AaHAceICH9kLXmFpmfIKEik2ful.0FNzMDOxwiN5EzNzEzW}
hacker@processes~killing-misbehaving-processes:~$ 
```
### New Learnings
in the first line we see all decoy processes by ps -aux and then use grep to find the ones that contain /challenge/decoy
then we kill the pid
Run the real writer and then use cat to see the flag inside fifo file
