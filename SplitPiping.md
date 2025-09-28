# Practicing Piping

## Split-piping
You will need to combine your knowledge of >(), 2>, and |. How to do it is a task I'll leave to you.

In this challenge, you have:

/challenge/hack: this produces data on stdout and stderr
/challenge/the: you must redirect hack's stderr to this program
/challenge/planet: you must redirect hack's stdout to this program

### Solve
**Flag:** `pwn.college{smCmJ4qZL0SRmW9db-04achOtjp.QXxQDM2wiN5EzNzEzW}`

```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 1> >(/challenge/planet) 2> >(/challenge/the)
Congratulations, you have learned a redirection technique that even experts 
struggle with! Here is your flag:
pwn.college{smCmJ4qZL0SRmW9db-04achOtjp.QXxQDM2wiN5EzNzEzW}
hacker@piping~split-piping-stderr-and-stdout:~$ 
```

### New Learnings
This runs /challenge/hack and sends its stdout to /challenge/planet and its stderr to /challenge/the. One of those programs should print the flag when given the correct stream.

> means “redirect stdout” (same as 1> explicitly).

>2 (stderr). 2> means “send stderr somewhere”.

 
