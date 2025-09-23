# Comprehending Commands

## Listing files
In this challenge, we've named /challenge/run with some random name! List the files in /challenge to find it.e

### Solve
**Flag:** `pwn.college{o5gpPQFQSMaVd4-p6WVbN0r5TG3.QX4IDO0wiN5EzNzEzW}`


```bash
hacker@commands~listing-files:~$ ls /challenge
2394-renamed-run-13589  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/2394-renamed-run-13589
Yahaha, you found me! Here is your flag:
pwn.college{o5gpPQFQSMaVd4-p6WVbN0r5TG3.QX4IDO0wiN5EzNzEzW}
hacker@commands~listing-files:~$ 
```
### New Learnings
ls will list files in all the directories provided to it as arguments, and ls will find all the files in the current directory if no arguments are provided...just like here we did with challenges and when it was randomly renamed


