# File globbing

## Mixing globs
We put a few happy, but diversely-named files in /challenge/files. Go cd there and, using the globbing you've learned, write a single, short (6 characters or less) glob that (when passed as an argument to /challenge/run) will match the files "challenging", "educational", and "pwning"!

### Solve
**Flag:** `pwn.college{k4eUwDtqxZinEu7SxuZRFOmScRA.QX1IDO0wiN5EzNzEzW}`

```bash
hacker@globbing~mixing-globs:~$ cd  /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/files$ /challenge/run [cep]*
bash: /challenge/files$: No such file or directory
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{k4eUwDtqxZinEu7SxuZRFOmScRA.QX1IDO0wiN5EzNzEzW}
hacker@globbing~mixing-globs:/challenge/files$ 
```
### New Learnings
[cep] means filtering out word with c e p 
adding * in front means the starting letter are cep and rest letters can be any