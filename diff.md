# Comprehending Commands

## Comparing Files
/challenge/decoys_only.txt contains 100 fake flags
/challenge/decoys_and_real.txt contains all 100 fake flags plus the one real flag
Use diff to find what's different between these files and get your flag!

### Solve
**Flag:** `pwn.college{sXo0Y5STFQcM6SrEiYRrKkrBca9.01MwMDOxwiN5EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for any bash commands and output you type on the terminal.

```bash
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
32a33
> pwn.college{sXo0Y5STFQcM6SrEiYRrKkrBca9.01MwMDOxwiN5EzNzEzW}
hacker@commands~comparing-files:~$ 
```

### New Learnings
the command diff shows differences between two files line by line.
the syntax is diff file1 file2



