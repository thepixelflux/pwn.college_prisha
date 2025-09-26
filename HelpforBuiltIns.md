# Digesting Documentation

## help for BuiltIns
Some good information! In this challenge, we'll practice using help to look up help for builtins. This challenge's challenge command is a shell builtin, rather than a program. Like before, you need to lookup its help to figure out the secret value to pass to it!
### Solve
**Flag:** `pwn.college{UqU4ZTCLj6_TrvP2yq3zyPnkcfe.QX0ETO0wiN5EzNzEzW}`


```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!
    
    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "UqU4ZTCL".
hacker@man~help-for-builtins:~$ challenge --secret UqU4ZTCL
Correct! Here is your flag!
pwn.college{UqU4ZTCLj6_TrvP2yq3zyPnkcfe.QX0ETO0wiN5EzNzEzW}

hacker@man~help-for-builtins:~$ 
```

### New Learnings
Brief note on what you learned from the challenge

### References 
Add any references or videos you used while solving the challenge.
