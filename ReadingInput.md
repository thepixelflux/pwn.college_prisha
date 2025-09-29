# Shell Variable

## Reading Input
your job is to use read to set the PWN variable to the value COLLEGE

### Solve
**Flag:** `pwn.college{gvdavy5U9ICxgM-U41ru9wP6Asg.QX4cTN0wiN5EzNzEzW}`

```bash
hacker@variables~reading-input:~$ PWN=COLLEGE
You've set the first PWN variable properly, but you seem to not have used 
'read' to do it. Please set it using 'read'
hacker@variables~reading-input:~$ echo $PWN
COLLEGE
You've set the first PWN variable properly, but you seem to not have used 
'read' to do it. Please set it using 'read'
hacker@variables~reading-input:~$ ^C
You've set the first PWN variable properly, but you seem to not have used 
'read' to do it. Please set it using 'read'
hacker@variables~reading-input:~$ read PWN
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{gvdavy5U9ICxgM-U41ru9wP6Asg.QX4cTN0wiN5EzNzEzW}
hacker@variables~reading-input:~$ 
```

### New Learnings
here we use the read command to read the value that has been stored in PWN variable

