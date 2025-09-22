# Pondering Paths

## Implicit relative paths
how you specify a particular file, depends on where the terminal prompt is located.To run /challenge/run using a relative path while having a current working directory of /.

### Solve
**Flag:** `pwn.college{ULMseVcry9hWlTTcobFyfATq4Gg.QX5QTN0wiN5EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for any bash commands and output you type on the terminal.

```bash
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{ULMseVcry9hWlTTcobFyfATq4Gg.QX5QTN0wiN5EzNzEzW}
hacker@paths~implicit-relative-paths-from-:/$ 
```

### New Learnings
A relative path is any path that does not start at root (i.e., it does not start with /) and is interpreted relative to your cwd.
