# Pondering Paths

## Program and absolute paths
execute the program by invoking its absolute path. 

### Solve
**Flag:** `pwn.college{cp51GRF6tkvhw0ErXs1nBOoJ0AP.QX1QTN0wiN5EzNzEzW}`

```bash
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{cp51GRF6tkvhw0ErXs1nBOoJ0AP.QX1QTN0wiN5EzNzEzW}
hacker@paths~program-and-absolute-paths:~$ 
```

### New Learnings
As I learned about the root directory (/) in previous challenge "The Root". The challenge is present in the absolute path and the next level run lives inside the /challenge directory .Thus, the path to the run challenge program is /challenge/run.


