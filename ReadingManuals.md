# Digesting Documentation

## Reading Manuals
The challenge in this level has a secret option that, when you use it, will cause the challenge to print the flag. You must learn this option through the man page for challenge!

### Solve
**Flag:** `pwn.college{42Olf8IRqbwJF_0KCHk1oyhl1Ze.QX0EDO0wiN5EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for any bash commands and output you type on the terminal.

```bash
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ 
hacker@man~reading-manuals:~$ /challenge/challenge --lfqbwk 428
Correct usage! Your flag: pwn.college{42Olf8IRqbwJF_0KCHk1oyhl1Ze.QX0EDO0wiN5EzNzEzW}
```

### New Learnings
When you opened the manpage (man challenge) you saw three useful sections:
NAME — program path and short purpose: /challenge/challenge - print the flag!
SYNOPSIS — how to call the program: challenge OPTION
DESCRIPTION — explanations of the options.
then we were supposed to find the special option which was --lfqbwk NUM....and we saw that NUM must be 428