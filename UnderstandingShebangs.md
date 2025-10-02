# Chaining commands

## Understanding shebangs
For this challenge, create a script at /home/hacker/solve.sh that has a proper shebang and outputs "hack the planet". Remember to make it executable, then run /challenge/run to verify your script works correctly!

FUN FACT: Common shebangs you might see:

#!/bin/bash for bash scripts
#!/usr/bin/python3 for Python scripts
#!/bin/sh for POSIX shell scripts --- this is a more primitive predecessor to bash with fewer features, but more compatibility to non-Linux systems!

### Solve
**Flag:** `pwn.college{YC2KcXI8Au6QQ6h4WT4wAGdCfwR.0VOzMDOxwiN5EzNzEzW}`

```bash
hacker@practice~chaining~understanding-shebangs:~$ nano solve.sh
hacker@practice~chaining~understanding-shebangs:~$ chmod a=rwx /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run
Testing your script...
Perfect! Your flag:
Flag: pwn.college{YC2KcXI8Au6QQ6h4WT4wAGdCfwR.0VOzMDOxwiN5EzNzEzW}
```
### New Learnings
using nano to edit the file and chmod to make it executable
using bash commands in script shell