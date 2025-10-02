# Practicing Piping

## Duplicating piped data with tee
This process' /challenge/pwn must be piped into /challenge/college, but you'll need to intercept the data to see what pwn needs from you!

### Solve
**Flag:** `pwn.college{AJQTPER_t9H3TM_A9Z1WvjWhhp4.QXxITO0wiN5EzNzEzW}`

```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee flag | /challenge/college
Processing...
WARNING: you are overwriting file flag with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat /flag
cat: /flag: Permission denied
hacker@piping~duplicating-piped-data-with-tee:~$ cat flag
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "AJQTPER_"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret AJQTPER_ | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{AJQTPER_t9H3TM_A9Z1WvjWhhp4.QXxITO0wiN5EzNzEzW}
hacker@piping~duplicating-piped-data-with-tee:~$
```
### New Learnings
tee flag duplicates the output ...one copy goes to flag and other copy goes to pipe into /challenge/college
it saves a copy of data while still letting it go into pipe at the same time