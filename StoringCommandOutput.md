# Shell Variable

## Storing Command Output
 Read the output of the /challenge/run command directly into a variable called PWN, and it will contain the flag!

### Solve
**Flag:** `pwn.college{wrGkKwHojaE_LHyyJTYiVp8hEIj.QX1cDN1wiN5EzNzEzW}`

```bash
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out 
and submit it!
hacker@variables~storing-command-output:~$ echo "$PWN"
pwn.college{wrGkKwHojaE_LHyyJTYiVp8hEIj.QX1cDN1wiN5EzNzEzW}
hacker@variables~storing-command-output:~$ 
```

### New Learnings
follwing the syntax of Command output
variablename=$(directory name)
then to print the flag value prenet inside the variablename use:-
echo "$variablename"

