# Processes and Jobs

## Killing processes
In this challenge, /challenge/run will refuse to run while /challenge/dont_run is running! You must find the dont_run process and kill it. If you fail, pwn.college will disavow all knowledge of your mission

### Solve
**Flag:** ``

```bash
hacker@processes~killing-processes:~$ ps -efww | grep /challenge | grep dont_run
hacker       136     135  0 05:34 ?        00:00:00 /challenge/dont_run
hacker@processes~killing-processes:~$ kill 136
hacker@processes~killing-processes:~$ ps -efww | grep /challenge | grep dont_run
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{kfLVikM-hDW5v1lMKQD_She-Mkg.QXyQDO0wiN5EzNzEzW}
hacker@processes~killing-processes:~$ 
```
### New Learnings
find written in q= use grep command with |
first find the /challenge with grep then find /dont_run with grep then pipeline them all 
then kill the pid u got 
then we can rerun the command again to confirm if it has been killed. now as the terminal is giving blank output it is killed
then we print the flag using /challenge/run after killing the ongoing /challenge/dont_run command

ps -ef or ps aux — list all running processes (two common formats).

ww (e.g. ps -efww) — prevent truncation of long command lines so you can see full paths.

grep pattern — filter output to lines that contain pattern.

kill PID — send default terminate signal (SIGTERM) to the process with id PID.
