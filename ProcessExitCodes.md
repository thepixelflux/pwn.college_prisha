# Processes and Jobs

## Starting background processes


### Solve
**Flag:** `pwn.college{s8DKUhEHv30CrXNQbuLuack8wzL.QX5YDO1wiN5EzNzEzW}`

```bash
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ /challenge/submit-code $?
CORRECT! Here is your flag:
pwn.college{s8DKUhEHv30CrXNQbuLuack8wzL.QX5YDO1wiN5EzNzEzW}
hacker@processes~process-exit-codes:~$ 
```
### New Learnings
/challenge/get-code=Runs the program that produces a specific exit code.
