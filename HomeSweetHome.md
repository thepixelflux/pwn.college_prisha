# Pondering Path

## Home sweet home
In this challenge, /challenge/run will write a copy of the flag to any file you specify as an argument on the commandline, with these constraints:
1.Your argument must be an absolute path.
2.The path must be inside your home directory.
3.Before expansion, your argument must be three characters or less.

### Solve
**Flag:** `pwn.college{cLcVE4aawVL0FifpgxHGnasP_2E.QXzMDO0wiN5EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for any bash commands and output you type on the terminal.

```bash
hacker@paths~home-sweet-home:~$ /
bash: /: Is a directory
hacker@paths~home-sweet-home:~$ /home
bash: /home: Is a directory
hacker@paths~home-sweet-home:~$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{cLcVE4aawVL0FifpgxHGnasP_2E.QXzMDO0wiN5EzNzEzW}
```

### New Learnings
~/a means:/home/hacker/a where a is just the name of the file where the flag will be stored.can be any random letter too.
Why we put ~/a after /challenge/run?
The syntax for running the program is:/challenge/run ARGUMENT
ARGUMENT tells /challenge/run where to write the flag.
So we provide ~/a as that argument:

three characters or less in the one of the 3 conditions mean that the literal string you type: ~+/+a (before the shell replaces ~ with /home/hacker).

Typed: ~/a → 3 characters
Expanded: /home/hacker/a → absolute path inside home ✅

