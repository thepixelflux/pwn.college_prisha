# Chaining Commands

## Scripting with conditionals
For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument
If the argument is "pwn", output "college"
For any other input, output nothing

### Solve
**Flag:** `pwn.college{Aa1kDjdgXeGn3EaP3zk4GrPyzJ3.0lNzMDOxwiN5EzNzEzW}`

```bash
hacker@chaining~scripting-with-conditionals:~$ nano solve/sh
hacker@chaining~scripting-with-conditionals:~$ nano solve.sh
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{Aa1kDjdgXeGn3EaP3zk4GrPyzJ3.0lNzMDOxwiN5EzNzEzW}
```
### New Learnings
in the bash we write:
#!/bin/sh

if [ "$1" = "pwn" ]; then
  printf '%s\n' "college"
fi
