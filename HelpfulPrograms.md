# Digesting Documentations

## Searching for Manuals
In this level, you will practice reading a program's documentation with --help.

### Solve
**Flag:** `pwn.college{oA0mmzwXYwM9bR_IjAOPOaJNyQu.QX3IDO0wiN5EzNzEzW}`

```bash
hacker@man~helpful-programs:~$ /challenge/challenge --h
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 93
hacker@man~helpful-programs:~$ /challenge/challenge -g 93
Correct usage! Your flag: pwn.college{oA0mmzwXYwM9bR_IjAOPOaJNyQu.QX3IDO0wiN5EzNzEzW}
hacker@man~helpful-programs:~$  
```

### New Learnings
by using the --h or --help command we get the -p and the -g commands required to print the flag thereby.