# Practising Piping

## Redirecting Output
In this challenge, you must use this output redirection to write the word PWN (all uppercase) to the filename COLLEGE (all uppercase).

### Solve
**Flag:** `pwn.college{MtqzEYIfcSyzaCldhSdAd_uOylt.QX0YTN0wiN5EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for any bash commands and output you type on the terminal.

```bash
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your 
flag:
pwn.college{MtqzEYIfcSyzaCldhSdAd_uOylt.QX0YTN0wiN5EzNzEzW}
hacker@piping~redirecting-output:~$ 
```

### New Learnings
redirecting stdout to files. You can accomplish this with the > character, as so:
for example if we write: echo hi > asdf
This will redirect the output of echo hi (which will be hi) to the file asdf.
