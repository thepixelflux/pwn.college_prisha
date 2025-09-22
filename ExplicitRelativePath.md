# Pondering Paths

## Explicit Relative Paths
Previously, your relative path was "naked": it directly specified the directory to descend into from the current directory. In this level, we're going to explore more explicit relative paths.

### Solve
**Flag:** `pwn.college{UvcXyFXFh1raJdNPTysK_WDwMcJ.QXwUTN0wiN5EzNzEzW}`


```bash
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{UvcXyFXFh1raJdNPTysK_WDwMcJ.QXwUTN0wiN5EzNzEzW}
hacker@paths~explicit-relative-paths-from-:/$ 
```

### New Learnings
. =this directory
cd / = so your current working directory is /
./challenge/run = in the current directory (.), go into challenge, then execute run

