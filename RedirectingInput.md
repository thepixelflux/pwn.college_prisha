# Practicing Piping

## Redirecting input
You can do interesting things with a lot of different programs using input redirection! In this level, we will practice using /challenge/run, which will require you to redirect the PWN file to it and have the PWN file contain the value COLLEGE! To write that value to the PWN file, recall the prior challenge on output redirection from echo!

### Solve
**Flag:** `pwn.college{42yqN1U_ODd-91wwxqJQDoi2wHY.QXwcTN0wiN5EzNzEzW}`

```bash
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read 
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{42yqN1U_ODd-91wwxqJQDoi2wHY.QXwcTN0wiN5EzNzEzW}
hacker@piping~redirecting-input:~$
```

### New Learnings
echo syntax:
echo inputmssg > file(inwhichuhvtoinputmssg)
xyz/rew < file (if u wanna redirect the file to a certain directory)