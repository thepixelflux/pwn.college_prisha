# Shell Variable

## Printing Exported Variable
Try the env command: it'll print out every exported variable set in your shell, and you can look through that output to find the FLAG variable!

### Solve
**Flag:** `pwn.college{8R-x-2-lqdgFRreKyYwjFMsumDI.QX4UTN0wiN5EzNzEzW}`


```bash
hacker@variables~printing-exported-variables:~$ printenv FLAG
pwn.college{8R-x-2-lqdgFRreKyYwjFMsumDI.QX4UTN0wiN5EzNzEzW}
hacker@variables~printing-exported-variables:~$ 
```

### New Learnings
printenv command directly prints the value of the exported FLAG
