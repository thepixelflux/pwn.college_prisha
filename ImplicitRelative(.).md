# Pondering Path

## Implicit Relative path
how to explicitly use relative paths to launch run in this scenario. The way to do this is to tell Linux that you explicitly want to execute a program in the current directory, using . like in the previous levels

### Solve
**Flag:** `pwn.college{ULkVh7nWXF1XRZj7j6NKxsjILrQ.QXxUTN0wiN5EzNzEzW}`


```bash
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{ULkVh7nWXF1XRZj7j6NKxsjILrQ.QXxUTN0wiN5EzNzEzW}
hacker@paths~implicit-relative-path:/challenge$ 
```

### New Learnings
. = the current directory
./run = the file named run present inside the current directory
You must explicitly prefix with ./ (or another relative/absolute path) to run a program in the current directory
If the path starts with /, it’s an absolute path ... always starts from root, no matter what your cwd is.
If the path starts with ., it’s a relative path ... starts from your cwd.


