# Shell Variable

## Reading Files
use that to read /challenge/read_me into the PWN environment variable, and we'll give you the flag! The /challenge/read_me will keep changing, so you'll need to read it right into the PWN variable with one command!

### Solve
**Flag:** `pwn.college{UPZHYZvtu6kbvsSFyjzhHRmvxCB.QXwIDO0wiN5EzNzEzW}`


```bash
hacker@variables~reading-files:~$ read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{UPZHYZvtu6kbvsSFyjzhHRmvxCB.QXwIDO0wiN5EzNzEzW}
hacker@variables~reading-files:~$ 
```
### New Learnings
putting what u want to assign to a variable in ""
